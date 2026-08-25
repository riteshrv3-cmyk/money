# Chapter 5.7  [SPINE]
## Data kho jaaye toh kya

---

### Samvaad

**Madhav:** Saara data ek disk pe hai. Woh disk kharaab ho jaati hai. Kya gaya?

**Kabir:** Sab kuch.

**Madhav:** Kya karoge?

**Kabir:** Copy rakhunga. Doosri disk pe.

**Madhav:** Kab copy karoge?

**Kabir:** Roz raat ko.

**Madhav:** Disk dopahar do baje kharaab hui. Kya gaya?

**Kabir:** Raat se dopahar tak ka sab kaam.

**Madhav:** Toh?

**Kabir:** Zyada baar copy karo. Har ghante.

**Madhav:** Toh ek ghanta jaayega. Aur agar ek second bhi na jaana chahiye?

**Kabir:** Toh har likhne ke saath hi doosri jagah bhi likhna padega.

**Madhav:** Ab woh dheema ho jaayega. Har kaam do jagah.

**Kabir:** Haan.

**Madhav:** Toh sauda kya hai?

**Kabir:** Jitna kam data khone ko taiyaar hoon, utna dheema aur mehnga.

**Madhav:** Ab ek doosri problem. Tumne copy bana li, usi kamre mein. Kamre mein aag lag gayi.

**Kabir:** Dono gaye. Copy door rakhni chahiye.

**Madhav:** Kitni door?

**Kabir:** Doosre sheher mein.

**Madhav:** Ab har likhne ke saath doosre sheher likhoge? Chapter 4.3 yaad karo.

**Kabir:** Latency. Har likhne mein safar ka waqt jud jaayega.

**Madhav:** Toh phir?

**Kabir:** Paas wali copy turant, door wali thodi der baad.

**Madhav:** Aur agar bade hadse mein paas wali dono chali jaayein?

**Kabir:** Toh door wali se thoda data kam milega.

**Madhav:** Bas. Ab teesri problem, aur yeh sabse tedhi hai. Tumne copy bana li, sab theek hai. Ab galti se ek command chal gayi jisne saara data mita diya.

**Kabir:** Copy se wapas le lunga.

**Madhav:** Copy turant banti hai, har likhne ke saath. Toh copy mein kya hai?

**Kabir:** Copy mein bhi mit gaya hoga.

**Madhav:** Kyunki copy ne kya kiya?

**Kabir:** Usne wahi kiya jo asli ne kiya. Woh galti bhi copy ho gayi.

**Madhav:** Toh copy kis cheez se bachati hai aur kis se nahi?

**Kabir:** Machine kharaab hone se bachati hai. Galti se nahi bachati.

**Madhav:** Toh galti se kya bachayega?

**Kabir:** Purana data. Kal ka, jo galti se pehle ka hai.

**Madhav:** Toh ab tumhare paas do bilkul alag cheezein hain, aur log unhe hamesha mila dete hain.

---

### Naam

Do alag cheezein, do alag kaam:

```
REPLICA  (nakal)
├── har badlav turant doosri jagah bhi hota hai
├── machine kharaab ho toh doosri turant sambhal leti hai
├── galti se nahi bachati: galti bhi turant copy ho jaati hai
└── uska kaam hai: chalte rehna

BACKUP  (purani copy)
├── kisi purane waqt ki tasveer, alag rakhi hui
├── galti, virus, ya kisi ke jaan-boojh ke mitane se bachati hai
├── wapas laane mein waqt lagta hai
└── uska kaam hai: waqt mein peeche jaana
```

Aur do naap jo har jagah istemaal hote hain:

```
KITNA DATA KHO SAKTA HAI      copy kitni baar banti hai
KITNI DER BAND REH SAKTA HAI  wapas aane mein kitna lagta hai
```

Dono ko zero ke kareeb laana mumkin hai, aur bahut mehnga hai. Isliye har company yeh tay karti hai ki uske liye kitna theek hai. Ek bank ke liye lagbhag zero. Ek chhote blog ke liye ek din bhi chalega.

Aur ab woh baat jo iss chapter ki asli seekh hai, aur jise log sabse zyada bhoolte hain:

**Backup tab tak backup nahi hai jab tak aapne use wapas laakar dekha na ho.**

Backup lena aasan hai. Woh chup-chaap chalta rehta hai aur koi kabhi nahi dekhta. Aur woh chup-chaap kharaab bhi ho sakta hai, mahinon tak, aur kisi ko pata nahi chalta.

Pata us din chalta hai jab zaroorat padti hai. Aur woh sabse bura din hota hai yeh pata karne ke liye.

---

### Asli duniya se ek example

