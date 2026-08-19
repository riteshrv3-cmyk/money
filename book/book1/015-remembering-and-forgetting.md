# Chapter 2.4  [SPINE]
## Yaad rakhna aur bhool jaana

---

### Samvaad

**Madhav:** Pichhle chapter mein tumne dekha ki paas wali jagah tez hai aur door wali dheemi. Ab sawal: sab kuch paas hi kyun nahi rakh lete?

**Kabir:** Jagah nahi hogi.

**Madhav:** Aur?

**Kabir:** Mehngi hogi?

**Madhav:** Dono sahi hain, aur ek teesri baat bhi hai jo tum abhi khud nikaaloge. Ek switch se ek bit banta hai. Us bit ko yaad rakhne ke liye kya chahiye?

**Kabir:** Switch ko usi haalat mein rakhna hoga.

**Madhav:** Aur switch usi haalat mein rehta kaise hai?

**Kabir:** Bijli aati rahegi toh rahega.

**Madhav:** Aur bijli chali gayi?

**Kabir:** Toh switch band ho jaayega. Sab kuch 0 ho jaayega.

**Madhav:** Bas. Tumne abhi computer ki sabse badi seema nikaal li. Jo cheez bijli se yaad rakhi jaati hai, woh bijli jaate hi gayab ho jaati hai.

**Kabir:** Toh phir meri photos kaise bachti hain?

**Madhav:** Kyunki woh switchon mein nahi rakhi hain. Unhe kisi aisi cheez mein rakha jaata hai jo bina bijli ke bhi apni haalat nahi badalti.

**Kabir:** Jaise?

**Madhav:** Jaise ek chhota sa dabba jismein kuch electron band kar diye jaate hain. Bijli chali jaaye toh bhi woh wahin fanse rehte hain. Unhe nikaalne ke liye khaas mehnat karni padti hai.

**Kabir:** Toh yeh behtar hai. Sab kuch usmein kyun nahi rakhte?

**Madhav:** Kyunki woh dheema hai. Electron ko band karne aur nikaalne mein waqt lagta hai, switch dabane se bahut zyada.

**Kabir:** Kitna zyada?

**Madhav:** Hazaar guna ke aas-paas. Aur agar ghoomne wali purani disk ho toh das lakh guna.

**Kabir:** Toh ek tez hai lekin bhool jaata hai, doosra yaad rakhta hai lekin dheema hai.

**Madhav:** Bas. Aur ab batao, agar tumhe machine banani ho, toh kya karoge?

**Kabir:** Dono rakhunga. Jispe abhi kaam chal raha hai woh tez wali mein, aur baaki sab dheemi wali mein.

**Madhav:** Aur jab program shuru hota hai?

**Kabir:** Toh dheemi se tez mein le aana padega.

**Madhav:** Isiliye phone chalu hone mein waqt lagta hai. Aur isiliye app pehli baar kholne mein dheema hota hai aur doosri baar tez.

**Kabir:** Aur isiliye bijli jaane pe jo maine save nahi kiya woh chala gaya.

**Madhav:** Save karne ka matlab kya hai, ab bolo.

**Kabir:** Tez wali jagah se dheemi wali jagah mein copy karna. Taaki bijli jaane pe bache.

**Madhav:** Bas yehi. "Save" ek jaadui shabd nahi hai. Woh ek jagah se doosri jagah copy karna hai.

---

### Naam

Do tarah ki jagah, aur inke naam har jagah milenge:

```
RAM   (tez, bhool jaane wali)
├── switchon jaisi cheezon mein rakha
├── bahut tez
├── bijli gayi, sab gaya
├── mehngi, isliye kam hoti hai
└── phone mein 6 se 16 GB

DISK / SSD   (dheemi, yaad rakhne wali)
├── electron fanse hue, ya chumbak
├── bahut dheemi
├── bijli gayi toh bhi bacha rehta hai
├── sasti, isliye zyada hoti hai
└── phone mein 128 se 512 GB
```

Aur ab poora dher, sabse tez se sabse dheema:

```
registers      ekdam CPU ke andar        1 kadam        kuch dozen numbers
cache          CPU ke bilkul paas        3 se 40 kadam  kuch MB
RAM            door, alag chip           ~200 kadam     kuch GB
SSD            aur door                  ~10 lakh kadam kuch sau GB
```

Har kadam pe wahi sauda: **tez, chhota, mehnga** ya **dheema, bada, sasta.**

Yeh dher poori computer ki duniya mein dohraya jaata hai. Aage aap ise phir dekhoge: database mein, network mein, server mein, aur AI mein. Har jagah wahi shakal.

