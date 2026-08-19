# Chapter 6.1  [SPINE]
## Ek user se hazaar user tak

---

### Samvaad

**Madhav:** Ek machine hai. Ek user aata hai, sawal poochta hai, jawab milta hai. Ek sawal mein sau millisecond lagte hain. Ek second mein kitne sawal sambhal sakti hai?

**Kabir:** Das.

**Madhav:** Ab sau log ek saath aa gaye. Kya hoga?

**Kabir:** Line lag jaayegi. Aakhri wale ko das second lagenge.

**Madhav:** Aur hazaar?

**Kabir:** Sau second. Log chale jaayenge.

**Madhav:** Toh kya karoge?

**Kabir:** Badi machine le lo.

**Madhav:** Achha. Do guna badi machine mili. Ab kitne?

**Kabir:** Bees per second.

**Madhav:** Chaar guna badi?

**Kabir:** Chalis.

**Madhav:** Ab sabse badi machine jo duniya mein milti hai. Uske baad?

**Kabir:** Uske baad kuch nahi.

**Madhav:** Toh ek deewar hai. Doosra raasta socho.

**Kabir:** Kai machinein lagao.

**Madhav:** Das machinein hain. User kis pe jaayega?

**Kabir:** Koi tay kare.

**Madhav:** Toh ek aur cheez chahiye jo saamne khadi ho aur baante.

**Kabir:** Haan.

**Madhav:** Ab woh khud kitne sambhal sakti hai?

**Kabir:** Woh bhi ek machine hai. Uski bhi seema hogi.

**Madhav:** Lekin uska kaam chhota hai. Woh sirf aage bhej rahi hai, sochna nahi pad raha. Toh woh ek lakh per second kar sakti hai jabki asli kaam wali sirf das.

**Kabir:** Toh theek hai.

**Madhav:** Ab ek problem. User pehle machine pe login karta hai. Agli baar woh teesri machine pe pahunchta hai. Kya hoga?

**Kabir:** Teesri ko pata hi nahi ki yeh kaun hai. Woh phir se login maangegi.

**Madhav:** Toh?

**Kabir:** Login ki jaankari machine mein nahi, kisi saanjhi jagah pe rakhni padegi.

**Madhav:** Kahan?

**Kabir:** Database mein. Ya kisi cache mein jo sabke liye ek ho.

**Madhav:** Bas. Aur ab yeh niyam ban jaata hai: machine ke andar kuch bhi aisa mat rakho jo sirf usi ke paas ho. Kyunki agli baar user kahin aur jaayega.

**Kabir:** Toh machinein khaali honi chahiye.

**Madhav:** Aur agar woh khaali hain, toh ek machine mar jaaye toh?

**Kabir:** Kuch nahi hoga. Baaki sambhal lengi.

**Madhav:** Aur agar aur log aa jaayein?

**Kabir:** Aur machinein jod do.

**Madhav:** Ab ek aakhri sawal. Das machinein hain, sab khaali. Sab kis cheez se data leti hain?

**Kabir:** Ek database se.

**Madhav:** Toh ab problem kahan chali gayi?

**Kabir:** Database pe. Ab woh sabka bojh utha raha hai.

**Madhav:** Bas. Tumne abhi wahi cheez dhoondh li jo har badhne wale system mein hoti hai. Aap bojh hatate nahi ho. Aap use khiska dete ho.

---

### Naam

Do tareeke bade hone ke:

```
UPAR JAANA (scale up)
├── ek machine ko bada karo
├── aasan: kuch nahi badalna padta
├── mehnga: bade machine ka daam tez badhta hai
└── ek deewar hai: sabse badi machine ke baad kuch nahi

BAGAL MEIN FAILNA (scale out)
├── kai chhoti machinein
├── sasta: chhoti machinein sasti hoti hain
├── koi deewar nahi: aur jodte jao
└── mushkil: ab sab kuch alag tareeke se banana padta hai
```

Woh saamne khadi cheez jo baantti hai, use **load balancer** kehte hain.

Aur woh niyam jo Kabir ne nikaala, woh sabse zaroori hai:

**Har machine khaali honi chahiye.** Yaani usmein aisi koi jaankari na ho jo sirf usi ke paas hai. Kyunki agli baar user kisi aur machine pe pahunchega.

Aisi machine ko **stateless** kehte hain, aur uske teen bade faayde hain:

```
ek machine mar jaaye  →  kisi ko farak nahi padta
bojh badhe            →  aur machinein jod do
kaam kam ho           →  machinein hata do
```

Aur ab woh baat jo iss poore Part ka dhaancha hai:

**Bojh hatta nahi hai. Woh khiskta hai.**

Aap web machinein badha lete ho, toh bojh database pe chala jaata hai. Database ko badha lete ho, toh bojh kisi ek table pe chala jaata hai. Usko baant do, toh bojh us jagah pe chala jaata hai jahan sab milte hain.

