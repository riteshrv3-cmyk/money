# Chapter 6.2  [SPINE]
## Use apne documents dena

### Samvaad

**Madhav:** Aapke paas paanch hazaar documents hain. Aap chahte ho ki AI unke baare mein jawab de. Kya karoge?

**Kabir:** Sab bhej doon?

**Madhav:** Kitne tokens honge?

**Kabir:** Karodon. Context mein aayenge hi nahi. Aur agar aa bhi jaate toh har sawal pe poora prefill hota. *(4.2, 4.4)*

**Madhav:** Toh?

**Kabir:** Sirf kaam ke documents bhejun.

**Madhav:** Kaunse kaam ke hain, yeh kaise pata chalega?

**Kabir:** Sawal se milte-julte.

**Madhav:** "Milta-julta" kaise naapoge? Shabd milaao?

**Kabir:** Woh kaam nahi karega. Main "chhutti ke niyam" poochunga aur document mein "avkash neeti" likha hoga.

**Madhav:** Toh shabd se nahi. Kis se?

**Kabir:** Matlab se.

**Madhav:** Matlab ko naapne ka koi tareeka humne dekha hai?

**Kabir:** Embedding! Chapter 3.1. Milti-julti cheezein paas hoti hain.

**Madhav:** Toh poora tareeka bolo.

**Kabir:** Har document ki embedding bana lo, pehle se. Sawal aane pe uski embedding banao. Phir dekho ki kaunse documents uske sabse paas hain.

**Madhav:** Aur phir?

**Kabir:** Woh das documents sawal ke saath bhej do.

**Madhav:** Aur model?

**Kabir:** Model unhe padh kar jawab dega. Yaad se nahi, saamne se.

**Madhav:** Ab do problem hain. Pehli: aapke document sau page ke hain. Poora document sabse paas hai, lekin usmein sirf ek paragraph kaam ka hai.

**Kabir:** Toh document ko tukdon mein tod do. Har tukde ki apni embedding.

**Madhav:** Kitne bade tukde?

**Kabir:** Bahut chhote toh matlab toot jaayega. Bahut bade toh shor aa jaayega.

**Madhav:** Aur agar jawab do tukdon ke beech mein baant kar likha ho?

**Kabir:** Toh tukdon ko thoda overlap karna padega.

**Madhav:** Doosri problem. Aapne das tukde bheje aur unmein jawab hai hi nahi. Model kya karega?

**Kabir:** Woh kuch bana dega. Chapter 5.1.

**Madhav:** Toh kya karna padega?

**Kabir:** Use saaf batana padega: "agar in tukdon mein jawab nahi hai toh keh do ki nahi mila."

**Madhav:** Aur kya?

**Kabir:** Aur jawab ke saath yeh bhi dikhaye ki kaunse tukde se aaya.

**Madhav:** Kyun?

**Kabir:** Taaki main khud dekh sakun. Chapter 5.4.

**Madhav:** Aapne poora system bana diya, aur uske teeno kamzor hisse bhi.

### Naam

Iss poore tareeke ka naam hai **RAG**: pehle dhoondho, phir jawab do.

```
PEHLE SE (ek baar)
1.  har document ko tukdon mein todo
2.  har tukde ki embedding banao
3.  unhe ek aise database mein rakho jo "paas wali" cheez dhoondh sake

HAR SAWAL PE
4.  sawal ki embedding banao
5.  sabse paas ke das tukde nikalo
6.  woh tukde sawal ke saath bhejo
7.  model unhi se jawab de, aur source dikhaye
```

Woh database jo embedding se dhoondhta hai, use **vector database** kehte hain. Aur woh Book 1 Chapter 5.2 ke index ka hi ek roop hai: **poori list padhne ki jagah, seedha paas wali cheez tak pahunchna.**

Ab teen baatein jo iss chapter ki jaan hain.

**Ek: yeh model ko sikhaana nahi hai. Yeh use dikhana hai.**

Model badalta nahi. Woh har baar naye sire se padhta hai jo aapne bheja.

Isliye aap ek document badal do aur agla jawab turant naya hoga. Training mein aisa karne ke liye karodon dollar lagte.

**Do: yeh hallucination ka sabse asli ilaaj hai.**

Chapter 5.1 se: woh isliye banata hai kyunki us jagah pe uske andar kuch bacha nahi tha. Agar aap woh cheez saamne rakh do, toh use banane ki zaroorat hi nahi rehti.

Aur agar aap uske saath source dikhwaao, toh aap jaanch bhi sakte ho.

**Teen: iski teen kamzoriyan hain, aur teeno dhoondhne wale hisse mein hain.**

