# Chapter 6.7  [SPINE]
## Cheezein dheeri kyun lagti hain

---

### Samvaad

**Madhav:** Ek button dabaya aur jawab aane mein do second lag gaye. Wajah kya kya ho sakti hai?

**Kabir:** Server dheema hoga.

**Madhav:** Aur?

**Kabir:** Internet dheema hoga.

**Madhav:** Aur?

**Kabir:** Bas.

**Madhav:** Chalo poore raaste pe chalte hain aur har jagah waqt naapte hain. Pehla kadam kya hai?

**Kabir:** Naam se pata nikalna. DNS.

**Madhav:** Kitna?

**Kabir:** Agar cache mein hai toh kuch nahi. Nahi toh shayad 50 millisecond.

**Madhav:** Phir?

**Kabir:** Server se judna. Aur taala lagana.

**Madhav:** Taala lagane mein kitne chakkar lagte hain?

**Kabir:** Kuch. Har chakkar mein aane-jaane ka waqt.

**Madhav:** Agar server doosre mahadweep mein hai toh ek chakkar lagbhag 150 millisecond ka hai. Teen chakkar?

**Kabir:** 450 millisecond. Aur abhi tak kuch maanga bhi nahi.

**Madhav:** Phir sawal jaata hai aur server sochta hai. Server kya karta hai?

**Kabir:** Database se poochta hai.

**Madhav:** Ek baar?

**Kabir:** Shayad kai baar. Pehle user, phir uske messages, phir har message ka bhejne wala.

**Madhav:** Agar sau messages hain aur har ek ke liye alag sawal?

**Kabir:** Sau sawal. Har ek mein thoda waqt.

**Madhav:** Har sawal 2 millisecond ka bhi ho toh?

**Kabir:** 200 millisecond, sirf yahan.

**Madhav:** Ab jawab wapas aata hai. Phir?

**Kabir:** Phone use dikhata hai. Photo utarti hai.

**Madhav:** Ab ginti karo. Kitne alag hisse the?

**Kabir:** Paanch chhe. Aur har ek mein sau-do sau millisecond.

**Madhav:** Ab batao, aapka pehla jawab kaisa tha? "Server dheema hoga."

**Kabir:** Woh sirf ek hissa tha. Aur shayad sabse chhota.

**Madhav:** Ab aakhri sawal. In sab mein kaunsa hissa aap sudhaar sakte ho, aur kaunsa nahi?

**Kabir:** Server ka hisaab sudhaar sakta hoon. Database ke sau sawal ek mein badal sakta hoon.

**Madhav:** Aur doosre mahadweep tak jaane ka waqt?

**Kabir:** Woh nahi badal sakta. Woh roshni ki speed hai.

**Madhav:** Toh kya karoge?

**Kabir:** Server paas le aaunga. Ya kam chakkar lagaunga.

---

### Naam

Kul waqt ka ek naam hai, aur uske hisse ginne ka bhi:

```
DNS              naam se pata               0 se 100 ms
JUDNA + TAALA    kuch chakkar               1 se 3 chakkar
SAWAL JAANA      ek chakkar                 doori pe nirbhar
SERVER SOCHNA    hisaab + database          aksar sabse bada
JAWAB AANA       ek chakkar                 doori pe nirbhar
DIKHANA          phone ka kaam              10 se 500 ms
```

Aur do cheezein jo alag hain aur log unhe mila dete hain, Chapter 4.3 se:

```
BANDWIDTH   sadak kitni chaudi   →  badhayi ja sakti hai
LATENCY     sadak kitni lambi    →  badhayi nahi ja sakti
```

Latency ki ek sakht seema hai: roshni. Ek chakkar Mumbai se New York lagbhag 150 millisecond ka hai, aur duniya ka koi paisa use kam nahi kar sakta.

Isliye speed ke do bilkul alag ilaaj hain:

```
KAAM KAM KARO    behtar hisaab, kam database sawal, cache

CHAKKAR KAM KARO ya doori kam karo
                 (aur yeh aksar zyada bada faayda deta hai)
```

Aur woh sabse aam galti jo har jagah milti hai, uska ek naam hai: **N+1**.

Ek sawal se sau cheezein aayin, aur phir har cheez ke liye ek alag sawal. Ek ki jagah ek sau ek sawal. Har ek chhota hai, aur unka jod bahut bada hai.

Ilaaj lagbhag hamesha wahi hai: **sau chhote sawal ek bade sawal mein badal do.**

