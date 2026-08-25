# Chapter 4.6  [SPINE]
## Public road pe private baat

---

### Samvaad

**Madhav:** Tumhara packet ghar se nikalta hai aur server tak pahunchta hai. Beech mein kitni machinein hoti hain?

**Kabir:** Pata nahi. Kuch.

**Madhav:** Aam taur pe das se bees. Aapki internet company ki, phir beech wale raaston ki, phir manzil wale ki. Kya har ek us packet ko padh sakti hai?

**Kabir:** Haan. Woh toh usmein se guzar raha hai.

**Madhav:** Toh tum jo bank ka password bhejte ho, woh bees ajnabi machinein dekh sakti hain.

**Kabir:** Toh use chhupana padega.

**Madhav:** Kaise?

**Kabir:** Ghuma do. Har akshar ko kuch aage khiska do. A ko D, B ko E.

**Madhav:** Ab lene wala use kaise kholega?

**Kabir:** Peeche khiskayega. Use pata hona chahiye ki kitna.

**Madhav:** Woh "kitna" hi chaabi hui. Ab problem batao.

**Kabir:** Use woh chaabi kaise pata chalegi?

**Madhav:** Bhej do.

**Kabir:** Toh beech wale bhi dekh lenge.

**Madhav:** Toh chaabi ko chhupa kar bhejo.

**Kabir:** Usko chhupane ke liye ek aur chaabi chahiye. Yeh phir ghoom raha hai.

**Madhav:** Yehi asli problem hai, aur do hazaar saal se yehi problem thi. Chaabi hamesha pehle se milni padti thi, aamne-saamne. Ab batao, kya aap us bank se kabhi mile ho jiska app aap chalate ho?

**Kabir:** Nahi.

**Madhav:** Toh 1970 tak yeh mumkin hi nahi tha. Ab main tumhe ek ajeeb sawal deta hoon. Kya aisa taala ho sakta hai jise koi bhi band kar sake, lekin khol sirf ek aadmi paaye?

**Kabir:** Hmm. Ek dabba jismein chitthi daali ja sakti ho lekin nikaali na ja sake. Post box.

**Madhav:** Bilkul. Post box ka muh sabke liye khula hai. Chaabi sirf postman ke paas.

**Kabir:** Toh woh bank sabko apna post box de de.

**Madhav:** Aur woh post box public ho, sabke saamne?

**Kabir:** Haan. Usse koi nuksaan nahi. Usmein daal hi sakte hain, nikaal nahi sakte.

**Madhav:** Toh ab bank ko chaabi bhejne ki zaroorat hai?

**Kabir:** Nahi. Woh apna post box sabko de sakta hai. Main usmein daal dunga, sirf woh kholega.

**Madhav:** Tumne abhi woh cheez nikaali jisne poore internet ka vyapar mumkin banaya. Ek aakhri sawal. Main tumhe ek post box deta hoon aur kehta hoon ki main bank hoon. Tumhe kaise pata ki main sach mein bank hoon?

**Kabir:** Pata nahi chalega.

**Madhav:** Toh?

**Kabir:** Koi teesra ho jise dono jaante hon, aur woh bataye ki yeh sach mein bank hai.

**Madhav:** Aur us teesre pe kaun bharosa karega?

**Kabir:** Woh pehle se sabke paas hona chahiye.

**Madhav:** Jaise protocol. Pehle se maujood, kyunki bheja nahi ja sakta.

---

### Naam

Wo do tarah ki chaabi wali cheez, uska naam hai **public key cryptography**.

```
PUBLIC KEY    sabko do. Isse band kiya ja sakta hai.
PRIVATE KEY   kisi ko mat do. Sirf isse khulta hai.
```

Aur woh teesra, jo batata hai ki koi sach mein wahi hai jo keh raha hai, use **certificate authority** kehte hain. Unke naam aapke phone aur browser mein pehle se bhare hote hain, jab woh bana tha.

Poori baat-cheet aise chalti hai:

```
1. tum server se juda, usne apna public key aur certificate diya
2. tumne certificate check kiya un naamon se jo pehle se tumhare paas the
3. theek nikla, toh tumne ek nayi chaabi banayi, sirf iss baat-cheet ke liye
4. woh nayi chaabi server ke public key se band karke bheji
5. ab dono ke paas ek hi chaabi hai, aur baaki saari baat usi se hoti hai
```

Aakhri kadam kyun? Kyunki public key wali cheez dheemi hai. Toh use sirf ek baar istemaal karte hain, ek aam chaabi bhejne ke liye. Uske baad tez wali chalti hai.

Yeh poori cheez **TLS** hai, aur jab HTTP uske andar chalta hai toh use **HTTPS** kehte hain. Woh taala jo aapke browser mein dikhta hai, wahi hai.

Aur ab woh baat jo log lagbhag hamesha galat samajhte hain, isliye ise saaf likh raha hoon:

