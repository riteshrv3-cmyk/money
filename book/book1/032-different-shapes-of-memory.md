# Chapter 5.3  [SPINE]
## Memory ki alag shapes

---

### Samvaad

**Madhav:** Ek school ka record rakhna hai. Har student ka naam, roll number, class, marks. Kaise rakhoge?

**Kabir:** Ek table. Har student ek line, har cheez ek column.

**Madhav:** Har student ke paas wahi cheezein hain?

**Kabir:** Haan. Sabka naam hai, sabka roll number hai.

**Madhav:** Ab ek doosra kaam. Ek online dukaan. Har cheez ka naam aur daam. Lekin ek shirt ka size hai, ek kitaab ka lekhak hai, ek phone ki battery hai.

**Kabir:** Toh table mein bahut saare column honge, aur zyadatar khaali rahenge.

**Madhav:** Aur kal ek nayi cheez aayi jismein ek naya gun hai?

**Kabir:** Naya column jodna padega. Poori table mein.

**Madhav:** Har baar?

**Kabir:** Yeh mushkil hai. Toh har cheez ko apna alag dabba de do, aur usmein jo hai woh likh do.

**Madhav:** Toh ab har cheez ki shakal alag ho sakti hai.

**Kabir:** Haan.

**Madhav:** Ab problem batao.

**Kabir:** Agar shakal tay hi nahi hai, toh main galti se kuch bhi daal sakta hoon. Daam ki jagah naam.

**Madhav:** Aur koi rokega?

**Kabir:** Nahi. Kyunki koi niyam hai hi nahi.

**Madhav:** Toh table mein sakhti hai aur badalna mushkil. Dabbon mein aazadi hai aur galti aasan. Ab ek teesra kaam. Ek social app. Kaun kiska dost hai. Kaise rakhoge?

**Kabir:** Ek table: dost A, dost B.

**Madhav:** Ab poocho: mere dost ke dost kaun hain?

**Kabir:** Do baar dekhna padega.

**Madhav:** Aur unke dost ke dost?

**Kabir:** Teen baar. Har baar table dobara padhni padegi.

**Madhav:** Aur chhe kadam door tak?

**Kabir:** Yeh bahut mehnga ho jaayega.

**Madhav:** Toh yahan kya chahiye?

**Kabir:** Aisa tareeka jismein rishte hi asli cheez hon, aur unpe chalna sasta ho.

**Madhav:** Ab teen alag kaam, teen alag shakal. Ek line mein batao ki shakal kis cheez se tay hoti hai.

**Kabir:** Iss baat se ki main kya sawal poochunga.

**Madhav:** Bas. Data ki shakal data se nahi aati. Woh sawal se aati hai.

---

### Naam

Teen badi shakalein, aur unke naam:

```
TABLE (SQL)
├── har cheez ki shakal ek jaisi, pehle se tay
├── rishte numbers se jode jaate hain
├── sakhti: galat cheez daali nahi ja sakti
├── badalna mushkil: shakal badlo toh sab badalna padta hai
└── Postgres, MySQL, SQLite

DABBA (document / NoSQL)
├── har cheez ki apni shakal
├── ek cheez se judi saari jaankari ek hi jagah
├── aazadi: naya gun jodna aasan
├── khatra: koi niyam nahi, galti pakdi nahi jaati
└── MongoDB, Firestore

RISHTA (graph)
├── asli cheez rishte hain, cheezein nahi
├── "iske iske iske dost" jaise sawal sasta
├── kam istemaal hota hai, lekin jahan chahiye wahan koi vikalp nahi
└── Neo4j
```

Aur ab woh baat jo iss chapter ki asli seekh hai:

**Koi shakal behtar nahi hai. Shakal us sawal se aati hai jo aap sabse zyada poochoge.**

Bank ko table chahiye, kyunki wahan sakhti sabse zaroori hai. Ek nayi app ko shayad dabbe theek lagein, kyunki uski shakal abhi tay hi nahi hai. Ek social app ko rishton wali shakal chahiye.

Aur bahut se asli systems mein ek se zyada saath chalte hain, alag alag kaam ke liye.

Ek chetavni, kyunki yeh galti bahut mehngi padti hai. Log aksar shakal isliye chunte hain ki koi nayi hai ya charcha mein hai. Shakal badalna baad mein sabse mushkil kaam ho jaata hai, kyunki poora data usi shakal mein pad chuka hota hai.

**Language badalna hafte ka kaam hai. Data ki shakal badalna saal ka kaam hai.**

---

### Asli duniya se ek example