---

### Asli duniya se ek example

Google ne apne experiments mein paya ki search ke nateeje 400 millisecond der se dikhane par log kam search karte the. Amazon ne bhi isi tarah dekha ki 100 millisecond ki der bikri par asar dalti thi.

Yeh numbers baar baar quote kiye jaate hain aur unka asli matlab yeh hai: **log der ko sochte nahi, mehsoos karte hain.**

Koi user yeh nahi kehta ki "yeh 400 millisecond dheema hai." Woh bas thoda kam istemaal karta hai, thoda jaldi chhod deta hai, aur use khud pata nahi hota ki kyun.

Isiliye speed ek feature hai, ek technical baat nahi. Aur isiliye badi companies apne server duniya bhar mein rakhti hain, sirf latency ke liye.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **badi machine se dheemi cheez theek karne ki koshish.**

Agar aapka waqt safar mein ja raha hai, toh do guna tez CPU se lagbhag kuch nahi hoga. Server pehle hi khaali baitha intezaar kar raha tha.

Doosri galti: **average dekhna.**

Maan lo aapka average 200 millisecond hai. Sunne mein achha hai. Lekin ho sakta hai ki 90 pratishat logon ko 50 millisecond mile aur 10 pratishat ko 3 second.

Woh 10 pratishat aksar aapke sabse zyada istemaal karne wale log hote hain, kyunki unka data sabse zyada hai.

Isliye ache systems mein average nahi dekha jaata. Woh dekha jaata hai jise "sabse bure 5 pratishat" kehte hain. **Average sabse bure anubhav ko chhupa deta hai, aur wahi anubhav log yaad rakhte hain.**

Teesri galti: yeh sochna ki dheemi cheez ek bug hai jo kabhi kabhi hoti hai. Aksar woh design hai jo har baar hoti hai, aur bas kisi ne naapi nahi.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  WAQT KE HISSE  DNS, judna, safar,      │  ← naya
    │                 sochna, dikhana         │
    │  N+1            sau chhote sawal        │  ← naya
    │  AVERAGE JHOOTH BOLTA HAI               │
    ├────────────────────────────────────────┤
    │  SHRINKHLA, CLOUD, API, UPTIME          │
    ├────────────────────────────────────────┤
    │  QUEUE, CACHE, DATABASE, INTERNET       │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Aapki site India mein banai gayi hai aur server bhi India mein hai. America se log kehte hain ki woh dheemi hai. Server ka hisaab tez karne se faayda hoga?

> **Jawab:** Bahut kam.
>
> Unka zyadatar waqt safar mein ja raha hai. Ek chakkar lagbhag 250 millisecond ka hai, aur judne mein kai chakkar lagte hain.
>
> Ilaaj doori kam karna hai: cheezein unke paas rakh do (CDN, Chapter 5.5), ya wahan bhi ek server rakh do.
>
> **Jab problem doori ki ho, toh hisaab tez karne se kuch nahi milta.**

**2. (samajh check)** Ek page 50 photos dikhata hai aur har photo alag se maangi jaati hai. Kya problem hai aur kya karoge?

> **Jawab:** Yeh N+1 ka doosra roop hai. 50 alag chakkar.
>
> Do ilaaj hain. Ek: sab ek saath maango, ek hi baar mein. Do: sirf woh photos maango jo abhi screen pe dikh rahi hain, baaki tab jab user neeche jaaye.
>
> Doosra tareeka aksar behtar hai, kyunki bahut se log neeche jaate hi nahi. **Sabse tez kaam woh hai jo aap karte hi nahi.**

**3. (jodne wala)** Chapter 2.3 kehta tha ki CPU tez hai aur data laana dheema. Kya wahi baat yahan bhi hai?

> **Jawab:** Bilkul wahi baat hai, sirf paimana badal gaya.
>
> ```
> ek machine ke andar   RAM se data laana   ~200 kadam
> ek building ke andar  doosri machine se   ~10 lakh kadam
> duniya ke us paar     doosre mahadweep se ~50 crore kadam
> ```
>
> Har baar hisaab sasta hai aur doori mehngi.
>
> Yeh iss kitaab ki sabse bade dohraav wali baat hai. Woh chip ke andar bhi sach hai, machine ke andar bhi, aur duniya ke paimane pe bhi. **Jo bhi banao, sabse pehle poocho ki data kahan se aa raha hai.**
