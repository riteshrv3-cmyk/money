# Chapter 4.3  [DEPTH]
## Message ko tukdon mein todna

---

*DEPTH chapter. Iske baad "internet slow hai," "call kat gayi," aur "video ruk-ruk kar chal raha hai" ek hi tasveer ke hisse ban jaate hain.*

---

### Samvaad

**Madhav:** Ek gaon se doosre gaon tak ek hi sadak hai. Sau log apna saaman bhejna chahte hain. Ek aadmi ka saaman bahut bada hai, poori sadak ghera leta hai, aur pahunchne mein do din lagenge.

**Kabir:** Baaki ninyanve log do din intezaar karenge.

**Madhav:** Achha lagta hai?

**Kabir:** Nahi. Chhote saaman wale pehle nikal jaane chahiye.

**Madhav:** Toh kya karoge?

**Kabir:** Bade saaman ko tukdon mein tod dunga. Har tukda alag bhejunga, aur beech mein doosron ka saaman bhi ja sakta hai.

**Madhav:** Ab problem yeh hai ki tukde alag-alag pahunchenge. Doosri taraf wale ko kaise pata chalega ki kya jodna hai?

**Kabir:** Har tukde pe likh dunga: kiska hai, aur kaunse number ka tukda hai.

**Madhav:** Aur agar tukda number 5 pehle pahunch gaya aur number 3 baad mein?

**Kabir:** Woh number dekh kar sahi order mein rakh lega.

**Madhav:** Aur agar tukda number 3 raaste mein kho gaya?

**Kabir:** Toh... woh dekhega ki 3 nahi aaya, aur dobara maangega.

**Madhav:** Kaise maangega? Use kaise pata chalega ki tukda kho gaya aur dheere nahi aa raha?

**Kabir:** Kuch der intezaar karega. Nahi aaya toh maan lega ki gaya.

**Madhav:** Ab ulta socho. Bhejne wale ko kaise pata chalega ki tukda pahuncha?

**Kabir:** Lene wala bataye ki mil gaya.

**Madhav:** Har tukde ke liye?

**Kabir:** Haan.

**Madhav:** Toh ab har tukde ke liye do baar safar. Ek jaane ka, ek jawab ka. Kya yeh dheema nahi ho jaayega?

**Kabir:** Ho jaayega. Toh... kuch tukde ek saath bhej doon, phir ek hi jawab maangun.

**Madhav:** Kitne ek saath?

**Kabir:** Pata nahi. Zyada bheje toh sadak jaam ho jaayegi.

**Madhav:** Toh kaise tay karoge?

**Kabir:** Dheere se badhaunga. Kaam chal raha hai toh aur bhejo. Kuch khone lage toh kam kar do.

**Madhav:** Tumne abhi internet ka sabse zaroori niyam khud bana diya. Ab aakhri sawal. Ek video call chal rahi hai. Ek tukda kho jaata hai. Kya karoge, dobara maangoge?

**Kabir:** Haan.

**Madhav:** Us tukde mein woh awaaz thi jo aadhe second pehle boli gayi thi. Dobara maangne mein aur aadha second lagega.

**Kabir:** Toh woh purani ho chuki hogi. Bekaar.

**Madhav:** Toh?

**Kabir:** Toh video call mein kho gaya toh chhod do. Aage badho.

**Madhav:** Aur file download mein?

**Kabir:** Wahan ek bhi tukda nahi chhod sakte. File toot jaayegi.

**Madhav:** Bas. Do bilkul alag zaroortein, aur isiliye do alag tareeke.

---

### Naam

Har chhote tukde ko **packet** kehte hain. Aam taur pe ek packet 1,500 byte se chhota hota hai.

Har packet pe likha hota hai:

```
kahan se aaya       (bhejne wale ka pata)
kahan jaana hai     (lene wale ka pata)
kaunse number ka    (taaki order banaya ja sake)
kis baat-cheet ka   (taaki alag baaton ke tukde na milein)
asli saaman         (data)
```

Aur woh do tareeke jo Kabir ne nikaale:

```
TCP   har tukda pahunchna zaroori
      ├── lene wala har baar batata hai ki mila
      ├── kho gaya toh dobara bheja jaata hai
      ├── order theek kiya jaata hai
      └── file, message, website, bank

UDP   pahunche toh theek, na pahunche toh chalo aage
      ├── koi jawab nahi maanga jaata
      ├── kho gaya toh gaya
      ├── tez, kyunki intezaar nahi
      └── video call, live stream, game
```

Aur woh aakhri cheez, dheere se badhana aur girne pe kam karna, use **congestion control** kehte hain.

Yeh internet ka sabse kam dikhne wala aur sabse zaroori hissa hai. Kisi ne kabhi tay nahi kiya ki kis machine ko kitni sadak milegi. Har machine khud koshish karti hai, aur girte hi peeche hat jaati hai. Sab milkar sadak baant lete hain, bina kisi manager ke.

