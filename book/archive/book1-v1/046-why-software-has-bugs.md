# Chapter 7.1  [SPINE]
## Software mein bug hote hi kyun hain

---

### Samvaad

**Madhav:** Ek pul banaya jaata hai. Woh kitni baar girta hai?

**Kabir:** Lagbhag kabhi nahi.

**Madhav:** Ek app banaya jaata hai. Usmein kitni galtiyan hoti hain?

**Kabir:** Hamesha kuch na kuch.

**Madhav:** Toh pul banane wale software banane walon se behtar hain?

**Kabir:** Shayad. Ya unka kaam alag hai.

**Madhav:** Chalo dekhte hain. Ek pul kitni alag haalaton mein hota hai?

**Kabir:** Wahi ek pul hai. Wazan badalta hai, mausam badalta hai.

**Madhav:** Kitni haalatein? Sau? Hazaar?

**Kabir:** Shayad.

**Madhav:** Ab ek chhota sa program. Usmein sirf teen cheezein hain: user ka naam, umar, aur ek button. Kitni haalatein?

**Kabir:** Naam kuch bhi ho sakta hai. Umar bhi. Toh bahut zyada.

**Madhav:** Naam khaali ho sakta hai? Bahut lamba? Usmein emoji ho sakta hai? Doosri bhasha?

**Kabir:** Haan sab.

**Madhav:** Umar negative ho sakti hai? Zero? Ek lakh?

**Kabir:** Agar koi rok na ho toh haan.

**Madhav:** Aur button do baar dab sakta hai? Beech mein internet ja sakta hai? Do log ek saath kar sakte hain?

**Kabir:** Haan, haan, haan.

**Madhav:** Ab ginti karo.

**Kabir:** Yeh toh anginat ho gaya.

**Madhav:** Teen cheezon wale program mein. Ab ek asli app mein sau cheezein hoti hain, jo ek doosre se judi hain.

**Kabir:** Toh use poora jaancha hi nahi ja sakta.

**Madhav:** Bas. Yeh iss chapter ka poora jawab hai. Ab dhyaan do ki yeh koi kaushal ki kami nahi hai. Ab batao, banane wala kya kar sakta hai?

**Kabir:** Woh sab jaanch nahi sakta. Toh use chunna padega ki kya jaanche.

**Madhav:** Kis aadhaar pe chunega?

**Kabir:** Jo cheezein sabse zyada hoti hain. Aur jinme galti ki keemat sabse zyada hai.

**Madhav:** Aur baaki?

**Kabir:** Baaki mein galtiyan rahengi, aur woh kabhi na kabhi milengi.

**Madhav:** Toh software mein galti hona kya hai: ek nakaami, ya ek sachai?

**Kabir:** Sachai.

---

### Naam

Galti ko **bug** kehte hain. Naam ki kahani mashhoor hai: 1947 mein ek machine mein sach mein ek keeda fansa mila tha, aur us kaagaz pe likh diya gaya tha "first actual case of bug being found."

Lekin naam se zyada zaroori wajah hai. Do wajahein, aur dono Kabir ne chhui:

**Ek: haalaton ki ginti bahut badi hai.**

```
pul             ~ hazaar haalatein
chhota program  ~ anginat
bada app        ~ anginat, aur woh ek doosre se judi hain
```

Aur "anginat" ka matlab hai ki poora jaanchna namumkin hai. Yeh mushkil nahi hai, yeh namumkin hai.

**Do: software badalta rehta hai.**

Ek pul ban kar khada rehta hai. Ek app har hafte badalta hai. Aur har badlav ek nayi jagah hai jahan kuch toot sakta hai, aksar wahan jahan kisi ne dekha bhi nahi tha.

Bug ke teen aam ghar:

```
SEEMA PE            khaali, zero, negative, bahut bada, pehla, aakhri
                    (sabse zyada bug yahin hote hain)

EK SAATH            do log ek hi waqt pe (Chapter 5.4)
                    ya kaam beech mein ruk jaana

JOD PE              do hisse alag alag theek hain
                    aur milkar galat kaam karte hain
```

Teesra sabse mushkil hai. Ek aadmi ne apna hissa theek banaya, doosre ne apna. Dono sahi hain. Aur unke beech ki maanyata alag thi.

---

### Asli duniya se ek example

1999 mein NASA ka ek yaan Mars pe pahunchte hi kho gaya. Kaaran yeh nikla ki ek team ne apna hisaab ek naap mein diya aur doosri team ne use doosre naap mein padha.

