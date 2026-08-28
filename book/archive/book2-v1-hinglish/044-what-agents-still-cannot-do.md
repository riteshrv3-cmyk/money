# Chapter 6.8  [SPINE]
## Agents abhi bhi kya nahi kar sakte

### Samvaad

**Madhav:** Ab uske paas jaankari hai, tools hain, aur ek loop hai. Chapter 5.2 wali aankh ki seemayein lagbhag hat gayin. Kya andar wali bhi hat gayin?

**Kabir:** Nahi. Woh abhi bhi nahi jaanta ki use kya nahi pata.

**Madhav:** Ab uska matlab kya hai, jab uske haath bhi hain?

**Kabir:** Woh aatmvishwas se galat kaam kar dega.

**Madhav:** Aur kya woh ruk kar poochega?

**Kabir:** Sirf tab jab use lage ki poochna chahiye. Aur woh "lagna" bhi sirf sambhavna hai.

**Madhav:** Toh do galtiyan mumkin hain. Batao.

**Kabir:** Ek: use poochna chahiye tha aur usne nahi poocha. Do: use kaam kar dena chahiye tha aur woh baar baar poochta raha.

**Madhav:** Aur dono ka ilaaj?

**Kabir:** Ilaaj yeh nahi ki woh behtar tay kare. Ilaaj yeh hai ki main tay karun ki kaunse kaam pe poochna zaroori hai.

**Madhav:** Bas. Ab doosri andar ki seema. Woh apni galti khud nahi pehchan sakta. Loop mein uska kya matlab hai?

**Kabir:** Kadam paanch ki galti kadam bees tak badi ho jaayegi, aur use pata nahi chalega.

**Madhav:** Aur agar aap use kaho "apna kaam check karo"?

**Kabir:** Woh check karne jaisa text likhega. Woh asli jaanch nahi hogi.

**Madhav:** Ab teesri. Woh lambe kaam pe khud tik nahi paata. Kyun?

**Kabir:** Kyunki uska plan sirf us likhawat mein hai jo ban chuki hai. Aur woh likhawat bhar jaati hai ya kat jaati hai.

**Madhav:** Ab ek nayi baat, jo tools ke saath aati hai. Ek agent teen ghante chala aur usne bees kaam kiye. Kya usne yeh socha ki bees kaam karne chahiye the ya nahi?

**Kabir:** Nahi. Usne har kadam pe agla kadam chuna.

**Madhav:** Toh usne kabhi peeche hat kar poori tasveer dekhi?

**Kabir:** Nahi. Uske paas woh jagah hi nahi hai.

**Madhav:** Aur aakhri. Kya use pata hai ki uske kaam ka asar kya hoga?

**Kabir:** Use asar dikhta hi nahi. Use sirf woh text dikhta hai jo wapas aaya.

**Madhav:** Toh uske paas kya nahi hai?

**Kabir:** Nateeje ka koi ehsaas. Uske liye ek file mitana aur ek file padhna, dono bas ek tool call hain.

**Madhav:** Aur wahi wajah hai ki aakhri faisla insaan ka hona chahiye.

### Naam

Char andar ki seemayein, aur ab unka asar hota hai:

```
1.  NAHI JAANTA KI KYA NAHI PATA
    tools ke saath: aatmvishwas se galat kaam

2.  APNI GALTI KHUD NAHI PEHCHAN SAKTA
    loop mein: galtiyan judti jaati hain, chup-chaap

3.  LAMBE KAAM PE KHUD TIK NAHI PAATA
    plan sirf likhawat mein hai, aur woh kat ta hai

4.  NATEEJE KA KOI EHSAAS NAHI
    "file padho" aur "file mitao" dono ek jaise tool calls hain
    keemat ka andaza uske andar hai hi nahi
```

Chauthi wali sabse zaroori hai aur sabse kam samjhi jaati hai.

Ek insaan intern jaanta hai ki kuch kaam wapas nahi hote. Woh us waqt ruk jaata hai, chahe kisi ne use na kaha ho. Woh ehsaas uske andar hai.

Model mein woh ehsaas nahi hai. Uske liye har tool call ek jaisi hai. **Keemat ka farak sirf us list mein hai jo aapne banayi.**

Aur isse iss poore Part ka nichod nikalta hai:

> **Agent us kaam mein achha hai jismein har kadam jaancha ja sakta hai, aur us mein khatarnak hai jismein galti wapas nahi hoti.**

