# Chapter 4.2  [SPINE]
## Har machine ko ek address

---

### Samvaad

**Madhav:** Tum ek chitthi bhejna chahte ho. Kya kya chahiye?

**Kabir:** Chitthi, aur pata.

**Madhav:** Pate mein kya hona chahiye?

**Kabir:** Aisa kuch jo duniya mein sirf ek jagah bataye.

**Madhav:** Aur agar do gharon ka ek hi pata ho?

**Kabir:** Toh chitthi galat jagah ja sakti hai.

**Madhav:** Toh pehla niyam: **ek pata, ek jagah.** Ab machines ke liye pata banao. Kaise banaoge?

**Kabir:** Har machine ko ek number de do.

**Madhav:** Kitne bade number?

**Kabir:** Jitni machinein hain.

**Madhav:** 1970 ke dashak mein jab yeh tay hua, tab duniya mein kuch sau computer the. Unhone chaar byte rakhe. Chaar byte se kitne pate?

**Kabir:** Chaar byte matlab battis bit. Do ko battis baar guna... lagbhag chaar arab.

**Madhav:** Us waqt chaar arab kaisa laga hoga?

**Kabir:** Bahut zyada. Kabhi khatam na hone wala.

**Madhav:** Aaj duniya mein kitne phone hain?

**Kabir:** Chaar arab se zyada. Aur laptop, server, TV, ghadi bhi.

**Madhav:** Toh?

**Kabir:** Pate khatam ho gaye.

**Madhav:** 2011 ke aas-paas hi lagbhag khatam ho gaye the. Ab batao kya karoge.

**Kabir:** Bade pate bana do.

**Madhav:** Bana diye gaye, 1998 mein hi. Solah byte wale. Unse itne pate bante hain ki zameen ke har ret ke kan ko bhi arbon pate mil jaayein.

**Kabir:** Toh problem hal ho gayi.

**Madhav:** Nahi hui. Aaj bhi duniya ka bada hissa purane pate hi istemaal karta hai.

**Kabir:** Kyun? Naye toh behtar hain.

**Madhav:** Yaad karo. Pichhle chapter mein tumne kya seekha tha ki behtar cheez ke saath kya hota hai?

**Kabir:** Jo pehle sab jagah pahunch gaya use hatana namumkin hai. Sabko ek saath badalna padega.

**Madhav:** Toh phir kaam kaise chal raha hai? Chaar arab pate hain aur bees arab cheezein judi hui hain.

**Kabir:** Kuch batwara ho raha hoga.

**Madhav:** Socho. Tumhare ghar mein kitni cheezein internet se judi hain?

**Kabir:** Do phone, ek laptop, TV.

**Madhav:** Aur ghar ka ek hi connection hai. Toh chaaron ke paas alag public pate hain ya ek?

**Kabir:** Shayad ek.

**Madhav:** Ek hi hai. Ghar ke andar sabke apne chhote pate hain, jo sirf ghar ke andar chalte hain. Bahar jaane wali har cheez ek hi pate se jaati hai, aur ek machine yaad rakhti hai ki kaunsa jawab kis andar wale ka hai.

**Kabir:** Toh yeh building ke flat jaisa hai. Building ka ek pata, andar flat number.

**Madhav:** Bilkul. Aur postman ko flat number nahi pata hota. Woh building tak laata hai, aur andar koi baant deta hai.

---

### Naam

Machine ke us pate ko **IP address** kehte hain.

Purane wale, chaar byte ke, **IPv4** hain. Woh aise dikhte hain: `142.250.183.14`. Chaar hisse, har ek 0 se 255 tak, kyunki har hissa ek byte hai.

Naye wale, solah byte ke, **IPv6** hain.

Aur woh ghar wali cheez, jo ek public pate ke peeche kai andar wale pate chhupa deti hai, use **NAT** kehte hain.

```
INTERNET
   │
   │  ek public pata: 103.21.58.7
   ▼
┌──────────────────────────────────┐
│  ghar ka router                  │
│  yaad rakhta hai kaunsa jawab    │
│  kiska hai                        │
└───┬──────┬──────┬──────┬─────────┘
    │      │      │      │
  phone  phone  laptop   TV
 192.168 192.168 192.168 192.168
   .1.2   .1.3   .1.4    .1.5
        (sirf ghar ke andar ke pate)
```

Ab ek baat jo iska seedha nateeja hai aur bahut kuch samjhati hai:

**Aapka phone bahar se pahuncha nahi ja sakta.** Woh bahar baat kar sakta hai, aur jawab wapas aa sakta hai. Lekin koi ajnabi aapke phone pe seedha chitthi nahi bhej sakta, kyunki uske paas jo pata hai woh building ka hai, flat ka nahi.

Isiliye har cheez ko ek beech wale server se hokar jaana padta hai. Aapka message doosre phone pe seedha nahi jaata. Woh pehle kisi aise machine tak jaata hai jiska apna pakka pata hai, aur woh use aage bhejti hai.