2010 ke aas-paas "NoSQL" ki badi lehar aayi. Kaha gaya ki table wale database purane ho gaye aur ab sab dabbon mein jaayega.

Bahut si companies ne apna data table se hata kar dabbon mein daal diya.

Kuch saal baad unmein se kai wapas aa gayin. Wajah yeh nahi thi ki dabbe kharaab the. Wajah yeh thi ki unhe sakhti chahiye thi aur unhone aazadi chun li thi, aur uski keemat unhe tab pata chali jab data mein gadbad milne lagi.

Aur ab dilchasp hissa: table wale database ne dabbe wali sahulat apne andar jod li. Aaj Postgres mein aap ek column ke andar poora dabba rakh sakte ho.

Yeh Chapter 3.3 wali baat hai, phir se: **jo cheez pehle se sab jagah hai, use hataya nahi jaata. Woh nayi cheez ko apne andar le leti hai.**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki "SQL vs NoSQL" ek behtar-ghatiya wala sawal hai.**

Log poochte hain "kaunsa achha hai" jaise ek jeet raha ho.

Sahi sawal alag hai: **mujhe sakhti chahiye ya aazadi? Aur main kaunse sawal sabse zyada poochunga?**

Aur ek aur galti isi ke saath aati hai: yeh sochna ki NoSQL ka matlab tez hai. Woh tez isliye lagta hai kyunki woh kuch cheezein nahi karta, jaise poori jaanch aur poori guarantee. Woh speed muft nahi hai. Aapne kuch chhoda hai, aur aksar aapko pata nahi hota ki kya chhoda.

Yeh galti tempting isliye hai ki tools ki tulna aise hi ki jaati hai, jaise phone ki. Lekin yeh tools alag kaam ke liye hain, ek hi kaam ke alag darje nahi.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  SHAKAL       table, dabba, rishta      │  ← naya
    │               sawal se tay hoti hai     │
    ├────────────────────────────────────────┤
    │  INDEX, DATABASE                        │
    ├────────────────────────────────────────┤
    │  INTERNET, PROTOCOL, PATA               │
    ├────────────────────────────────────────┤
    │  OS, CPU, RAM/DISK, SWITCH              │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek hospital ka system bana rahe ho jismein mareez ka record, dawai, aur bill hai. Kaunsi shakal, aur kyun?

> **Jawab:** Table.
>
> Wajah sakhti hai. Ek dawai ki matra galat shakal mein nahi jaani chahiye. Ek bill ka number kabhi khaali nahi hona chahiye. Aap chahte ho ki galat data andar ja hi na sake.
>
> Aur mareez, dawai, doctor, bill ke beech ke rishte tay hain aur badalte nahi.
>
> Yeh Chapter 3.3 wala sawal hai dobara: **galti ki keemat kitni hai?** Jahan keemat zyada hai, wahan sakhti chuni jaati hai, chahe woh likhne mein dheemi ho.

**2. (samajh check)** Ek naya app bana rahe ho aur aapko abhi pata nahi ki usmein kaunsi cheezein rakhni hongi. Dabbe chunoge?

> **Jawab:** Yeh sabse aam tark hai aur woh aadha sahi hai.
>
> Sahi: shuruaat mein shakal badalti rehti hai, aur dabbe usmein aasan hain.
>
> Aadha galat: shakal tab bhi maujood hoti hai. Woh sirf likhi nahi hoti. Woh aapke code mein bikhri hoti hai, aur jab teen saal baad koi naya aadmi aata hai, toh use kahin bhi nahi milti.
>
> Toh sawal yeh nahi hai ki shakal hai ya nahi. Sawal yeh hai ki **shakal ek jagah likhi hai, ya sau jagah bikhri hai.**

**3. (jodne wala)** Chapter 5.1 mein chauthi problem "dohrav" thi. Dabbon wali shakal us problem ke saath kya karti hai?

> **Jawab:** Woh use jaan-boojh ke wapas le aati hai.
>
> Table wali shakal kehti hai: naam ek jagah rakho, baaki jagah ishara.
>
> Dabbe wali aksar kehti hai: naam wahin rakh do jahan zaroorat hai, chahe woh das jagah ho.
>
> Faayda: padhte waqt sab ek jagah mil jaata hai, doosri jagah jaana nahi padta. Tez.
>
> Keemat: naam badla toh das jagah badalna padega, aur woh aapka kaam hai, database ka nahi.
>
> Yeh wahi sauda hai jo poore Part 5 mein chal raha hai: **sahi rakhna, ya tez rakhna.** Har shakal ne uska ek alag jawab chuna hai.
