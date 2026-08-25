# Chapter 6.3  [SPINE]
## Dikhne wala hissa, na dikhne wala hissa

---

### Samvaad

**Madhav:** Aap ek shopping app kholte ho. Saaman ki list dikhti hai, daam dikhta hai, ek button hai. Yeh sab kahan chal raha hai?

**Kabir:** Mere phone pe.

**Madhav:** Aur daam kahan se aaya?

**Kabir:** Server se.

**Madhav:** Toh do jagah kaam ho raha hai. Ab ek sawal. Daam ka hisaab kahan hona chahiye, phone pe ya server pe?

**Kabir:** Phone pe hoga toh tez hoga.

**Madhav:** Achha. Toh main apne phone mein daam ka hisaab badal doon aur ek rupaye mein khareed loon?

**Kabir:** Nahi... phir toh server pe hona chahiye.

**Madhav:** Kyun? Ek line mein.

**Kabir:** Kyunki phone mera hai. Main usmein kuch bhi badal sakta hoon.

**Madhav:** Bas. Yeh iss chapter ka poora niyam hai. Ab dobara batao: kya kya phone pe ho sakta hai?

**Kabir:** Dikhana. Rang, layout. Scroll karna. Shayad ginti ki jaanch, jaise khaali box.

**Madhav:** Aur woh jaanch phone pe kyun, jab server bhi kar sakta hai?

**Kabir:** Kyunki turant dikhta hai. Server tak jaane mein waqt lagta hai.

**Madhav:** Toh woh jaanch phone pe hai. Ab main phone mein woh jaanch hata doon aur khaali form bhej doon. Kya hoga?

**Kabir:** Server ko phir se jaanchna padega.

**Madhav:** Toh jaanch do jagah?

**Kabir:** Haan. Phone pe user ki suvidha ke liye, aur server pe sach mein.

**Madhav:** Ab yeh yaad rakho, kyunki yahin log sabse badi galti karte hain. Phone wali jaanch **madad** hai. Server wali jaanch **suraksha** hai. Dono ek jaisi dikhti hain aur unka kaam bilkul alag hai.

**Kabir:** Samajh gaya.

**Madhav:** Ab ek aur sawal. Woh saaman ki list phone pe aayi. Kis shakal mein aayi?

**Kabir:** Data ki shakal mein.

**Madhav:** Ya server poora page bana ke bhej sakta tha, saja hua, taiyaar.

**Kabir:** Woh bhi ho sakta hai.

**Madhav:** Dono mein kya farak padta hai?

**Kabir:** Agar server poora bana ke bheje toh phone ka kaam kam hoga aur pehli baar jaldi dikhega.

**Madhav:** Aur agar sirf data bheje?

**Kabir:** Toh phone ko banana padega. Pehli baar dheemi, lekin uske baad har chhote badlav ke liye poora page nahi laana padega.

**Madhav:** Aur ek teesri baat. Agar server poora page banata hai, toh kya wahi data ek doosre app ko bhi de sakta hai?

**Kabir:** Nahi. Page toh browser ke liye hai.

**Madhav:** Aur agar sirf data deta hai?

**Kabir:** Toh koi bhi le sakta hai. Phone app, website, koi aur company.

**Madhav:** Toh ab dono ke faayde saaf hain, aur koi ek jawab nahi hai.

---

### Naam

```
FRONT (dikhne wala hissa)
├── user ke device pe chalta hai
├── dikhana, chhoona, turant jawab
├── user use badal sakta hai, isliye uspe bharosa nahi
└── kaam: anubhav

BACK (na dikhne wala hissa)
├── server pe chalta hai
├── asli faisle, asli hisaab, asli data
├── user use chhoo bhi nahi sakta, isliye yahi sach hai
└── kaam: sachai aur suraksha
```

Aur woh ek niyam jo kabhi nahi tootta:

> **Client pe kabhi bharosa mat karo.**

Jo cheez user ke device pe chal rahi hai, use badla ja sakta hai. Chahe woh app ho, website ho, ya kuch bhi. Isliye har zaroori jaanch server pe dobara honi chahiye, chahe woh phone pe pehle ho chuki ho.

Do jaanch bekaar nahi hain. Woh do alag kaam kar rahi hain:

```
phone pe   →  user ko turant bata do, taaki use intezaar na ho
server pe  →  galat cheez andar aane hi mat do
```

Aur woh doosra sawal, page kahan bane:

```
SERVER PE BANE
├── pehli baar jaldi dikhta hai
├── purane aur dheeme device pe behtar
└── har chhote badlav pe server tak jaana padta hai

DEVICE PE BANE
├── pehli baar dheemi, uske baad tez
├── data alag milta hai, toh koi bhi use kar sakta hai
└── device pe zyada kaam, battery zyada
```

