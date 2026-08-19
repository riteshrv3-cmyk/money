# Chapter 5.4  [DEPTH]
## Jab do log ek hi waqt likhein

---

*DEPTH chapter. Yeh woh problem hai jiski wajah se bank ka software itna mehnga hota hai, aur jiski wajah se ticket "sold out" hone ke baad bhi bik jaata hai.*

---

### Samvaad

**Madhav:** Ek bank ka khaata hai. Usmein hazaar rupaye hain. Do jagah se ek saath sau nikaale jaate hain. Kya hona chahiye?

**Kabir:** Aath sau bachne chahiye.

**Madhav:** Ab dekho ki machine kya karti hai. Nikaalne ka kaam teen kadam ka hai. Padho ki kitne hain. Ghatao. Wapas likho. Ab do log ek saath karein toh?

**Kabir:** Dono hazaar padhenge. Dono nau sau likhenge.

**Madhav:** Aur khaate mein?

**Kabir:** Nau sau. Do sau nikle aur sirf sau kate.

**Madhav:** Bank ne sau rupaye kho diye. Ab yeh ek din mein lakh baar hota hai. Kya karoge?

**Kabir:** Ek waqt mein sirf ek ko karne do.

**Madhav:** Kaise rokoge doosre ko?

**Kabir:** Taala laga do. Jab tak pehla khatam na ho, doosra intezaar kare.

**Madhav:** Theek. Ab ek naya kaam. Paise ek khaate se doosre mein bhejne hain. Kitne kadam?

**Kabir:** Ek se kam karo, doosre mein jodo. Do kadam.

**Madhav:** Pehla kadam ho gaya aur beech mein bijli chali gayi.

**Kabir:** Toh paise ek se kat gaye aur doosre mein aaye hi nahi. Gayab.

**Madhav:** Toh kya chahiye?

**Kabir:** Ya toh dono kadam hon, ya ek bhi na ho.

**Madhav:** Kaise?

**Kabir:** Pehle likh do kahin ki main yeh dono karne wala hoon. Phir karo. Beech mein ruk jaaye toh baad mein woh likha hua dekh kar tay kar lo.

**Madhav:** Kya tay karoge, poora karoge ya wapas karoge?

**Kabir:** Agar "main karne wala hoon" likha tha lekin "ho gaya" nahi likha, toh wapas kar do. Jaise kuch hua hi nahi.

**Madhav:** Tumne abhi database ka sabse zaroori hissa bana diya. Ab aakhri problem, aur yeh sabse tedhi hai. Do khaate hain. Ek aadmi A se B mein bhej raha hai. Doosra B se A mein. Dono ne apne pehle khaate pe taala laga liya.

**Kabir:** Ab pehla B ka taala maangega, jo doosre ke paas hai. Aur doosra A ka maangega, jo pehle ke paas hai.

**Madhav:** Aur?

**Kabir:** Dono intezaar karenge. Hamesha ke liye.

**Madhav:** Kya karoge?

**Kabir:** Kuch der baad ek ko chhod dena chahiye. Aur dobara koshish kare.

**Madhav:** Kaun chhodega? Dono ko lagta hai woh sahi hai.

**Kabir:** Koi niyam bana do. Jaise jo baad mein aaya woh chhode.

**Madhav:** Ya sabse aasan: taale hamesha ek hi order mein lo, chahe kaam kuch bhi ho. Toh do log kabhi ulte order mein phansenge hi nahi.

---

### Naam

Us "ya toh sab, ya kuch bhi nahi" wale ek kaam ko **transaction** kehte hain.

Woh chaar guarantee jo ek achha database deta hai:

```
SAB YA KUCH NAHI   aadha kaam kabhi nahi bachta
                   (yahi Kabir ne banaya)

NIYAM TOOTE NAHI   jo shartein tay hain woh har haal mein sach rahein
                   (khaata negative na ho, wagairah)

EK DOOSRE SE ALAG  do kaam ek saath chalein toh aise dikhein
                   jaise baari baari hue hon

PAKKA HO JAAYE     "ho gaya" kaha toh bijli jaane pe bhi bacha rahe
```

Aur woh do problem jo iske saath aati hain:

```
TAALA          ek waqt mein ek. Surakshit, lekin dheema.
               Jitne zyada taale, utna zyada intezaar.

DONO ATAK JAANA do kaam ek doosre ka taala maang rahe hain
               Hal: hamesha ek hi order mein taale lo,
               ya kuch der baad ek ko chhod do
```

Aur ab woh baat jo iss chapter ki asli seekh hai:

**Yeh sab suraksha muft nahi hai. Uski keemat speed hai.**

Ek database jo yeh chaaron cheezein pakki karta hai, woh us database se dheema hoga jo nahi karta. Isiliye kuch systems jaan-boojh ke inmein se kuch chhod dete hain.

Ek bank kabhi nahi chhodta. Ek app jo yeh gin raha hai ki kitne logon ne like kiya, woh aaram se chhod sakta hai. Ek like idhar udhar ho jaaye toh kisi ka kuch nahi jaata.

