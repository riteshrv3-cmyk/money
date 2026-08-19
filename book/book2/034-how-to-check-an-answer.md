# Chapter 5.4  [SPINE]
## Jawab sahi hai ya nahi, kaise check karein

*Yeh iss kitaab ka sabse practical chapter hai. Iske baad aap AI ko roz zyada surakshit tareeke se istemaal kar paoge.*

### Samvaad

**Madhav:** Aapko ek jawab mila. Ab batao ki woh sahi hai ya nahi.

**Kabir:** Usse poochta hoon ki kya woh pakka hai.

**Madhav:** Woh kya karega?

**Kabir:** Sambhavit jawab dega. "Haan, pakka."

**Madhav:** Toh woh raasta band hai. Doosra socho. Kya aapke paas koi aisa tareeka hai jo model se bahar ho?

**Kabir:** Main khud dekh lun.

**Madhav:** Har baar? Har jawab?

**Kabir:** Woh toh AI ka faayda hi khatam kar dega.

**Madhav:** Toh kaunse jawab jaanchne padenge aur kaunse nahi?

**Kabir:** Jinme galti mehngi ho.

**Madhav:** Bas. Ab ek aur cheez. Kuch jawab jaanchne mein aasan hote hain aur kuch mushkil. Farak batao.

**Kabir:** Code toh chala kar dekh sakta hoon.

**Madhav:** Aur ek tathya?

**Kabir:** Woh dhoondhna padega.

**Madhav:** Aur ek raay, jaise "yeh business idea achha hai"?

**Kabir:** Woh toh jaanchi hi nahi ja sakti.

**Madhav:** Toh teen alag darje ho gaye. Ab ek chalak tareeka. Chapter 4.3 se: agar aap wahi sawal paanch baar poochho toh?

**Kabir:** Agar paanchon jawab ek jaise hain toh woh sthir hai.

**Madhav:** Aur agar alag alag?

**Kabir:** Toh woh andaza laga raha hai.

**Madhav:** Yeh aapko sach nahi batata. Kya batata hai?

**Kabir:** Yeh ki kahan dhyaan dena hai.

**Madhav:** Ab ek aur. Aap poochte ho "Bharat ki rajdhani kya hai." Aur phir poochte ho "kya yeh sach hai ki Bharat ki rajdhani Mumbai hai?"

**Kabir:** Doosre mein woh sehmat ho sakta hai, kyunki maine daala hai.

**Madhav:** Toh sawal ki shakal jawab badal deti hai.

**Kabir:** Haan. Toh mujhe apna jawab sawal mein nahi daalna chahiye.

**Madhav:** Aur aakhri. Sabse mazboot tareeka kya hai?

**Kabir:** Use asli source dena, aur kehna ki wahin se jawab do.

**Madhav:** Aur phir?

**Kabir:** Aur phir source khud dekh lena.

**Madhav:** Toh aap kya kar rahe ho?

**Kabir:** Main use jawab dhoondhne wala bana raha hoon, jawab jaanne wala nahi.

**Madhav:** Yeh iss poore chapter ka nichod hai.

### Chaar tareeke, kaam ke kram mein

**1. Jaanch model ke bahar se aani chahiye.**

```
code           →  chala kar dekho
hisaab         →  calculator se milaao
tathya         →  source dhoondho
data           →  asli file se milaao
```

Yeh sabse mazboot hai. Aur zyadatar kaamon mein yeh mumkin hai, agar aap us shakal mein kaam karwao jo jaanchi ja sake.

**2. Use jawab dhoondhne wala banao, jaanne wala nahi.**

Asli jaankari saath bhejo aur kaho ki sirf usmein se jawab do. Phir jawab ko us jaankari se milaao.

Yeh hallucination ko bahut kam kar deta hai (Ch 5.1), kyunki ab jawab yaaddasht se nahi, saamne rakhi cheez se aa raha hai.

**3. Sthirta naapo, aatmvishwas nahi.**

Wahi sawal teen ya paanch baar poochho, alag alag chats mein.

```
sab jawab ek jaise    →  model sthir hai. (sahi hone ki guarantee nahi,
                          lekin ek sanket hai)
jawab alag alag       →  woh andaza laga raha hai. Dhyaan do.
```

Yeh uske aatmvishwas se kahin behtar naap hai, kyunki aatmvishwas dhaala gaya tha (Ch 2.8) aur yeh naapa jaata hai.

**4. Sawal mein apna jawab mat daalo.**

```
kamzor    "mujhe lagta hai X sahi hai, kya main sahi hoon?"
kamzor    "kya yeh sach hai ki X?"
behtar    "X ke paksh aur vipaksh mein sabse mazboot tark kya hain?"
behtar    "yeh galat kaise ho sakta hai?"
```

Pehle do mein aap use woh raasta de rahe ho jispe woh chalna chahta hai.

### Kab jaanchna zaroori hai

