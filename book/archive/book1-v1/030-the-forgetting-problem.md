# Chapter 5.1  [SPINE]
## Bhoolne ki problem

---

### Samvaad

**Madhav:** Server ne aapka message le liya. Ab use rakhna hai. Kahan rakhega?

**Kabir:** Disk pe. RAM mein rakhega toh bijli jaate hi gaya.

**Madhav:** Theek. Kis shakal mein?

**Kabir:** Ek file mein likh dega.

**Madhav:** Achha. Ek file, aur usmein har message ek line. Ab do sawal. Pehla: das crore message ke baad woh file kitni badi hogi?

**Kabir:** Bahut badi. Kuch GB.

**Madhav:** Aur agar usmein se ek khaas message dhoondhna ho?

**Kabir:** Poori file padhni padegi.

**Madhav:** Kitna waqt lagega?

**Kabir:** Chapter 2.3 ke hisaab se, disk dheemi hai. Kuch second, shayad zyada.

**Madhav:** Har sawal ke liye kuch second, aur ek second mein hazaaron sawal. Chalega?

**Kabir:** Nahi.

**Madhav:** Doosra sawal. Do log ek hi waqt pe us file mein likhte hain. Kya hoga?

**Kabir:** Dono ek hi jagah likh sakte hain. Ek doosre ke upar.

**Madhav:** Aur teesra. Likhte waqt bijli chali jaaye?

**Kabir:** Aadhi line likhi jaayegi. File kharaab.

**Madhav:** Toh ek simple file ke saath teen problem hain. Ginao.

**Kabir:** Dhoondhna dheema. Do log ek saath nahi likh sakte. Aur beech mein ruk jaaye toh sab kharaab.

**Madhav:** Ab ek chauthi bhi hai. Maan lo har message ke saath yeh bhi rakhna hai ki kisne bheja, kab bheja, kis group mein. Toh har line mein woh sab likhoge?

**Kabir:** Haan.

**Madhav:** Aur ek aadmi apna naam badal de? Uske purane das lakh message mein naam likha hai.

**Kabir:** Sab badalne padenge.

**Madhav:** Toh chauthi problem: ek hi cheez kai jagah likhi hai, aur badalne pe sab jagah badalni padti hai.

**Kabir:** Toh naam alag jagah rakh do. Message mein sirf ek number rakh do ki kaun tha.

**Madhav:** Ab tum sochne lage ho. Toh ab do file hain: ek logon ki, ek message ki. Aur message wali mein sirf ishara hai.

**Kabir:** Haan.

**Madhav:** Ab teen file, chaar file, das file. Aur unke beech ke ishare. Yeh sab kaun sambhalega?

**Kabir:** Mujhe khud likhna padega.

**Madhav:** Har app banane wale ko, har baar, shuru se?

**Kabir:** Nahi. Koi ek baar bana de, sab istemaal karein.

**Madhav:** Bas. Aur wahi hua.

---

### Naam

Woh alag program jo yeh saara kaam sambhalta hai, use **database** kehte hain.

Woh chaar problem jo Kabir ne khud nikaali, database unhi chaar ke liye maujood hai:

```
1. DHOONDHNA        das crore mein se ek, turant
2. EK SAATH LIKHNA  kai log ek waqt pe, bina ek doosre ko bigaade
3. BEECH MEIN RUKNA bijli jaaye toh aadha kaam na bache
4. DOHRAV           ek cheez ek jagah, baaki jagah sirf ishara
```

Aur database khud kuch nayi cheez nahi hai. Woh ek program hai jo disk pe files hi likhta hai. Bas usne yeh chaar problem itni baar hal ki hain ki ab koi dobara nahi karta.

Yeh Chapter 3.1 wali baat hai, phir se. Kisi ne ek baar takleef uthayi, aur uske baad kisi ko nahi uthani padi.

Aur ab woh cheez jo iss poore part ka aadhaar hai:

**Data ko rakhna aasan hai. Use wapas dhoondhna mushkil hai.**

Kuch bhi likh dena sasta hai. Das crore cheezon mein se ek nikalna, woh asli kaam hai. Poora Part 5 lagbhag isi ek sawal ke aas-paas hai.

---

### Asli duniya se ek example

1970 mein IBM ke ek researcher, Edgar Codd, ne ek paper likha jismein usne kaha ki data ko tables mein rakha jaaye, aur unke beech ke rishte numbers se banaye jaayein, na ki us baat se ki file mein kya kahan pada hai.

