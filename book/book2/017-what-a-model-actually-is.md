# Chapter 2.9  [SPINE]
## Model actually hai kya

### Samvaad

**Madhav:** Ab poora Part 2 dekh liya. Ek line mein batao ki model hai kya.

**Kabir:** Ek badi file jismein numbers hain.

**Madhav:** Bas?

**Kabir:** Aur ek program jo un numbers ko istemaal karta hai.

**Madhav:** Do alag cheezein?

**Kabir:** Haan. Numbers ek cheez hain, aur unhe chalane wala code doosri.

**Madhav:** Yeh farak zaroori hai. Ab ek sawal. Kya woh file copy ki ja sakti hai?

**Kabir:** Haan. Woh ek file hai.

**Madhav:** Aur agar main aapko woh file de doon?

**Kabir:** Toh mere paas poora model hai.

**Madhav:** Kya usmein kuch chhupa hai jo mere paas rahega?

**Kabir:** Nahi. File hi sab kuch hai.

**Madhav:** Ab yeh soch kar dekho. Karodon dollar, mahinon ki training, hazaaron machinein. Aur nateeja ek file hai jise koi bhi copy kar sakta hai, ek pen drive mein.

**Kabir:** Toh use rokne ka koi tareeka nahi hai?

**Madhav:** Ek hi tareeka hai: file kisi ko do hi mat. Use apne server pe rakho aur logon ko sirf sawal poochne do.

**Kabir:** Toh isiliye kuch models ki file milti hai aur kuch ki nahi.

**Madhav:** Bas. Aur yeh ek karobaari faisla hai, technical nahi. Ab ek aur baat. Woh file kya kar sakti hai, aur kya nahi?

**Kabir:** Woh sirf agla token guess kar sakti hai.

**Madhav:** Aur baaki sab?

**Kabir:** Baaki sab woh program karta hai jo use chalata hai.

**Madhav:** Ginao. Kya kya baaki hai?

**Kabir:** Sawal ko tokens mein badalna. Purani baat-cheet jodna. Har baar ek token chunna aur wapas daalna. Kab rukna hai yeh tay karna.

**Madhav:** Aur bhi. Kya bhejna hai model ko, kya nahi. Jawab pe kya filter lagana hai. Kya model ko kuch tools dene hain.

**Kabir:** Toh product ka bada hissa model ke bahar hai.

**Madhav:** Zyadatar log jise "AI" samajhte hain, uska bada hissa model ke bahar hai. Model ek purza hai, poori machine nahi.

### Naam

Do cheezein, hamesha alag:

```
WEIGHTS (file)
├── kuch sau GB, sirf numbers
├── training ka nateeja: mahinon, karodon dollar
├── sthir hai, kabhi badalti nahi
└── copy ki ja sakti hai, agar aapke paas ho

CHALANE WALA CODE
├── chhota, lagbhag muft
├── tokens banana, jodna, chunna, rokna
├── aksar open source, sabke liye maujood
└── isi mein saara product baitha hai
```

Aur poora product, jo aap istemaal karte ho, aisa dikhta hai:

```
┌───────────────────────────────────────────────┐
│  APP        aapki screen, chat, history       │
├───────────────────────────────────────────────┤
│  FILTER     kya andar jaayega, kya bahar aayega│
├───────────────────────────────────────────────┤
│  SANDARBH   purani baat, tools, aur woh cheezein│
│             jo sawal ke saath bheji jaati hain │
├───────────────────────────────────────────────┤
│  CHALANE WALA CODE                            │
├───────────────────────────────────────────────┤
│  WEIGHTS    ek sthir file                     │
└───────────────────────────────────────────────┘
```

Ab teen nateeje jo iss se seedhe nikalte hain.

**Ek: "AI product" aur "model" ek cheez nahi hain.** Do companies ek hi model ke upar bilkul alag product bana sakti hain, aur unmein bada farak dikhega. Us farak ka bada hissa model ke bahar wali parat mein hai.

**Do: model chori ho sakta hai, product nahi.** Isliye woh companies jo apni file deti hain, woh apna faayda kahin aur rakhti hain: product mein, data mein, ya paimane mein.

**Teen: "kaunsa model behtar hai" aksar galat sawal hai.** Aap jo istemaal karte ho woh poora dher hai. Ek behtar model ek kharaab dher mein kharaab lagega.

Aur ek aakhri baat, jo poore Part 2 ka nichod hai:

> **Model ek nichod hai jo ek yaantrik process se bana, ek chune hue data pe, ek tay kiye gaye lakshya ke liye, aur uske baad insaan ki pasand se dhaala gaya.**

