# Chapter 7.6  [SPINE]
## AI ko expert ki tarah chalana

*Iss chapter mein koi nayi cheez nahi hai. Har baat kitaab ke kisi chapter se aayi hai. Yeh sirf unhe kaam ke roop mein rakhta hai.*

### Samvaad

**Madhav:** Ab aap sab jaante ho. Toh batao: expert aur aam user mein farak kya hai?

**Kabir:** Expert ko pata hai ki andar kya ho raha hai.

**Madhav:** Aur us jaankari se woh kya alag karta hai?

**Kabir:** Woh use aisi cheez nahi poochta jo woh kar hi nahi sakta.

**Madhav:** Aur?

**Kabir:** Woh use jaankari deta hai, yaad se maangta nahi.

**Madhav:** Aur?

**Kabir:** Woh jawab jaanchta hai.

**Madhav:** Bas teen? Ek aur socho. Aap ek sawal likhte ho. Usmein aapka nazariya hota hai?

**Kabir:** Aksar hota hai. "Mujhe lagta hai X sahi hai..."

**Madhav:** Aur uska kya asar hai?

**Kabir:** Woh us taraf khinch jaata hai. Chapter 2.8, 5.4.

**Madhav:** Toh chautha?

**Kabir:** Apna jawab sawal mein mat daalo.

**Madhav:** Aur paanchva. Ek lambi baat-cheet mein jawab kharaab hote ja rahe hain. Expert kya karega?

**Kabir:** Nayi chat shuru karega. Chapter 4.4.

**Madhav:** Aur chhatha, jo sabse kam kiya jaata hai. Aap ek bada kaam dete ho. Kya karna chahiye?

**Kabir:** Chhote tukdon mein todna. Kyunki lambe kaam mein galtiyan judti hain. Chapter 6.4.

**Madhav:** Aur har tukde ke baad?

**Kabir:** Dekh lena ki theek hai ya nahi, aage badhne se pehle.

**Madhav:** Bas. Ab dhyaan do ki inmein se ek bhi "jaadui shabd" nahi hai.

**Kabir:** Sab kuch iss baat se aaya ki andar kya ho raha hai.

**Madhav:** Aur wahi asli farak hai.

### Aath niyam

**1. Use woh mat poochho jo woh kar hi nahi sakta.**

Pehle poochho: yeh aankh ki seema hai ya andar ki? *(5.2)*

```
akshar ginna, hisaab, taazi baat, aapka data
   →  aankh ki seema, tool ya jaankari se hat jaayegi

"kya tumhe pakka pata hai," "apni galti dhoondho"
   →  andar ki seema, ismein kuch nahi milega
```

**2. Jaankari do, yaad se mat maango.**

Jo cheez data mein kam thi, wahan woh sabse zyada aatmvishwas se galat hoga *(5.1)*. Toh use saamne rakh do.

```
kamzor    "hamari chhutti ki policy kya hai?"
mazboot   "yeh rahi hamari policy [text]. Iske hisaab se batao..."
```

**3. Apna jawab sawal mein mat daalo.**

```
kamzor    "mujhe lagta hai X sahi hai, kya main sahi hoon?"
kamzor    "kya yeh sach hai ki X?"
mazboot   "X ke paksh aur vipaksh mein sabse mazboot tark kya hain?"
mazboot   "yeh galat kaise ho sakta hai?"
```

**4. Sandarbh se matlab kheencho.**

Ek shabd ka matlab uske aas-paas se banta hai *(3.2)*. Toh pehle duniya set karo, phir sawal poochho.

```
kamzor    "python ke baare mein batao"
mazboot   "main ek web server bana raha hoon. Python ke baare mein..."
```

**5. Bada kaam todo. Har tukde ke baad dekho.**

Lambe loop mein galtiyan judti hain aur pata nahi chalta *(6.4)*. Teen kadam ka kaam tees kadam ke kaam se lagbhag hamesha behtar chalta hai.

**6. Jaanch hamesha bahar se.**

Code chala kar, source dekh kar, hisaab milaa kar. Model se uski hi jaanch mat karwao *(5.4)*.

**7. Bharosa naapna ho toh sthirta naapo.**

Wahi sawal teen baar, alag chats mein. Ek jaise jawab ek sanket hain, alag alag jawab ek chetavni *(4.3)*.

**8. Chat gandi ho jaaye toh nayi shuru karo.**

Purani baat naye shabdon ka matlab kheenchti hai, context bharta hai, aur shuruaat kat jaati hai *(4.4)*. Nayi chat sabse sasta ilaaj hai.

### Chhoti baatein jo bada farak karti hain

