# Chapter 7.2  [SPINE]
## Galti pehle dhoondhna

---

### Samvaad

**Madhav:** Pichhle chapter mein tay hua ki poora jaanchna namumkin hai. Toh phir jaanchne ka faayda kya?

**Kabir:** Kuch galtiyan toh milengi.

**Madhav:** Kaunsi? Woh jo aapne socheen, ya woh jo aapne nahi socheen?

**Kabir:** Jo maine socheen.

**Madhav:** Aur bug aksar wahan hote hain jo aapne nahi socha. Toh phir?

**Kabir:** Toh jaanch bekaar hai?

**Madhav:** Ulta socho. Aapne ek galti dhoondi aur theek ki. Kal aap kuch aur badalte ho aur wahi galti wapas aa jaati hai. Kya hoga?

**Kabir:** Mujhe dobara dhoondhni padegi.

**Madhav:** Aur agar aapne uski jaanch likh kar rakh di hoti?

**Kabir:** Toh woh turant pakad leti.

**Madhav:** Toh jaanch ka asli kaam kya hai?

**Kabir:** Nayi galtiyan dhoondhna nahi. Purani galtiyan wapas aane se rokna.

**Madhav:** Bas. Yeh sabse zaroori baat hai aur lagbhag sab log ise ulta samajhte hain. Ab agla sawal. Ek app mein hazaar jaanch likhi hain. Woh kab chalti hain?

**Kabir:** Jab main chalaun.

**Madhav:** Aur agar main bhool jaaun?

**Kabir:** Toh nahi chalengi.

**Madhav:** Toh?

**Kabir:** Apne aap chalni chahiye. Har badlav pe.

**Madhav:** Kaun chalayega?

**Kabir:** Koi machine, jo dekhti rahe ki kuch badla ya nahi.

**Madhav:** Aur agar koi jaanch fail ho?

**Kabir:** Toh woh badlav aage na jaaye.

**Madhav:** Ab teen tarah ki jaanch hoti hain. Ek: ek chhote hisse ko akele jaancho. Doosri: do hisson ko milakar. Teesri: poora system, jaise ek asli user chala raha ho. Kaunsi tez hai?

**Kabir:** Pehli. Woh sabse chhoti hai.

**Madhav:** Kaunsi sach ke sabse kareeb hai?

**Kabir:** Teesri. Woh asli istemaal jaisi hai.

**Madhav:** Toh sirf teesri kyun na likhein?

**Kabir:** Woh dheemi hogi. Aur agar fail ho toh pata nahi chalega ki kahan galti hai.

**Madhav:** Aur sirf pehli kyun na likhein?

**Kabir:** Toh har hissa alag se theek hoga aur milkar phir bhi toot sakta hai. Pichhla chapter.

**Madhav:** Toh?

**Kabir:** Teeno chahiye. Chhoti wali bahut saari, badi wali kam.

---

### Naam

Teen darje, aur unka aam anupaat:

```
CHHOTI JAANCH (unit)
├── ek chhota hissa, akela
├── bahut tez, second ke hisse mein hazaaron
├── fail ho toh turant pata ki kahan
└── sabse zyada, shayad 70%

JOD KI JAANCH (integration)
├── do ya teen hisse milkar
├── dheemi
├── woh galtiyan pakadti hai jo beech mein hoti hain
└── beech ki ginti, shayad 20%

POORI JAANCH (end to end)
├── asli user jaisa poora raasta
├── sabse dheemi, aur sabse zyada tootne wali
├── sach ke sabse kareeb
└── sabse kam, shayad 10%
```

Aur woh machine jo har badlav pe apne aap sab chalati hai, use **CI** kehte hain.

Ab woh do baatein jo iss chapter ka nichod hain.

**Ek: jaanch ka asli kaam bharosa hai, khoj nahi.**

Bina jaanch ke, har badlav ek daanv hai. Aap chhota badlav karne se bhi darte ho, kyunki pata nahi kya toot jaaye. Toh aap kam badalte ho, aur software dheere dheere jamm jaata hai.

Jaanch ke saath aap nirbhay ho kar badal sakte ho. **Jaanch aapko bug se nahi bachati. Woh aapko darr se bachati hai.**

**Do: jaanch ki bhi keemat hai.**

Har jaanch likhni padti hai, sambhalni padti hai, aur jab aap jaan-boojh ke kuch badalte ho toh use bhi badalna padta hai.

Isliye har cheez ki jaanch likhna bhi galat hai. Wahan likho jahan:

```
galti ki keemat zyada ho
woh hissa baar baar badalta ho
usmein pehle bhi galti nikal chuki ho
```

Aakhri wali sabse kaam ki hai: **jahan ek bug mila, wahan aur bhi honge.** Bug jhund mein rehte hain.

---

### Asli duniya se ek example