2017 mein GitLab naam ki company mein ek engineer ne raat ko, thaka hua, ek command chalayi. Woh galat server pe chal gayi. Lagbhag 300 GB ka asli data mit gaya.

Unke paas paanch alag tarah ke bachaav the.

Unmein se chaar us waqt kaam nahi kar rahe the. Kuch chup-chaap band ho chuke the, kuch se banti hui files khaali thin, kuch kabhi jaanche hi nahi gaye the.

Paanchva ek chhe ghante purana snapshot tha, jo kisi ne kisi aur kaam ke liye banaya tha. Usi se woh bache. Chhe ghante ka data phir bhi gaya.

Sabse dhyaan dene wali baat: unhone poori ghatna sabke saamne likhi, live. Aur usse yeh saaf hua ki unke paas bachaav ki kami nahi thi. **Unke paas paanch bachaav the aur unmein se kisi ki jaanch nahi hoti thi.**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **replica ko backup samajhna.**

"Mera data cloud pe hai, do jagah copy hai, toh surakshit hai."

Woh machine kharaab hone se surakshit hai. Woh aapki apni galti se bilkul surakshit nahi hai.

Agar aap galti se ek folder delete karo, toh woh dono jagah se delete hoga. Turant. Kyunki replica ka poora kaam hi yeh hai ki wahi kare jo asli ne kiya.

Iska seedha nateeja: log apni photos "cloud pe hain" samajh kar nishchint rehte hain, aur ek din galti se delete karke unhe pata chalta hai ki cloud ne woh galti bhi wafadari se copy kar di.

Isiliye achhe systems delete ko turant nahi karte. Woh use kuch din ke liye ek kone mein rakhte hain. Woh ek chhota sa backup hai, jaan-boojh ke banaya gaya, aapki apni galti ke liye.

Sahi soch:

```
machine kharaab      →  replica bachayega
building mein aag    →  door wala replica bachayega
aapki galti          →  sirf backup bachayega
virus / hamla        →  sirf purana backup bachayega
```

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  REPLICA      chalte rehna              │  ← naya
    │  BACKUP       waqt mein peeche jaana    │  ← naya
    │               (jaanchi na ho toh backup │
    │                hai hi nahi)             │
    ├────────────────────────────────────────┤
    │  QUEUE, CACHE, TRANSACTION, INDEX       │
    ├────────────────────────────────────────┤
    │  INTERNET, OS, CPU, RAM/DISK, SWITCH    │
    └────────────────────────────────────────┘

    Part 5 khatam.
```

---

### Part 5 ka gate

**1.** Ek app das hazaar users pe theek chal raha tha, das lakh pe dheema ho gaya. Code wahi hai. Kya hua? *(nahi aaya toh 5.2)*

> **Jawab:** Kahin poori list padhi ja rahi hai. Woh kaam data ke saath seedha badhta hai.
>
> Das hazaar pe woh dikha nahi. Das lakh pe woh saamne aa gaya. Ilaaj index hai, badi machine nahi.

**2.** Aapka data do jagah copy hota hai, turant. Aap galti se ek table delete kar dete ho. Bach jaaoge? *(nahi aaya toh 5.7)*

> **Jawab:** Nahi. Replica ne woh delete bhi turant copy kar diya.
>
> Aapko purana backup chahiye, jo galti se pehle ka ho.

**3.** Ek app "order confirmed" turant dikhata hai lekin das minute baad cancel ka message aata hai. Yeh bug hai? *(nahi aaya toh 5.6)*

> **Jawab:** Nahi, yeh design hai. "Confirmed" ka matlab tha ki order pakka likh liya gaya. Baaki sab queue mein tha.
>
> Company ne jaan-boojh ke thodi gadbad chuni, taaki intezaar na ho.

---

### Chat app pe wapas

```
Aapka message ek database mein jaata hai, file mein nahi,
kyunki chaar problem hain: dhoondhna, ek saath likhna,
beech mein rukna, aur dohrav.

Use dhoondhne ke liye index hai, warna das crore mein se ek
nikaalne mein paanch crore kadam lagte.

Bhejna ek transaction hai: message likha bhi jaaye aur
"bheja gaya" bhi lage, ya dono mein se kuch bhi nahi.

Notification queue mein jaati hai, isliye aapko "sent" turant
dikhta hai jabki doosre ke phone tak pahunchne mein waqt lagta hai.

Aapki purani chat cache mein hai, isliye scroll karna tez hai.

Aur woh sab do jagah copy hai, taaki machine kharaab ho toh
chalta rahe. Lekin agar aap khud chat delete kar do, toh woh
dono jagah se delete ho jaayegi.
```

Ab ek sawal jo abhi tak khula hai:

**Yeh sab ek machine pe chal raha tha. Ab ek crore log ek saath aa jaayein toh?** Yeh Part 6 hai.
