# Chapter 6.2  [SPINE]
## Woh machine jo kabhi band nahi hoti

---

### Samvaad

**Madhav:** Chapter 4.2 mein tay hua tha ki aapka phone bahar se pahuncha nahi ja sakta, isliye beech mein koi hota hai. Woh beech wali machine kaisi honi chahiye?

**Kabir:** Hamesha chalu.

**Madhav:** Kyun? Aapka phone toh raat ko band ho jaata hai.

**Kabir:** Kyunki mujhe nahi pata ki kaun kab message bhejega. Agar woh us waqt band hui toh message kahin nahi jaayega.

**Madhav:** Toh "hamesha chalu" ek zaroorat hai. Ab batao, hamesha chalu rehna kitna mushkil hai?

**Kabir:** Bijli chahiye, internet chahiye. Bas.

**Madhav:** Bijli chali gayi?

**Kabir:** Battery honi chahiye.

**Madhav:** Battery khatam?

**Kabir:** Generator.

**Madhav:** Machine kharaab ho gayi?

**Kabir:** Doosri machine honi chahiye.

**Madhav:** Software update karna hai?

**Kabir:** Hmm. Update karne ke liye band karna padega.

**Madhav:** Toh update ke liye site band?

**Kabir:** Nahi. Ek machine band karo, doosri chalti rahe. Phir doosri.

**Madhav:** Achha. Ab batao, aap "hamesha chalu" kitna pakka kar sakte ho? Sau pratishat?

**Kabir:** Shayad nahi.

**Madhav:** Kyun nahi?

**Kabir:** Kuch bhi ho sakta hai. Bhookamp. Poore ilaake ki bijli. Kisi ki bahut badi galti.

**Madhav:** Toh aap sirf yeh keh sakte ho ki kitna kam band rahega. Chalo ginti karte hain. Saal mein kitne ghante hote hain?

**Kabir:** Lagbhag 8,760.

**Madhav:** 99 pratishat chalu ka matlab kitna band?

**Kabir:** Ek pratishat. Lagbhag 88 ghante. Teen din se zyada.

**Madhav:** 99.9?

**Kabir:** Lagbhag 9 ghante.

**Madhav:** 99.99?

**Kabir:** Lagbhag 53 minute.

**Madhav:** 99.999?

**Kabir:** Paanch minute. Poore saal mein.

**Madhav:** Ab socho. Saal bhar mein paanch minute. Uska matlab hai ki koi insaan uthkar theek nahi kar sakta, kyunki uthne mein hi paanch minute lag jaayenge.

**Kabir:** Toh sab kuch apne aap theek hona chahiye.

**Madhav:** Aur uski keemat?

**Kabir:** Bahut zyada hogi. Har cheez ki do copy, aur unhe apne aap sambhalne wala system.

**Madhav:** Ab batao, har cheez ko 99.999 banana chahiye?

**Kabir:** Nahi. Sirf usko jiska band hona sach mein mehnga ho.

---

### Naam

Us "kitna chalu raha" ko **uptime** kehte hain, aur log use naukon mein ginte hain.

```
99%       ek saal mein  ~3.65 din band
99.9%                   ~8.8 ghante
99.99%                  ~53 minute
99.999%                 ~5 minute
```

Har naya nau daam ko lagbhag guna kar deta hai. 99.9 se 99.99 tak jaana aksar poore system ko dobara banana hota hai.

Aur woh cheez jiska matlab hai "band hone wali koi ek jagah na ho," use **no single point of failure** kehte hain. Yaani koi bhi ek cheez aisi na ho jiske marne se sab ruk jaaye.

Ek machine ko hamesha chalu rakhne ke liye kya kya do baar chahiye:

```
bijli          →  do alag laain, battery, generator
internet       →  do alag company
machine        →  kam se kam do, alag jagah
disk           →  kai, ek kharaab ho toh chalta rahe
building       →  do alag sheher (bade systems mein)
aadmi          →  koi hamesha uplabdh ho
```

Aur ab woh baat jo iss chapter ki asli seekh hai:

**"Hamesha chalu" ek naukri hai, koi feature nahi.**

Woh ek baar bana kar chhoda nahi ja sakta. Koi hamesha dekh raha hota hai. Koi raat ko phone uthata hai. Koi har update ko aise karta hai ki beech mein kuch na ruke.

Aur isiliye "server pe daal do" itna sasta nahi hota jitna log sochte hain. Machine ka kiraya chhota hissa hai. **Use hamesha chalu rakhna asli kharcha hai**, aur woh kharcha zyadatar aadmiyon ka hai, machinon ka nahi.