```
JAWAB KI SHAKAL MAANGO      "sirf number do," "table mein do"
                             kyunki lamba jawab mehnga hai (4.2)
                             aur jaanchna mushkil (5.4)

USE ROLE MAT DO, SANDARBH DO "tum ek expert ho" se kam faayda
                             "yeh rahi asli jaankari" se zyada

KAM TOOLS DO                 zyada tools matlab galat chunav aur
                             zyada daam (6.3)

MISAAL DO                    ek achha udaharan das nirdeshon se
                             behtar kaam karta hai

NA KARNE WALI CHEEZ LIKHO    "yeh mat karna" aksar "yeh karna" se
                             zyada kaam ka hota hai
```

### Asli duniya se

Do log ek hi model istemaal karte hain. Ek kehta hai woh bekaar hai. Doosra usse roz asli kaam nikalta hai.

Farak aksar in paanch cheezon mein hota hai:

```
ek yaad se poochta hai        doosra jaankari deta hai
ek bada kaam ek saath deta    doosra tukdon mein
ek jawab maan leta hai        doosra jaanchta hai
ek apna jawab sawal mein daal doosra khula sawal poochta hai
ek ek hi lambi chat mein rehta doosra nayi shuru karta hai
```

**Model dono ke liye ek hi hai.** Farak iss baat mein hai ki kisko pata hai ki andar kya ho raha hai.

### Yahan log kya galat samajhte hain

Sabse aam galti: **"prompt engineering" ko jaadui shabdon ki list samajhna.**

Log lambi templates copy karte hain jinme "tum ek vishwa-prasiddh expert ho" jaisa likha hota hai.

Uska asar chhota hai. Bada asar in cheezon se aata hai: kaunsi jaankari saath gayi, kaam kitna chhota tha, aur jaanch kya thi.

Doosri galti: **AI ko convince karne ki koshish.**

Log bahas karte hain, dobara samjhaate hain, gussa karte hain. Woh sab context mein jud jaata hai aur aksar cheezein aur bigaad deta hai.

Agar do koshish mein sahi nahi hua, toh **nayi chat, behtar sawal.** Bahas se kuch nahi milta.

Teesri galti: **uske aatmvishwas ko sanket samajhna.** Ab tak yeh kitaab yeh baat paanch baar keh chuki hai, aur woh isliye ki yeh sabse mehngi galti hai.

### Sochne ke liye

**1. (samajh check)** Aap ek kaam do baar poochte ho aur dono baar jawab kharaab hai. Ab kya?

> **Jawab:** Teesri baar wahi mat poochho.
>
> Poochho: kya use woh jaankari mili jo chahiye thi? Kya kaam bahut bada tha? Kya maine apna jawab sawal mein daal diya? Kya chat gandi ho chuki hai?
>
> Aur phir **nayi chat, badla hua sawal.**
>
> Usi chat mein teesri koshish lagbhag hamesha kharaab hoti hai, kyunki ab do kharaab jawab bhi context mein hain aur woh agle jawab ko kheench rahe hain.

**2. (samajh check)** Aapko ek lambe document se das cheezein nikaalni hain. Kaise poochoge?

> **Jawab:** Ek ek karke, ya chhote batch mein. Sab ek saath nahi.
>
> Kyunki das cheezein ek saath maangne mein woh kuch chhod dega aur aapko pata nahi chalega. Aur jawab lamba hoga, jo mehnga aur jaanchne mein mushkil hai.
>
> Aur jawab aisi shakal mein maango jo jaanchi ja sake: har cheez ke saath woh line jahan se woh aayi.
>
> **Phir aap ek nazar mein dekh sakte ho ki woh line sach mein document mein hai ya nahi.** Yeh Chapter 6.2 ka wahi source dikhane wala niyam hai, ab aapke haath mein.

**3. (jodne wala)** In aath niyamon mein se kaunsa Book 1 se aata hai, AI se nahi?

> **Jawab:** "Bada kaam todo aur har tukde ke baad dekho."
>
> Woh Book 1 Chapter 8.4 hai: thoda badlo, dekho, phir aage badho. Aur Chapter 7.5: chhota kaam theek se aanka jaata hai, bada nahi.
>
> Aur "jaanch hamesha bahar se" bhi Book 1 Chapter 7.2 se aata hai: jaanch ka kaam bharosa dena hai, aur woh cheez khud ko nahi jaanch sakti.
>
> **Yeh dhyaan dene laayak hai. AI ko chalane ke aadhe niyam AI ke baare mein hain hi nahi.** Woh us baat ke baare mein hain ki kisi bhi cheez pe kaise kaam kiya jaata hai jispe poora bharosa na ho.