**Taala sirf yeh batata hai ki raaste mein koi padh nahi sakta. Woh yeh nahi batata ki doosri taraf wala imaandaar hai.**

Ek thagne wali website pe bhi taala ho sakta hai, aur aksar hota hai. Usne bas yeh saabit kiya hai ki woh wahi naam hai jo likha hai. Ki woh naam bharosa laayak hai ya nahi, uska iss taale se koi lena dena nahi.

---

### Asli duniya se ek example

2015 tak zyadatar websites bina taale ke chalti thin, kyunki certificate mehnga tha aur lagana mushkil tha. Sirf bank aur bade sites hi lagate the.

Phir ek muft aur apne aap chalne wali certificate dene wali cheez shuru hui, Let's Encrypt. 2016 mein web ka lagbhag aadha traffic taale ke saath tha. Aaj lagbhag 95 pratishat se zyada hai.

Chapter 3.6 ke chaar wajahon pe lagao. Yeh kisne banaya aur kyun? Ise browser banane wali companies ne paisa diya. Unhe iska seedha paisa nahi mila.

Unka faayda yeh tha ki poora web surakshit ho gaya, aur unka product uspe khada hai. Neeche wali parat sabke liye muft kar do, taaki upar wali cheez chal sake.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **taale ko "yeh site surakshit hai" samajhna.**

Log taala dekh kar apna card number daal dete hain, yeh sochkar ki taale ka matlab bharosa hai.

Taale ka matlab sirf itna hai: raaste mein koi nahi padh sakta, aur doosri taraf wala wahi naam hai jo likha hai.

Ek thag ek naam khareed sakta hai, uspe taala laga sakta hai, aur aapka data poori suraksha ke saath apne paas mangwa sakta hai. Encryption ne uska kaam aur asaan hi kiya, kyunki ab aapka internet dene wala bhi nahi dekh sakta.

Yeh galti tempting isliye hai ki browser ne taale ka nishaan hi aisa banaya ki woh "sab theek hai" jaisa lagta hai. Woh sirf ek hi baat keh raha hai, aur log usse teen baatein sun lete hain.

Sahi soch:

```
taala kehta hai       →  raaste mein koi nahi padh raha
taala kehta hai       →  naam wahi hai jo dikh raha hai
taala NAHI kehta      →  yeh log imaandaar hain
taala NAHI kehta      →  aapka data unke paas surakshit hai
```

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  DO CHAABIYAN  ek band kare, ek khole   │  ← naya
    │  BHAROSA       teesra, pehle se maujood │  ← naya
    ├────────────────────────────────────────┤
    │  NAAM, PROTOCOL, PACKET, PATA           │
    ├────────────────────────────────────────┤
    │  OS, PROCESS, CPU, RAM/DISK, SWITCH     │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Aap ek public wifi pe ho. Ek site pe taala hai, doosri pe nahi. Wifi ka maalik kya dekh sakta hai?

> **Jawab:** Bina taale wali site pe: sab kuch. Har page, har shabd, har password.
>
> Taale wali site pe: sirf yeh ki aap kis naam se baat kar rahe ho, aur kitna data aa-ja raha hai. Andar ki baat nahi.
>
> Toh taala aapko chhupata nahi hai, woh aapki **baat** chhupata hai. Yeh farak mayne rakhta hai: koi ab bhi jaan sakta hai ki aap kis site pe gaye, bas yeh nahi ki wahan kya kiya.

**2. (samajh check)** Public key sabko diya jaata hai. Toh koi usse aapke sandesh khol kyun nahi sakta?

> **Jawab:** Kyunki woh chaabi sirf band karne ke liye hai, kholne ke liye nahi.
>
> Post box wale example mein: sabko us box ka muh dikhta hai, aur sab usmein daal sakte hain. Uska muh dekh kar koi andar ki chitthi nahi nikaal sakta.
>
> Yeh ganit se aata hai. Kuch hisaab aise hote hain jinhe ek taraf karna aasan hai aur ulta karna lagbhag namumkin. Do bade numbers guna karna aasan hai. Nateeje se wapas woh do numbers nikaalna bahut mushkil.

**3. (jodne wala)** Chapter 4.4 kehta tha ki protocol pehle se maujood hona zaroori hai, kyunki use bheja nahi ja sakta. Bharosa uss baat ka kaunsa roop hai?

> **Jawab:** Bilkul wahi roop.
>
> Bharosa bheja nahi ja sakta. Agar main tumhe bhej kar batata ki mujh pe bharosa karo, toh woh bekaar hai, kyunki koi bhi wahi bhej sakta hai.
>
> Isliye bharosa pehle se aana padta hai. Woh browser aur phone ke andar bhara jaata hai jab woh bante hain.
>
> Aur yahan ek gehri baat hai: **poori internet ki suraksha ek chhoti si list pe khadi hai jo aapke device mein pehle se pad gayi thi.** Aapne woh list kabhi nahi dekhi. Aapne kabhi tay nahi kiya ki usmein kaun ho.