Aaj ke zyadatar bade systems dono karte hain: pehla page server se banaya hua, uske baad sab device pe.

---

### Asli duniya se ek example

Purane zamane mein har page server pe banta tha. Aap kuch bhi click karte, poora page dobara aata tha, aur screen safed hokar wapas aati thi.

2005 ke aas-paas ek naya tareeka phaila: page ko poora badalne ki jagah, sirf zaroori data mangwao aur page ka ek hissa badal do. Google Maps ne yeh mashhoor kiya, jahan aap naksha kheench sakte the aur page dobara nahi khulta tha.

Uske baad lehar itni door chali gayi ki lagbhag sab kuch device pe banne laga, aur log bhool gaye ki uski keemat kya hai. Websites bhaari ho gayin, purane phone pe atakne lagin, aur pehli baar khulne mein der lagne lagi.

Ab lehar wapas beech mein aa rahi hai. Pehla page server se, baaki device pe.

Yeh dhyaan dene laayak hai, kyunki yeh baar baar hota hai: **koi nayi cheez aati hai, log usse har jagah lagate hain, uski keemat dikhti hai, aur phir woh apni sahi jagah pe baith jaati hai.** Yeh kamzori nahi hai, yeh seekhne ka tareeka hai. Lekin agar aap beech mein aaye ho toh lagta hai ki sab log ek disha mein daud rahe hain.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki app ke andar ka code chhupa hua hai.**

Log apne app ya website mein password, chaabiyan, ya zaroori niyam daal dete hain, yeh sochkar ki user use dekh nahi sakta.

User sab kuch dekh sakta hai. Woh app ko khol sakta hai, uske andar jhaank sakta hai, aur usmein se nikli har cheez padh sakta hai. Aisa hazaaron baar hua hai, aur aaj bhi roz hota hai.

**Jo cheez user ke device pe hai, woh user ki hai.**

Yeh galti tempting isliye hai ki code padhne mein mushkil dikhta hai, aur log maan lete hain ki mushkil ka matlab namumkin hai. Aur kyunki jab aap khud dekhte ho toh sab theek chalta hai, toh yeh khatra kabhi saamne nahi aata jab tak koi dhoondh na le.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  FRONT / BACK                           │  ← naya
    │  client pe kabhi bharosa mat karo       │
    ├────────────────────────────────────────┤
    │  UPTIME, BADA HONA, KHAALI MACHINE      │
    ├────────────────────────────────────────┤
    │  REPLICA, QUEUE, CACHE, DATABASE        │
    ├────────────────────────────────────────┤
    │  INTERNET, OS, CPU, RAM/DISK, SWITCH    │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek app mein "sirf 18 saal se upar" wali jaanch hai. Woh phone pe hai. Kya problem hai?

> **Jawab:** User use hata sakta hai.
>
> Woh jaanch user ki madad ke liye theek hai, taaki use turant pata chale. Lekin woh suraksha nahi hai.
>
> Agar us jaanch ka kanooni ya karobaari matlab hai, toh woh server pe honi chahiye, jahan user pahunch hi nahi sakta.
>
> Yeh niyam har jagah lagta hai: **jo cheez sach mein zaroori hai, woh wahan honi chahiye jahan user ka haath na pahunche.**

**2. (samajh check)** Ek website pehli baar khulne mein 6 second leti hai lekin uske baad bahut tez chalti hai. Kya ho raha hai?

> **Jawab:** Lagbhag poora page device pe banaya ja raha hai.
>
> Pehli baar poora program utarna padta hai aur chalna padta hai, isliye der lagti hai. Uske baad sab kuch device pe hai, isliye har click turant hai.
>
> Sauda saaf hai: **pehli baar mehngi, baad mein sasti.**
>
> Aur woh sauda kis ke liye theek hai, yeh iss baat pe hai ki log ek baar aakar bahut kaam karte hain, ya ek baar aakar ek cheez dekh kar chale jaate hain. Ek dukaan ke liye ek jawab hai, ek news site ke liye doosra.

**3. (jodne wala)** Chapter 3.4 mein OS har app ko alag rakhta tha, aur app ko poori taakat nahi deta tha. Front aur back ka batwara usse kaise milta hai?

> **Jawab:** Bilkul wahi soch hai, ek parat upar.
>
> OS kehta hai: app ko taakat mat do, use maangne do, aur main tay karunga.
>
> Server kehta hai: user ke device ko taakat mat do, use maangne do, aur main tay karunga.
>
> Dono jagah wahi niyam hai: **jispe aapka control nahi hai, uspe bharosa mat karo.**
>
> Yeh soch aage Book 2 mein phir milegi, jahan ek AI agent ke paas bhi apni koi taakat nahi hoti, aur har cheez kisi na kisi ke through jaati hai.