---

### Asli duniya se ek example

2021 mein ek badi cloud company ki ek service kuch ghanton ke liye baith gayi. Uske saath duniya bhar ki hazaaron websites, apps aur cheezein baith gayin, kyunki woh sab usi ke upar khadi thin.

Un hazaaron companies mein se har ek ne apne system ko mazboot banaya tha. Har ek ke paas kai machinein thin, backup the, sab kuch tha.

Lekin sabke neeche ek hi cheez thi.

Yeh us baat ka sabse saaf udaharan hai jo iss chapter mein hai: **aapka system utna hi mazboot hai jitni uski sabse kamzor neeche wali parat.** Aur woh parat aksar aapki nahi hoti, aur aapko yaad bhi nahi hota ki woh wahan hai.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki "cloud pe hai isliye hamesha chalu rahega."**

Cloud sirf kisi aur ki machinein hain. Woh bhi band hoti hain. Farak sirf yeh hai ki jab woh band hoti hain toh aapke saath hazaaron aur bhi band hote hain, aur aap kuch nahi kar sakte, sirf intezaar.

Doosri galti: yeh sochna ki zyada nau hamesha behtar hai.

99.99 ka matlab hai ki poore saal mein 53 minute se zyada band nahi. Uski keemat aksar poore system ko dobara banana hoti hai, aur log ko raat ko uthana hota hai.

Ek chhoti company ke liye 99.9 lagbhag hamesha kaafi hai. Woh saal mein 9 ghante hain, jo aksar update aur chhoti dikkaton mein hi chale jaate hain, aur kisi ko farak nahi padta.

Sahi sawal: **ek ghanta band rehne se kitna nuksaan hota hai?** Agar jawab "kuch khaas nahi" hai, toh naukon ke peeche bhagna sirf paisa jalana hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  UPTIME       naukon mein ginti         │  ← naya
    │               har nau daam guna karta   │
    │  KOI EK JAGAH aisi na ho jo sab rok de  │  ← naya
    ├────────────────────────────────────────┤
    │  BADA HONA, KHAALI MACHINE              │
    ├────────────────────────────────────────┤
    │  REPLICA, QUEUE, CACHE, DATABASE        │
    ├────────────────────────────────────────┤
    │  INTERNET, OS, CPU, RAM/DISK, SWITCH    │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek company kehti hai "hamara uptime 99.9% hai." Woh saal mein kitni der band reh sakti hai, aur kya woh achha hai?

> **Jawab:** Lagbhag 8.8 ghante saal mein, ya har mahine lagbhag 43 minute.
>
> Achha hai ya nahi, yeh iss baat pe hai ki band hone se kya jaata hai.
>
> Ek blog ke liye bahut achha. Ek shopping site ke liye theek. Ek bank ke card system ke liye bilkul nahi, kyunki 43 minute mein lakhon transaction fail ho jaayenge.
>
> **Naukon ka koi apna matlab nahi hai. Unka matlab band hone ki keemat se aata hai.**

**2. (samajh check)** Aap sab kuch do baar rakhte ho: do machinein, do database, do internet connection. Kya ab aap surakshit ho?

> **Jawab:** Un cheezon se, haan. Lekin do saval bache hain.
>
> **Ek:** kya dono ek hi building mein hain? Kya dono ek hi bijli pe hain? Kya dono ek hi cloud company pe hain?
>
> **Do:** kya woh doosri wali sach mein kaam karegi? Kabhi jaanchi hai?
>
> Yeh Chapter 5.7 wali baat hai: **jo bachaav jaancha nahi gaya, woh bachaav hai hi nahi.** Bahut se systems mein doosri machine saalon se maujood thi aur kabhi chali hi nahi thi.

**3. (jodne wala)** Chapter 6.1 kehta tha ki bojh hatta nahi, khiskta hai. Uptime ke saath kya wahi hota hai?

> **Jawab:** Haan, aur ek nayi shakal mein.
>
> Aap ek machine ko do bana dete ho, toh woh problem hat jaati hai. Ab problem us cheez pe chali jaati hai jo tay karti hai ki kaunsi machine chal rahi hai.
>
> Use do bana do, toh problem us cheez pe chali jaati hai jo un dono ke beech faisla karti hai.
>
> Har baar aap ek jagah ki kamzori hatate ho aur ek nayi jagah bana dete ho.
>
> Isiliye 100 pratishat kabhi mumkin nahi hota. **Har hal apne saath ek nayi, chhoti kamzori laata hai.** Aap use chhota kar sakte ho, khatam nahi.