Yeh ek suraksha ki tarah bhi kaam karta hai aur ek majboori bhi hai. Aur yeh bahut bada karobaari nateeja rakhta hai: **beech mein hamesha koi baithta hai, aur jo beech mein baithta hai woh sab kuch dekhta hai.**

---

### Asli duniya se ek example

1981 mein IPv4 tay hua tha, chaar arab pate ke saath. Us waqt internet pe kuch sau machinein thin. Chaar arab kabhi khatam na hone wali sankhya lagti thi.

31 saal baad, 2011 mein, sabse upar wale bandware ne aakhri bade blocks baant diye. Pate khatam ho gaye.

IPv6, jo 1998 mein hi taiyaar tha, aaj 26 saal baad bhi duniya ke lagbhag aadhe traffic tak hi pahuncha hai.

Yeh soch ne laayak baat hai. Ek behtar cheez, poori tarah taiyaar, samasya saaf, aur phir bhi 26 saal mein aadhi duniya. Wajah technical nahi hai. Wajah yeh hai ki sabko ek saath badalna padta hai, aur kisi ek ke badalne ka koi faayda nahi hota.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki IP address aapki jagah batata hai.**

Filmon mein "IP trace kar liya, ghar ka pata mil gaya" dikhaya jaata hai. Asliyat kaafi alag hai.

IP address batata hai ki aap kis network se jude ho, na ki aap kahan ho. Woh aapke internet dene wali company ka pata hota hai, jo aksar aapke sheher ya usse bade ilaake tak hi pahunchata hai. Aur mobile pe woh poore rajya ka kuch bhi ho sakta hai.

Aur NAT ki wajah se ek hi pate ke peeche kai sau log ho sakte hain.

Yeh galti tempting isliye hai ki "address" shabd hi ghar ka pata sujhata hai. Woh ghar ka pata nahi hai. Woh **network mein jagah** hai, zameen pe jagah nahi.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  PATA         ek pata, ek jagah         │  ← naya
    │               public bahar, private andar│
    ├────────────────────────────────────────┤
    │  NETWORK      value judav mein hai      │
    ├────────────────────────────────────────┤
    │  OS, PROCESS, LANGUAGE                  │
    ├────────────────────────────────────────┤
    │  CPU, RAM/DISK, PROGRAM, SWITCH         │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Aapke ghar mein chaar cheezein internet se judi hain aur ek hi public pata hai. Do phone ek saath ek hi website kholte hain. Jawab sahi phone pe kaise pahunchta hai?

> **Jawab:** Router ek chhoti list rakhta hai.
>
> Jab pehla phone bahar bhejta hai, toh router likh leta hai: "yeh baat-cheet andar wale phone 192.168.1.2 ki hai." Doosre phone ke liye alag entry.
>
> Jawab aata hai toh router list dekh kar sahi phone ko de deta hai.
>
> Yeh Chapter 3.4 wali baat hai dobara: **jab ek cheez hai aur maangne wale kai, toh koi beech mein baith kar baantta hai, aur use yaad rakhna padta hai ki kaun kaun hai.**

**2. (samajh check)** IPv6 1998 se taiyaar hai aur behtar hai. 26 saal mein bhi poori duniya nahi aayi. Iss se aap kya seekhte ho?

> **Jawab:** Ki technology ki duniya mein behtar hona kaafi nahi hota.
>
> Badlav ki keemat sabko milkar chukani padti hai, lekin faayda tab tak kisi ko nahi milta jab tak sab na badlein. Toh har akela aadmi intezaar karna chunta hai.
>
> Yeh Chapter 4.1 ka network effect hai, ulti shakal mein: jo cheez sabko jodti hai, wahi sabko rok bhi leti hai.
>
> Aur yeh bahut aage tak jaata hai. Chapter 8.5 mein hum poochenge ki technology jeetati kyun hai, aur yeh un teen-chaar wajahon mein se ek hoga.

**3. (jodne wala)** Chapter 4.1 kehta tha ki value judav mein hai. Ab pata chala ki aapka phone bahar se pahuncha hi nahi ja sakta. Toh phir aapka phone judta kaise hai?

> **Jawab:** Kisi beech wale ke through.
>
> Aapka phone hamesha pehle bahar jaata hai, kisi aise server tak jiska pakka pata hai. Woh server aapke liye sandesh rakhta hai aur aage bhejta hai.
>
> Iska seedha nateeja: **do phone kabhi seedha baat nahi karte.** Beech mein hamesha koi hota hai.
>
> Aur jo beech mein hai, woh sab dekhta hai, sab rok sakta hai, aur sab band kar sakta hai. Yahan se do baatein nikalti hain jo aage aayengi: encryption kyun zaroori hai (Chapter 4.6), aur beech wali jagah itni keemti kyun hai (Part 6).