---

### Asli duniya se ek example

2007 tak lagbhag har computer mein ghoomne wali disk hoti thi: ek dhaatu ki plate jo minute mein hazaaron baar ghoomti thi, aur ek sui uspar se padhti thi.

Us sui ko sahi jagah pahunchne mein lagbhag 10 millisecond lagte the. Chip ke hisaab se woh lagbhag **teen karod kadam** ka intezaar hai.

SSD mein koi cheez ghoomti nahi. Sirf electron hain. Wahi kaam lagbhag 0.1 millisecond mein hota hai, yaani sau guna tez.

Isiliye purane laptop mein SSD daalte hi woh naya lagne lagta hai. CPU wahi hai. RAM wahi hai. Sirf intezaar sau guna kam ho gaya.

Aur ab wapas Chapter 2.3 ki baat pe: **speed hisaab se nahi, doori se aati hai.**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **RAM aur storage ko ek hi cheez samajhna.**

Log kehte hain "mere phone mein 128 GB memory hai." Woh storage hai. RAM alag hai, aur woh 8 GB hogi.

Yeh sirf shabdon ka farak nahi hai. Iska seedha nateeja hai:

Jab phone kehta hai "jagah nahi hai," toh woh storage ki baat kar raha hai. Photos delete karni padegi.

Jab phone dheema ho jaata hai aur app band ho jaate hain, toh woh RAM ki baat hai. Photos delete karne se kuch nahi hoga. App band karne se hoga.

Do bilkul alag problem, do bilkul alag hal, aur log aksar galat wala lagate hain.

Yeh galti templing isliye hai ki dono ko "memory" kehte hain, aur dono GB mein naapte hain. Lekin ek yaad rakhti hai aur doosri bhool jaati hai, aur wahi asli farak hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  DO TARAH KI JAGAH                     │  ← naya
    │  tez + bhool jaane wali (RAM)          │
    │  dheemi + yaad rakhne wali (disk)      │
    ├────────────────────────────────────────┤
    │  CPU, DOORI                            │
    ├────────────────────────────────────────┤
    │  PAIMANA, COMPRESSION, SIZE            │
    ├────────────────────────────────────────┤
    │  PROGRAM, ENCODING, BINARY, SWITCH     │
    └────────────────────────────────────────┘

    Part 2 khatam.
```

---

### Part 2 ka gate

**1.** Aapka phone dheema chal raha hai aur app baar baar band ho rahe hain. Photos delete karne se faayda hoga? *(nahi aaya toh 2.4)*

> **Jawab:** Nahi. Yeh RAM ki problem hai, storage ki nahi.
>
> App band karo, ya phone restart karo. Photos delete karne se sirf storage khaali hoti hai, jiska iss problem se koi lena dena nahi.

**2.** "Naya AI model 400 GB ka hai." Kya woh aapke phone mein aa jaayega, aur kya woh chalega? *(nahi aaya toh 2.2, 2.4)*

> **Jawab:** Rakhne mein nahi aayega, kyunki aam phone mein 128 se 512 GB storage hoti hai aur usmein pehle se sab bhara hai.
>
> Aur agar aa bhi jaata, toh chalta nahi, kyunki chalane ke liye use RAM mein aana padta, aur phone mein 8 se 16 GB RAM hai.
>
> Rakhna aur chalana do alag sawal hain. Log inhe hamesha mila dete hain.

**3.** Ek program dheema hai. Do wajahein ho sakti hain. Batao. *(nahi aaya toh 2.3)*

> **Jawab:** Ek: hisaab bahut zyada hai. Do: data door se aa raha hai.
>
> Aur zyadatar mamlon mein doosri wali hi hoti hai.

---

### Chat app pe wapas

Part 2 ke baad, aapke chat app ke baare mein yeh saaf ho gaya:

```
Ek text message lagbhag 100 byte ka hai. Bahut sasta.
Ek photo lagbhag 30 lakh byte ki. Tees hazaar guna zyada.
Ek minute ka video ek lakh message ke barabar.

Message likhte waqt woh RAM mein hai. Bijli gayi toh gaya.
"Bhej diya" ka matlab hai woh kisi aisi jagah pahunch gaya
jo bijli jaane pe bhi use yaad rakhegi.

Aur jab aap purana message dhoondhte ho, toh woh disk se
aana padta hai, jo RAM se das lakh guna dheemi hai.
```

Agla sawal, jo Part 3 kholta hai:

**Woh nirdeshon ki list, jo app hai, likhi kisne? Aur insaan seedha numbers mein toh likhta nahi hoga?**