Har cheez jaanchna mumkin nahi hai. Toh ek saada niyam:

```
JAANCHO HAMESHA
├── numbers, tarikhein, naam, hawaale
├── kanooni, medical, paise wali baat
├── kuch bhi jo aage jaakar kisi aur ko bheja jaayega
└── kuch bhi jo aapke naam se jaayega

JAANCHNA ZAROORI NAHI
├── ideas aur shuruaati draft
├── woh baat jo aap khud jaante ho aur bas jaldi chahiye thi
└── aisa kaam jiska nateeja aap turant khud dekh lete ho
```

Aur ek aakhri niyam, jo Chapter 5.1 se seedha aata hai:

> **Sawal jitna khaas aur chhota, jaanch utni zaroori.**

Aam baaton pe woh mazboot hai. Ek khaas naam, ek chhoti tarikh, ek chhote ilaake ka niyam, wahan woh sabse zyada aatmvishwas se galat hota hai.

### Asli duniya se

Un logon ka tareeka jo isse sach mein kaam nikalte hain, aksar aisa dikhta hai:

```
1.  kaam ko aise tode ki har hissa jaancha ja sake
2.  jaankari saath bheje, yaaddasht pe bharosa na kare
3.  jawab ko aisi shakal mein maange jo machine jaanch sake
4.  aur ek chhota, apna test rakhe (Ch 5.3)
```

Aur woh log jo nirash hote hain, aksar ek bada, dhundhla sawal poochte hain, ek lamba jawab lete hain, aur use waise hi aage bhej dete hain.

**Farak model mein nahi hai. Farak kaam ki shakal mein hai.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **model se hi uski jaanch karwaana.**

"Check karo ki yeh sahi hai" ek jaanch nahi hai. Woh aur likhawat hai, usi tareeke se bani.

Thoda faayda hota hai, khaaskar jab aap asli jaankari saath do. Bina uske woh lagbhag bekaar hai.

Doosri galti: **aatmvishwas ko sanket samajhna.**

Woh sahi baat aur galat baat ek hi andaz mein kahega. Uska andaz uski dhalai se aaya hai, uske gyaan se nahi.

Teesri galti, jo sabse dhoke wali hai: **jaanch karna aur jaanch jaisa lagna.**

Aap poochte ho "kya tumne yeh source dekha?" aur woh kehta hai "haan, maine dekha." Agar uske paas woh source bheja hi nahi gaya, toh usne dekha kaise?

Woh jhooth nahi bol raha. Woh us jagah pe sambhavit vaakya likh raha hai.

**Jab tak aapne khud kuch bheja nahi, tab tak usne kuch dekha nahi.**

### Sochne ke liye

**1. (samajh check)** Aap AI se ek article ke liye teen aankde lete ho. Kya jaanchoge aur kaise?

> **Jawab:** Teeno, aur model se nahi.
>
> Har aankda ek asli source pe jaake dekho. Aur agar model ne source ka naam diya hai, toh woh naam bhi jaancho: source ka maujood hona aur usmein woh aankda hona, do alag cheezein hain.
>
> Aankde us kism ki cheez hain jahan model sabse zyada aatmvishwas se galat hota hai (Ch 5.1), aur jahan galti sabse zyada dikhti hai kyunki woh aapke naam se chhapegi.
>
> **Behtar tareeka:** pehle source dhoondho, phir model se kaho ki usi source se aankda nikaale. Ab kaam badal gaya: yaad karne se padhne mein.

**2. (samajh check)** Aap ek hi sawal teen baar poochte ho aur teeno jawab ek jaise aate hain. Kya woh sahi hai?

> **Jawab:** Zaroori nahi. Woh sthir hai.
>
> Ek model sthir roop se galat ho sakta hai, aur aksar hota hai. Agar galti data mein thi, ya woh kisi aam galat baat ko dohra raha hai, toh woh har baar wahi galat jawab dega.
>
> Sthirta yeh batati hai ki woh andaza nahi laga raha. Woh yeh nahi batati ki woh sahi hai.
>
> **Alag alag jawab ek chetavni hain. Ek jaise jawab chetavni ka na hona hai, saboot nahi.**

**3. (jodne wala)** Chapter 5.2 mein tha ki woh apni galti khud nahi pehchan sakta. Iss chapter ke chaar tareeke us seema se kaise nipatte hain?

> **Jawab:** Sab uske bahar se aate hain.
>
> Code chalana, calculator, source dekhna: yeh sab model ke bahar hain.
>
> Sthirta naapna: yeh model ko ek doosre ke khilaaf istemaal kar raha hai, uske andar nahi jhaank raha.
>
> Sawal ki shakal badalna: yeh use woh raasta nahi de raha jispe woh phisalta hai.
>
> **Ek cheez khud ko nahi jaanch sakti. Har asli jaanch bahar se aati hai.** Aur yehi Part 6 ka poora aadhaar hai: use tools dena, taaki woh bahar ki duniya se mil sake.