Us waqt log data ko is baat se dhoondhte the ki woh disk pe kis jagah pada hai. Yaani program ko pata hona padta tha ki cheez kahan rakhi hai.

Codd ne kaha ki program ko yeh nahi pata hona chahiye. Program bataye ki **kya** chahiye, aur database khud dekhe ki woh **kahan** hai.

Yeh Chapter 0.4 wala abstraction hai, data pe laga hua. Aur woh ek soch aaj bhi lagbhag har database ke andar chal rahi hai, pachas saal baad.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki database ek jaadui cheez hai jo files se alag hai.**

Log "database" sunkar kuch bahut alag sochte hain. Woh disk pe files hi hain. Aap unhe kholo toh andar numbers milenge.

Farak yeh nahi hai ki woh kis cheez pe likhta hai. Farak yeh hai ki woh un chaar problem ka hal apne andar rakhta hai.

Iska seedha nateeja: log poochte hain "database istemaal karun ya file?" Sahi sawal yeh hai: "kya mujhe un chaar problem mein se koi bhi hai?" Agar aapko sirf kuch settings rakhni hain, ek file kaafi hai. Agar das crore cheezein hain aur sau log ek saath likh rahe hain, toh nahi.

Yeh galti tempting isliye hai ki database ka naam bada hai aur woh alag cheez lagta hai. Neeche wahi disk hai jo Chapter 2.4 mein thi.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  DATABASE     dhoondhna, ek saath likhna│  ← naya
    │               beech mein rukna, dohrav  │
    ├────────────────────────────────────────┤
    │  INTERNET, PROTOCOL, PATA, NETWORK      │
    ├────────────────────────────────────────┤
    │  OS, PROCESS, CPU, RAM/DISK, SWITCH     │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Aap ek chhota app bana rahe ho jismein sirf aapki apni 200 notes hain, aur sirf aap use karte ho. Database chahiye?

> **Jawab:** Nahi. Ek file kaafi hai.
>
> Chaaron problem dekho: 200 cheezein dhoondhna turant hai. Sirf aap likh rahe ho, toh takraav nahi. Beech mein rukna ek chhoti problem hai. Aur dohrav lagbhag nahi hai.
>
> Database ki keemat tab chukayi jaati hai jab woh chaar problem asli hon. Warna woh sirf ek aur cheez hai jise sambhalna padta hai.
>
> Yeh aage bar bar aayega: **har hal ki apni keemat hoti hai, aur woh keemat tabhi chukani chahiye jab problem asli ho.**

**2. (samajh check)** Ek aadmi apna naam badalta hai. Uske das lakh purane message mein naam likha hai. Do tareeke hain: sab jagah badal do, ya sirf ek jagah rakho aur baaki jagah ishara. Kaunsa behtar hai, aur kya kimat hai?

> **Jawab:** Ishara behtar hai, lekin muft nahi hai.
>
> Faayda: naam ek jagah hai, ek baar badla, sab jagah badal gaya.
>
> Keemat: ab har baar message dikhaate waqt naam alag se laana padta hai. Yaani ek kaam do jagah se hota hai, jo dheema hai.
>
> Isiliye kabhi kabhi log jaan-boojh ke dohrav rakhte hain, sirf speed ke liye. Aur phir unhe khud sambhalna padta hai ki dono jagah ek jaisa rahe.
>
> **Yeh iss poore part ka sabse aam sauda hai: sahi rakhna, ya tez rakhna.**

**3. (jodne wala)** Chapter 2.4 mein RAM aur disk ka farak tha. Database uss farak ka kaunsa istemaal karta hai?

> **Jawab:** Dono ka, ek saath.
>
> Woh data disk pe rakhta hai, taaki bijli jaane pe bache. Lekin woh jo hissa abhi kaam mein aa raha hai, use RAM mein rakhta hai, taaki tez ho.
>
> Aur likhte waqt woh pehle ek chhoti si "yeh hone wala hai" wali entry disk pe likhta hai, phir asli kaam karta hai. Isse beech mein bijli jaane pe woh baad mein dekh kar tay kar sakta hai ki kya poora hua tha aur kya nahi.
>
> Yeh teesri problem ka hal hai, aur Chapter 5.4 mein hum ise poora kholenge.