Knight Capital naam ki ek trading company ne 2012 mein 45 minute mein lagbhag 44 crore dollar kho diye.

Wajah yeh thi ki naya code aath machinon pe daalna tha aur ek machine chhoot gayi. Us ek machine pe purana code chalta raha, aur uska ek purana hissa naye code ke saath milkar galat kaam karne laga.

Yeh Chapter 7.1 wala teesra bug hai: naya sahi tha, purana sahi tha, aur woh saath mein galat the.

Aur ismein ek aur sabak hai jo agle do chapter ka vishay hai: galti code mein nahi thi. Galti **daalne ke tareeke** mein thi. Ek aadmi ne haath se aath machinon pe copy kiya aur ek chhoot gayi.

Company us hafte lagbhag khatam ho gayi.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki 100 pratishat jaanch ka matlab hai ki bug nahi honge.**

Ek maap hai jo batata hai ki jaanch ne code ki kitni lines chalayi. Log usse 100 pratishat karne mein lag jaate hain.

Lekin har line chal jaana aur har **haalat** ka jaancha jaana do alag baatein hain. Aap ek line ko chala sakte ho aur phir bhi us haalat ko na jaanchein jismein woh galat hoti hai.

Toh 100 pratishat ka matlab hai "har line ek baar chali," na ki "sab kuch sahi hai."

Doosri galti: **poori jaanch pe zyada bharosa karna.**

Poori jaanch sach ke kareeb hai lekin woh dheemi hai aur bina wajah bhi fail hoti rehti hai: network dheema tha, page thodi der se aaya, kuch aur badal gaya.

Aur jab jaanch bina wajah fail hone lagti hai, toh log use dekhna band kar dete hain. Aur us din se woh jaanch hai hi nahi.

**Ek jaanch jispe bharosa na ho, woh jaanch nahi hai.** Woh sirf shor hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  JAANCH       chhoti, jod, poori        │  ← naya
    │               kaam: darr hataana        │
    │  CI           har badlav pe apne aap    │  ← naya
    ├────────────────────────────────────────┤
    │  BUG, KHARCHA, API, UPTIME              │
    ├────────────────────────────────────────┤
    │  QUEUE, CACHE, DATABASE, INTERNET       │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek team kehti hai "hamare paas 5,000 jaanch hain" aur unka software phir bhi baar baar toot ta hai. Kya ho sakta hai?

> **Jawab:** Kai sambhavnayein, aur teeno aam hain.
>
> **Ek:** jaanch un jagahon pe hain jahan galti hoti hi nahi, aur jahan hoti hai wahan nahi hain.
>
> **Do:** sab chhoti jaanch hain aur jod ki koi nahi. Har hissa akela theek hai.
>
> **Teen:** jaanch fail hoti hai lekin log use nazarandaaz karte hain, kyunki woh bina wajah bhi fail hoti rehti hai.
>
> **Ginti kabhi jawab nahi hoti.** 5,000 jaanch ka matlab kuch nahi hai. Sawal yeh hai ki woh kahan hain aur unpe bharosa hai ya nahi.

**2. (samajh check)** Aapko ek chhota badlav karna hai lekin darr lag raha hai ki kuch toot jaayega. Iska kya matlab hai?

> **Jawab:** Ki wahan jaanch nahi hai, ya uspe bharosa nahi hai.
>
> Aur woh darr apne aap mein ek nuksaan hai, chahe kuch toote ya na toote. Kyunki us darr ki wajah se aap sudhaar nahi karte, safai nahi karte, aur software dheere dheere jamm jaata hai.
>
> Isiliye purane systems mein log kehte hain "isse haath mat lagao." Woh code kharaab nahi hota. Bas uske aas-paas koi jaal nahi hota, isliye koi kudne ki himmat nahi karta.

**3. (jodne wala)** Chapter 6.6 mein systems ek seema par jhatke mein girte the. Kya jaanch us tarah ki galti pakad sakti hai?

> **Jawab:** Aam jaanch bilkul nahi pakadti, aur yeh dhyaan dene laayak hai.
>
> Kyunki jaanch aksar ek user, ek sawal, ek waqt pe chalti hai. Aur woh galti tab dikhti hai jab hazaaron log ek saath aayein.
>
> Uske liye alag tarah ki jaanch hoti hai, jismein jaan-boojh ke bahut bojh daala jaata hai, aur dekha jaata hai ki cheez kahan girti hai.
>
> Aur ek aur tareeka hai jo bade systems istemaal karte hain: **jaan-boojh ke apni hi cheezein todna**, chalte hue system mein, taaki pata chale ki woh sach mein sambhal payegi ya nahi. Kyunki Chapter 5.7 wali baat yahan bhi lagti hai: **jo bachaav jaancha nahi gaya, woh bachaav hai hi nahi.**