```
ACHHA CHALTA HAI
├── code likhna aur chalana (test paas ya fail)
├── data nikalna aur milaana (source se milaao)
├── dhoondhna aur padhna (aap khud dekh sakte ho)
└── draft banana (aap padhoge hi)

KHATARNAK HAI
├── kuch bhejna (email, sandesh, paisa)
├── kuch mitana
├── settings badalna
└── kuch aisa jispe koi doosra insaan bharosa karega
```

### Asli duniya se

2024 aur 2025 mein bahut se "poora kaam apne aap kar dega" wale agents aaye, aur unmein se zyadatar demo mein kamaal the aur asli kaam mein nirash karte the.

Aur jo chale, unmein ek cheez saanjha thi: **woh chhote, jaanche ja sakne wale kaam karte the, aur beech mein insaan ko dikhate the.**

Code likhne wale agents isliye sabse aage nikle. Wahan har kadam pe ek asli jaanch hai jo model ke bahar se aati hai.

Yeh Book 1 Chapter 8.2 wali baat hai, teesri baar: **jinka sahi jawab saaf hai woh kaam aasan hain. Jinka dhundhla hai woh mushkil.** AI ne yeh niyam nahi badla. Usne sirf pehli list ko sasta kar diya.

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki agent ek "digital employee" hai.**

Ek employee ke paas nateeje ka ehsaas hota hai, apni galti pehchanne ki kshamta hoti hai, aur ek lakshya jo uske andar rehta hai.

In teeno mein se koi bhi yahan nahi hai. Jo hai woh ek loop hai, jo har kadam pe agla sambhavit kadam chunta hai.

Doosri galti: **aur zyada taakat dekar bharosa badhane ki koshish.**

Woh ulta chalta hai. Zyada taakat matlab zyada nuksaan jab woh bhatakta hai, aur woh bhatkega.

Bharosa jaanch se aata hai, aazadi se nahi.

Teesri galti: **yeh sochna ki yeh sab kal theek ho jaayega.**

Aankh ki seemayein tezi se hat rahi hain. Ye chaar andar wali seemayein pichhle kuch saal mein lagbhag nahi hilee hain.

**Aur jo aap bana rahe ho, uska design isi farak pe khada hona chahiye.**

### Sochne ke liye

**1. (samajh check)** Aap ek agent bana rahe ho jo aapke customers ko jawab de. Kya doge aur kya nahi?

> **Jawab:** Doge: apne documents padhne ka tool (Ch 6.2), aur jawab draft karne ka kaam.
>
> Nahi doge: seedha bhejne ki taakat, refund dene ki taakat, ya account badalne ki taakat.
>
> Aur beech mein ek insaan rakhoge, kam se kam un jawabon pe jo paise ya vaade se jude hon.
>
> **Kyunki ek galat jawab jo customer ko chala gaya, woh wapas nahi aata.** Aur model apni galti khud nahi pehchan sakta.

**2. (samajh check)** Aapka agent bees kadam chala aur nateeja galat hai. Sabse pehle kya dekhoge?

> **Jawab:** Har kadam ka record, shuru se.
>
> Kyunki galti aksar ek kadam pe hui aur baaki unnees us galti ke upar khade hain. Aakhri kadam dekhne se kuch nahi milega.
>
> Isliye har achhe agent system mein har kadam ka poora record rakha jaata hai: kya bheja gaya, kya laut a, kya chuna gaya.
>
> **Yeh Book 1 Ch 7.3 ka wahi sabak hai: itihaas ke bina aap sirf yeh jaan sakte ho ki kuch toota, kyun nahi.**

**3. (jodne wala)** Book 1 Ch 8.2 mein chaar pehchaanein thin ki kaunsa kaam aasan hai aur kaunsa mushkil. Agents pe woh kaise lagti hain?

> **Jawab:** Seedha lagti hain, aur woh sabse kaam ka naksha deti hain.
>
> ```
> sahi jawab saaf hai   →  agent achha chalega (code, data, hisaab)
> sahi jawab dhundhla   →  agent bhatkega aur pata nahi chalega
> waqt ki sakhti        →  agent dheema hai, loop mein waqt lagta hai
> paisa ya kanoon juda  →  insaan ka haath zaroori
> purani cheez chhoona  →  sabse khatarnak, kyunki wapas jaana mushkil
> ```
>
> **AI ne yeh chaar pehchaanein nahi badli.** Usne pehli wali list ko bahut sasta kar diya, aur baaki lagbhag waise hi hain.
>
> Aur wahi Chapter 7.2 ka aadhaar hai: ek aadmi 2026 mein kya bana sakta hai.