Har baar aapko naya sabse patla hissa dhoondhna padta hai. Kaam kabhi khatam nahi hota, sirf jagah badalti hai.

---

### Asli duniya se ek example

Twitter ke shuruaati saalon mein ek nishaan mashhoor ho gaya tha: ek whale ko chidiyan utha rahi hain. Woh tab dikhta tha jab site bojh se baith jaati thi, aur 2007 se 2009 tak woh bahut dikhta tha.

Unki shuruaati banawat ek hi bade database pe khadi thi. Jab tak users kam the, theek chala. Jab woh tez badhne lage, toh woh ek database sabse patla hissa ban gaya.

Unhe kai saal aur poori banawat badalni padi. Yeh naye code se nahi hua, banawat ke naye faisle se hua.

Aur yeh kahani lagbhag har badhne wale product mein dohrayi jaati hai. **Jo banawat sau users pe sahi hai, woh das lakh pe galat hoti hai. Aur woh galat isliye nahi hoti ki koi galti hui thi. Woh us waqt sahi thi.**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **pehle din se bade paimane ke liye banana.**

Log shuruaat mein hi woh sab lagate hain jo das lakh users ke liye chahiye: das machinein, load balancer, sab kuch baanta hua.

Uski keemat teen tarah se chukani padti hai: banane mein zyada waqt, chalane mein zyada kharcha, aur galti dhoondhna bahut mushkil, kyunki ab cheez kai jagah bikhri hai.

Aur zyadatar products kabhi das lakh users tak pahunchte hi nahi. Toh woh saari mehnat ek aisi problem ke liye thi jo kabhi aayi hi nahi.

Yeh galti templing isliye hai ki bade companies ke tareeke likhe hue milte hain aur woh samajhdaar lagte hain. Log woh tareeke uthate hain lekin unki wajah nahi uthate.

Sahi soch:

```
ab jo hai uske liye banao
lekin aisi cheezein mat karo jo aage badalna namumkin kar dein
```

Aur unmein sabse badi cheez wahi hai jo iss chapter mein aayi: machine ko khaali rakho. Woh aaj lagbhag kuch nahi maangta, aur kal sab kuch aasan kar deta hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  BADA HONA    upar jaana, ya bagal      │  ← naya
    │  KHAALI MACHINE   jaankari machine mein │  ← naya
    │                   nahi, saanjhi jagah pe│
    │  BOJH KHISKTA HAI, hatta nahi           │
    ├────────────────────────────────────────┤
    │  REPLICA, QUEUE, CACHE, DATABASE        │
    ├────────────────────────────────────────┤
    │  INTERNET, OS, CPU, RAM/DISK, SWITCH    │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Aapne das machinein lagayin aur site phir bhi dheemi hai. Kahan dekhoge?

> **Jawab:** Us jagah jahan sab dus milti hain. Aksar database.
>
> Das machinein sirf apna hissa baant rahi hain. Agar sabko ek hi jagah se data laana hai, toh woh jagah ab das guna bojh utha rahi hai.
>
> Yeh iss chapter ka poora nichod hai: **jab aap ek jagah ka bojh baantte ho, toh woh agli jagah pe chala jaata hai.** Har baar naya sabse patla hissa dhoondhna padta hai.

**2. (samajh check)** Ek machine user ka login apne andar rakh leti hai kyunki woh tez hai. Kya problem hai?

> **Jawab:** Agli baar user kisi doosri machine pe ja sakta hai, aur usko kuch pata nahi hoga.
>
> Aur agar woh machine mar jaaye toh us par ke saare users ka login gaya.
>
> Aur aap us machine ko hata nahi sakte, kyunki usmein kuch aisa hai jo sirf usi ke paas hai.
>
> Ek chhoti si "speed ki chaal" ne teen aazadiyan cheen li: machine marne ki, hatane ki, aur nayi jodne ki.

**3. (jodne wala)** Chapter 3.4 mein OS ek manager tha jo baari baantta tha. Load balancer usse kaise alag hai aur kaise ek jaisa?

> **Jawab:** Ek jaisa: dono baantte hain jab ek cheez hai aur maangne wale kai.
>
> Alag: OS ek machine ke andar baantta hai, aur uske paas poori taakat hai. Load balancer machinon ke beech baantta hai, aur uske paas koi taakat nahi hai. Woh sirf aage bhejta hai.
>
> Aur yeh farak mayne rakhta hai. OS ek program ko rok sakta hai. Load balancer ek machine ko nahi rok sakta, woh sirf usse door ja sakta hai.
>
> **Jitna aap failte ho, utni aapki taakat kam hoti jaati hai.** Yeh Part 6 mein baar baar dikhega.