Dono ka code sahi tha. Dono ne apna kaam theek kiya. Kisi ne likha hi nahi tha ki naap kaunsa hai, kyunki dono ko lagta tha ki yeh saaf hai.

Yeh teesre tarah ka bug hai, aur woh sabse mehnga hota hai. Woh kisi ek hisse mein nahi hota. Woh do hisson ke **beech** mein hota hai, aur uske liye koi zimmedar nahi hota.

Isiliye API (Chapter 6.4) itna zaroori hai. Woh sirf ek technical cheez nahi hai. Woh woh jagah hai jahan do hisson ki maanyataayein likh di jaati hain, taaki woh maanyataayein sirf kisi ke dimaag mein na rahein.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki bug ka matlab hai ki banane wala laaparwaah tha.**

Kuch bug laaparwaahi se aate hain. Zyadatar nahi.

Zyadatar bug un haalaton se aate hain jinke baare mein kisi ne socha hi nahi, kyunki sochne ke liye anginat haalatein thin.

Iska seedha nateeja: log software banane ka waqt bahut kam aankte hain. "Yeh toh chhota kaam hai" tab kaha jaata hai jab sirf seedha raasta dekha jaata hai. Aur asli waqt seedhe raaste mein nahi jaata, un sau tedhe raaston mein jaata hai jinka pata baad mein chalta hai.

Doosri galti: **yeh maan lena ki bug khatam kiye ja sakte hain.**

Woh kam kiye ja sakte hain. Zaroori jagahon pe lagbhag khatam kiye ja sakte hain, aur uski keemat bahut hoti hai: jahan galti se jaan jaati hai, wahan ek line code likhne mein ghante lagte hain aur uska daam sau guna hota hai.

Har baaki jagah pe, sawal yeh nahi hai ki bug hon ya na hon. Sawal yeh hai ki **kaunse bug bardaasht kiye ja sakte hain.** Aur woh ek karobaari faisla hai, technical nahi.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  BUG          haalatein anginat hain    │  ← naya
    │               poora jaanchna namumkin   │
    │               seema pe, ek saath, jod pe│
    ├────────────────────────────────────────┤
    │  KHARCHA, CLOUD, API, UPTIME            │
    ├────────────────────────────────────────┤
    │  QUEUE, CACHE, DATABASE, INTERNET       │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek form hai jismein sirf ek khaana hai: "apni umar likho." Kitni galat cheezein ho sakti hain?

> **Jawab:** Bahut zyada, aur ginne se hi samajh aata hai ki problem kya hai.
>
> Khaali. Zero. Negative. Dashamlav. Bahut bada number. Akshar. Emoji. Space. Doosri bhasha ke ank. Bahut lamba text jo memory bhar de. Aisa text jo program ke liye kuch aur matlab rakhta ho.
>
> Ek khaane mein pandrah se zyada. Ab sau khaane wala app socho.
>
> **Isliye "chhota feature" jaisi koi cheez nahi hoti. Har feature apne saath ek anginat duniya laata hai.**

**2. (samajh check)** Do team alag alag hisse banati hain. Dono ka code sahi hai. Phir bhi milkar cheez toot jaati hai. Kya hua?

> **Jawab:** Unki maanyataayein alag thin, aur woh kisi ne likhi nahi thin.
>
> Ek ne socha ki tarikh iss shakal mein aayegi, doosre ne doosri shakal mein. Ek ne socha ki khaali ho sakta hai, doosre ne socha kabhi nahi.
>
> Yeh sabse mehnga bug hai kyunki jaanch dono taraf paas ho jaati hai.
>
> Ilaaj: **maanyataayein likh do, aur unhe jaancho.** Yahi API ka asli kaam hai. Woh do dimaagon ke beech ka anumaan ek kaagaz pe le aata hai.

**3. (jodne wala)** Chapter 3.2 kehta tha ki kuch galtiyan compiler pakad leta hai aur kuch sirf chalne pe dikhti hain. Ab woh baat poori karo.

> **Jawab:** Compiler shakal ki galtiyan pakad sakta hai: galat likha, do cheezein jo jud hi nahi sakti.
>
> Woh **matlab** ki galtiyan nahi pakad sakta: aapne jodne ki jagah ghata diya, aapne galat cheez ki jaanch ki, aapne ek haalat sochi hi nahi.
>
> Isliye "compile ho gaya" ka matlab hai ki program chal sakta hai, na ki yeh ki woh sahi hai.
>
> Aur isiliye jaanch ek alag kaam hai, jo agle chapter ka vishay hai.