Iss ek line ke andar Part 2 ke saare nau chapters hain. Aur usmein kahin bhi "samajh" ya "irada" jaisa shabd nahi hai.

### Asli duniya se

Kuch companies apne model ki file public karti hain. Koi bhi use download kar sakta hai, badal sakta hai, aur apne kaam ke liye dobara train kar sakta hai.

Doosri companies file kabhi nahi deti. Aap sirf unke server se sawal poochh sakte ho.

Ab Book 1 Chapter 3.6 ke chaar wajahon pe lagao. Ek company apni karodon dollar ki cheez muft mein kyun degi?

Wajahein wahi hain jo Book 1 mein thin: neeche wali parat pe kabza karna, taaki log aapke upar cheezein banayein. Naam aur saabiti. Aur yeh ki agar aap use nahi denge toh koi aur de dega, aur phir sab uske aas-paas banega.

Aur woh keemat bhi wahi hai: aapne apni sabse mehngi cheez de di, aur ab aapko paisa kahin aur se banana padega.

Yeh Chapter 7.1 ka aadha hissa hai, jahan hum poochenge ki iss udyog mein paisa kaun kamata hai.

### Yahan log kya galat samajhte hain

Sabse aam galti: **model aur product ko ek samajhna.**

Log kehte hain "yeh AI kharaab hai" jab aksar problem uss parat mein hoti hai jo model ke aas-paas lagi hai: kaunsi jaankari bheji gayi, kaunsa filter laga, kitni purani baat rakhi gayi.

Iska seedha nateeja: ek hi model do jagah bilkul alag lagta hai, aur log sochte hain ki unmein se ek jhooth bol raha hai.

Doosri galti: **yeh sochna ki model ke andar "AI" hai aur baaki sab bas ek wrapper hai.**

Woh parat hi aksar poore anubhav ka aadha hissa hai. Kya bheja jaata hai, kitna bheja jaata hai, aur kis tarah bheja jaata hai, yeh sab nateeje ko badalta hai.

Iska ek kaam ka roop hai: **jab jawab kharaab aaye, toh sirf model ko mat kosiye. Poocho ki use kya diya gaya tha.** Yeh Chapter 7.6 ka aadhaar hai.

### Sochne ke liye

**1. (samajh check)** Ek company apne model ki file public kar deti hai. Uske paas ab kya bacha hai?

> **Jawab:** Kaafi kuch, aur woh cheezein aksar file se badi hain.
>
> Product aur uska anubhav. Woh saara data jo unke paas aata hai aur aage ke models ko behtar karega. Woh machinein jinpe woh chalta hai, aur uska paimana. Aur woh log jo agla model bana sakte hain.
>
> **File ek nateeja hai. Use banane ki kaabiliyat file mein nahi hai.**
>
> Isiliye file de dena utna khatarnak nahi hai jitna lagta hai, agar aapke paas agli file banane ka rasta hai.

**2. (samajh check)** Aapko ek hi sawal ka do jagah alag jawab milta hai, aur dono ek hi model istemaal karte hain. Kya ho sakta hai?

> **Jawab:** Kuch bhi jo model ke bahar hai.
>
> Ek ne aapki purani baat-cheet bheji, doosre ne nahi. Ek ne ek chhupa hua nirdesh joda ("aise likho," "yeh mat karo"). Ek ne search ke nateeje saath bheje. Ek ne jawab pe filter lagaya. Ek ne alag temperature rakhi (Chapter 4.4).
>
> **Model wahi hai. Uske aas-paas ki parat alag hai.**
>
> Aur zyadatar mein aapko yeh kabhi nahi dikhaya jaata ki kya joda gaya tha.

**3. (jodne wala)** Book 1 Ch 1.6 mein tha ki program bhi sirf numbers hain, aur machine badalti nahi, sirf numbers badalte hain. Model us baat ka kaunsa roop hai?

> **Jawab:** Woh usi baat ka sabse bada roop hai.
>
> Wahi chip, wahi machine. Sirf ek nayi file, aur ab woh machine baat karti hai.
>
> Lekin ek farak hai jo naya hai. Book 1 mein woh numbers kisi insaan ne likhe the. Yahan nahi.
>
> Toh Book 1 ka niyam ab aisa dikhta hai:
>
> ```
> machine badalti nahi
> numbers badalte hain
> aur ab woh numbers khud bhi ek process se banaye ja sakte hain
> ```
>
> Yehi teesri tarah ke numbers thi, jo Chapter 1.1 mein aayi thi. Ab aap jaante ho ki woh kaise bante hain.