```
GALAT TUKDE MILE      dhoondhna sahi tukda nahi laaya
                      → model ke paas jawab tha hi nahi

JAWAB BIKHRA HUA      jawab paanch documents mein baanta hai
                      → das tukde laane se poori tasveer nahi banti

SAWAL DHUNDHLA        "hamari policy kya hai" ki embedding
                      kisi khaas cheez ke paas nahi hai
                      → kuch bhi aa sakta hai
```

Aur teeno mein model bilkul theek kaam kar raha hota hai. **RAG mein jab jawab kharaab aata hai, toh problem aksar dhoondhne mein hoti hai, model mein nahi.**

Yeh sabse zaroori practical baat hai jo iss chapter mein hai.

### Asli duniya se

Lagbhag har "apne data pe AI" wala product isi tareeke pe khada hai: company ke documents, customer support, kanooni kaagaz, medical record.

Aur lagbhag har aisa product jo nirash karta hai, ek hi wajah se karta hai: **dhoondhna kamzor hai.**

Log dhyaan model pe dete hain, aur asli kaam un cheezon mein hai jo boring lagti hain: tukde kitne bade hon, unmein overlap kitna ho, kya document ke shirshak bhi tukde ke saath jaayein, aur kya embedding ke saath saath seedha shabd milaana bhi chalaya jaaye.

**Yeh Book 1 ka wahi sabak hai: hisaab sasta hai, sahi data laana asli kaam hai.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **RAG ko "model ko training dena" samajhna.**

Log kehte hain "maine AI ko apne documents pe train kiya." Aksar unhone kuch bhi train nahi kiya. Unhone ek dhoondhne wali cheez banayi jo har sawal pe kuch tukde bhej deti hai.

Yeh farak mayne rakhta hai kyunki dono ki keemat aur kamzoriyan bilkul alag hain.

Doosri galti: **yeh maan lena ki agar document system mein hai toh model ne use dekh liya.**

Woh sirf woh das tukde dekhta hai jo iss sawal ke liye laaye gaye. Baaki paanch hazaar documents uske liye maujood hi nahi hain.

Isliye "usne to poora manual padh liya hai" galat hai. Usne das tukde padhe.

Teesri galti: **jab jawab kharaab ho toh model badal dena.**

Pehle dekho ki kaunse tukde bheje gaye the. Agar jawab un tukdon mein tha hi nahi, toh naya model bhi wahi galat jawab dega.

### Sochne ke liye

**1. (samajh check)** Aap poochte ho "chhutti ke niyam kya hain" aur jawab galat aata hai. Sabse pehle kya dekhoge?

> **Jawab:** Kaunse tukde bheje gaye the.
>
> Agar sahi tukda bheja hi nahi gaya, toh model kuch nahi kar sakta tha. Problem dhoondhne mein hai.
>
> Agar sahi tukda bheja gaya tha aur phir bhi jawab galat hai, tab problem model ya nirdesh mein hai.
>
> **Yeh do bilkul alag problem hain aur unke ilaaj bilkul alag hain.** Aur zyadatar log seedha model ko doshi maan lete hain.

**2. (samajh check)** Aap chahte ho ki agar jawab documents mein na ho toh woh saaf mana kar de. Kaise karoge?

> **Jawab:** Use saaf likh kar batana padega, har baar, nirdesh mein.
>
> Aur usse zyada mazboot tareeka: jawab ke saath source maango. Agar woh source nahi de sakta, toh jawab bhi nahi dena chahiye.
>
> Aur uske baad ek jaanch bhi lagayi ja sakti hai, model ke bahar: **kya jo source usne diya, woh sach mein bheje gaye tukdon mein hai?** Agar nahi, toh jawab rok do.
>
> Yeh Chapter 5.4 ka wahi niyam hai: **jaanch hamesha bahar se.**

**3. (jodne wala)** Book 1 Ch 5.2 mein index tha, aur Ch 5.5 mein cache. RAG unse kaise judta hai?

> **Jawab:** Woh dono ka mishran hai.
>
> **Index ki tarah:** poori list padhne ki jagah seedha kaam ki cheez tak. Bas yahan "kaam ki" ka matlab shabd milna nahi, matlab milna hai.
>
> **Cache ki tarah:** woh model ke andar ka gyaan nahi hai. Woh bahar rakhi hui cheez hai jo waqt pe laayi jaati hai. Aur uska sauda bhi wahi hai: woh purani ho sakti hai, aur use update karna aasan hai.
>
> **Aur yahi uski sabse badi khoobi hai.** Document badlo, agla jawab naya. Model ko chhuye bina.