Isiliye jab bahut log ek saath internet istemaal karte hain, toh sabko thoda thoda dheema milta hai, kisi ek ko poora band nahi milta.

---

### Asli duniya se ek example

Aap Netflix pe video dekhte ho. Woh kabhi kabhi dhundhla ho jaata hai aur phir saaf ho jaata hai. Ruk-ruk kar nahi chalta, sirf quality girti hai.

Woh jaan-boojh ke hai. App har waqt naap raha hai ki tukde kitni jaldi aa rahe hain. Jab sadak bhari hoti hai, toh woh chhoti quality wala video maangna shuru kar deta hai, jiske tukde chhote hote hain.

Aap dhundhla dekh lete ho. Rukna aapko bura lagta hai, dhundhlapan utna nahi.

Aur video call mein bilkul ulta chunav hota hai. Wahan woh tukde chhodta hai, quality nahi girata, kyunki der se aayi awaaz kisi kaam ki nahi.

Do alag product, ek hi problem, do ulte hal. Aur dono hal usi chunav se aaye jo Kabir ne khud kar liya tha: **kya purana data kaam ka hai ya nahi.**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **"internet slow hai" ko ek hi cheez samajhna.**

Do bilkul alag cheezein hoti hain, aur unke ilaaj bhi alag hain:

```
BANDWIDTH   ek second mein kitna data aa sakta hai
            (sadak kitni chaudi hai)

LATENCY     ek tukde ko jaane aur wapas aane mein kitna waqt
            (sadak kitni lambi hai)
```

Film download karne mein bandwidth mayne rakhti hai. Video call aur game mein latency mayne rakhti hai.

Isiliye ek bahut tez connection pe bhi call kharaab ho sakti hai, aur ek dheeme connection pe bhi theek chal sakti hai. Aur isiliye satellite internet mein bandwidth bahut ho sakti hai lekin game nahi khela ja sakta: signal ko upar jaakar wapas aana padta hai.

Yeh galti tempting isliye hai ki dono ka nateeja ek jaisa dikhta hai. Cheez dheere ho gayi. Lekin wajah alag hai, aur isliye hal bhi alag hai.

Aur yeh Chapter 2.3 wali baat hai, badi shakal mein: **doori speed se zyada mayne rakhti hai.**

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  PACKET       bade ko tukdon mein todo  │  ← naya
    │  TCP / UDP    pakka, ya tez             │  ← naya
    │  BANDWIDTH vs LATENCY                   │  ← naya
    ├────────────────────────────────────────┤
    │  PATA, NETWORK                          │
    ├────────────────────────────────────────┤
    │  OS, PROCESS, CPU, RAM/DISK, SWITCH     │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek online game mein aapka character ruk-ruk kar chalta hai. Aapka connection 500 Mbps ka hai. Kya problem hai?

> **Jawab:** Bandwidth nahi, latency. Sadak chaudi hai lekin lambi.
>
> Game mein har second kai baar chhoti si jaankari aani-jaani hoti hai, aur har baar jawab ka intezaar hota hai. Agar ek chakkar mein 200 millisecond lagte hain, toh chaudi sadak se koi faayda nahi.
>
> Isiliye gamers ping dekhte hain, speed nahi.
>
> Aur isiliye game ke server aapke sheher ke paas rakhe jaate hain. Woh doori kam karne ke liye hai, taakat badhane ke liye nahi.

**2. (samajh check)** Aap ek file download kar rahe ho aur beech mein internet 5 second ke liye chala jaata hai. File toot jaayegi?

> **Jawab:** Nahi. TCP dobara maang lega.
>
> Bhejne wale ko jawab nahi milega, toh woh un tukdon ko dobara bhejega. Download ruk kar phir chalu ho jaayega.
>
> Ab wahi 5 second ek video call mein hote toh woh awaaz hamesha ke liye chali jaati, kyunki UDP dobara nahi maangta.
>
> Ek hi ghatna, do alag nateeje, aur wajah sirf yeh ki kaunsa tareeka chuna gaya tha.

**3. (jodne wala)** Chapter 4.1 kehta tha ki network mein koi manager nahi hai. Ab pata chala ki sadak bhi koi nahi baant raha. Yeh kaise chal jaata hai?

> **Jawab:** Kyunki har machine khud peeche hat jaati hai jab use dikhta hai ki tukde kho rahe hain.
>
> Koi upar se nahi keh raha ki tum itna hi bhejo. Har ek badhata hai jab tak dard na ho, phir peeche hat jaata hai.
>
> Aur yeh isiliye chalta hai kyunki lagbhag sab log wahi niyam maan rahe hain. Agar koi jaan-boojh ke peeche na hate, toh woh zyada le lega.
>
> Yeh internet ke baare mein sabse zaroori baat hai, aur Chapter 4.7 mein hum ise poora karenge: **internet ek machine nahi hai. Woh ek sehmati hai.**