**Sawal hamesha ek hi hai: galti ki keemat kya hai?**

---

### Asli duniya se ek example

Concert ke ticket bikne pe ek jaani-pehchani ghatna hoti hai. Site kehti hai ki 100 ticket bache hain. Hazaaron log ek saath click karte hain. Kuch logon ko ticket mil jaata hai aur baad mein cancel ho jaata hai.

Wajah lagbhag hamesha wahi hai jo iss chapter mein hai. Ginti padhi gayi, ghatai gayi, wapas likhi gayi, aur beech mein koi aur bhi wahi kar raha tha.

Sahi hal taala hai. Lekin taala matlab ek waqt mein ek aadmi, aur hazaaron log line mein.

Toh companies aksar beech ka raasta chunti hain: ticket ko kuch minute ke liye rok do, poora taala mat lagao, aur agar ginti galat ho jaaye toh baad mein maafi maang lo.

Yeh galti nahi hai. Yeh ek chunav hai: **thodi galti, ya bahut intezaar.** Aur woh chunav technical nahi, karobaari hai.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki "database istemaal kar liya, ab sab surakshit hai."**

Database yeh guarantee tab deta hai jab aap use sahi tareeke se maango. Agar aapne apna kaam ek transaction mein nahi rakha, toh database aapko kuch nahi bachayega. Woh aapke teen alag kaam ko teen alag kaam hi samjhega.

Aur doosri galti: yeh sochna ki yeh problem sirf paise wale systems mein hoti hai. Kahin bhi jahan do log ek hi cheez badalte hain, wahi problem hai. Ek hi document do log edit karein. Ek hi seat do log book karein. Ek hi saaman do log khareedein.

Yeh galti tempting isliye hai ki test karte waqt yeh kabhi nahi dikhta. Ek aadmi test karta hai, sab theek chalta hai. Problem sirf tab aati hai jab bahut log ek saath aayein, yaani tab jab aap kaamyab ho jaate ho.

**Yeh kaamyabi ke saath aane wali bug hai.** Woh sabse mehngi hoti hai kyunki woh sabse bure waqt pe aati hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  TRANSACTION  sab ya kuch nahi          │  ← naya
    │  TAALA        ek waqt mein ek, dheema   │  ← naya
    │  SAUDA        thodi galti ya intezaar   │
    ├────────────────────────────────────────┤
    │  SHAKAL, INDEX, DATABASE                │
    ├────────────────────────────────────────┤
    │  INTERNET, OS, CPU, RAM/DISK, SWITCH    │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek app mein like ki ginti hai. Do log ek saath like karte hain aur ginti sirf ek badhti hai. Kya yeh theek karna chahiye?

> **Jawab:** Shayad nahi.
>
> Poocho: galti ki keemat kya hai? Ek like ki ginti ek kam. Kisi ka kuch nahi gaya.
>
> Aur theek karne ki keemat? Har like pe taala, yaani har like pe intezaar, us cheez ke liye jo second mein hazaaron baar hoti hai.
>
> Isliye aise systems aksar ginti ko thoda galat rehne dete hain aur baad mein sudhaar lete hain.
>
> Wahi baat bank ke khaate pe laagu karo aur jawab bilkul ulta ho jaata hai. **Technology wahi hai, faisla alag hai, kyunki galti ki keemat alag hai.**

**2. (samajh check)** Do kaam ek doosre ka taala maang kar atak gaye. Aapne niyam banaya ki jo baad mein aaya woh chhod dega. Kya yeh poori tarah hal hai?

> **Jawab:** Nahi, aur yeh dhyaan dene laayak hai.
>
> Agar dono baar baar wahi koshish karein toh woh phir se takra sakte hain, baar baar.
>
> Isliye asli systems mein chhodne ke baad thoda **alag-alag** intezaar kiya jaata hai, taaki dono ek saath wapas na aayein.
>
> Aur behtar hal wahi hai jo Madhav ne kaha: taale hamesha ek hi order mein lo. Tab woh haalat ban hi nahi sakti. **Problem ko hal karne se behtar hai use hone hi na dena.**

**3. (jodne wala)** Chapter 5.2 kehta tha ki index padhna tez karta hai aur likhna dheema. Yeh chapter kehta hai ki taala surakshit karta hai aur dheema. Inmein kya saanjha hai?

> **Jawab:** Dono ek hi shakal ke saude hain, aur poori kitaab unse bhari hui hai.
>
> ```
> index      →  padhna tez     |  likhna dheema
> taala      →  sahi           |  dheema
> cache      →  tez            |  purana ho sakta hai
> compression→  chhota         |  kholne mein kaam
> dabba      →  aazadi         |  galti aasan
> table      →  sakhti         |  badalna mushkil
> ```
>
> Ek bhi jagah aisi nahi hai jahan kuch muft mila ho.
>
> Yeh iss kitaab ki sabse kaam ki aadat hai: **jab bhi koi cheez kuch deti dikhe, poocho ki woh badle mein kya le rahi hai.** Jawab hamesha hota hai. Agar nahi dikh raha, toh aapne dhoondha nahi hai.
