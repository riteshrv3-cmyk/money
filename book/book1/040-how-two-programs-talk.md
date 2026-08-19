# Chapter 6.4  [SPINE]
## Do programs aapas mein baat kaise karte hain

---

### Samvaad

**Madhav:** Aapke phone ka app server se data maangta hai. Ab yeh socho: woh kaise maangta hai?

**Kabir:** Chapter 4.4 wala protocol. Woh keh dega ki mujhe yeh chahiye.

**Madhav:** Protocol batata hai ki sandesh ki shakal kya hogi. Lekin yeh kaun tay karta hai ki kya kya maanga ja sakta hai?

**Kabir:** Server wala.

**Madhav:** Aur app banane wale ko kaise pata chalega?

**Kabir:** Server wale ko batana padega.

**Madhav:** Kis shakal mein?

**Kabir:** Ek list. "Yeh yeh cheezein maang sakte ho, aur is tarah maangna."

**Madhav:** Ab agar server wala kal woh list badal de?

**Kabir:** Toh saare app toot jaayenge.

**Madhav:** Kitne app?

**Kabir:** Jo bhi use istemaal kar rahe hain. Ho sakta hai hazaaron.

**Madhav:** Aur woh app kiske hain?

**Kabir:** Doosre logon ke. Doosri companies ke.

**Madhav:** Toh ab server wale ke haath bandh gaye. Woh apni cheez badal nahi sakta.

**Kabir:** Kyunki uspe doosre khade hain.

**Madhav:** Toh kya karega jab use sach mein kuch badalna ho?

**Kabir:** Purana chalta rahe, aur naya alag se de de.

**Madhav:** Dono ek saath, kitne saal?

**Kabir:** Jab tak sab naye pe na aa jaayein. Shayad kabhi na aayein.

**Madhav:** Bas. Ab ek aur baat. Agar doosri companies aapke server se data le sakti hain, toh yeh aapke liye achha hai ya bura?

**Kabir:** Bura. Woh mera data le rahe hain.

**Madhav:** Ya achha. Socho.

**Kabir:** Achha... agar woh mere upar apna kuch banayein toh mere bina unka kaam nahi chalega.

**Madhav:** Aur unke users?

**Kabir:** Woh sab ghoomkar mere paas hi aayenge.

**Madhav:** Toh ek list, jo sirf technical cheez lagti hai, woh kya ban gayi?

**Kabir:** Ek raasta jisse doosre log mere upar khade ho jaate hain.

**Madhav:** Aur us raaste ka maalik kaun hai?

**Kabir:** Main.

**Madhav:** Aur agar main kal woh raasta band kar doon?

**Kabir:** Toh jo log mere upar khade the woh gir jaayenge.

**Madhav:** Yaad rakhna. Yeh aage bahut zaroori hoga.

---

### Naam

Us list ka naam hai **API**: woh tay-shuda tareeka jisse ek program doosre program se baat karta hai.

Farak samajhna zaroori hai:

```
PROTOCOL   sandesh ki shakal kya hogi
           (sabke liye ek, jaise HTTP)

API        kaunse sandesh maangne ki ijaazat hai, aur unka matlab kya hai
           (har service ka apna)
```

Protocol yeh hai ki chitthi kaise likhi jaaye. API yeh hai ki iss daftar mein kaunsi darkhwastein manzoor hoti hain.

Ek API kuch aisa dikhta hai:

```
GET   /users/42            →  us user ki jaankari do
GET   /users/42/messages   →  uske messages do
POST  /messages            →  naya message banao
DELETE /messages/99        →  woh message hata do
```

Aur ab teen baatein jo API ko technical cheez se zyada bana deti hain.

**Ek: API ek waada hai.** Ek baar aapne diya, log uspe khade ho jaate hain. Use badalna unhe todna hai. Isliye badalne ki jagah aksar naya jod diya jaata hai aur purana chalta rehta hai, saalon tak.

**Do: API ek darwaza hai.** Jo aapke API pe kuch banata hai, woh aap pe nirbhar ho jaata hai. Uske users ghoomkar aapke paas aate hain.

**Teen: API ek taala bhi hai.** Jisne darwaza khola hai, woh use band bhi kar sakta hai. Aur jo log uspe khade the, woh gir jaate hain.

Yeh teesri baat ek asli karobaari chaal hai, aur woh baar baar chali gayi hai: pehle darwaza khol do taaki log aa jaayein aur aapke upar cheezein banayein, aur jab woh nirbhar ho jaayein tab shartein badal do.

---

### Asli duniya se ek example

2006 se 2012 tak Twitter ka API lagbhag khula tha. Uske upar hazaaron app bane, aur unmein se kuch Twitter ke apne app se behtar the. Woh khula darwaza hi ek badi wajah tha ki Twitter itna phaila.

Phir shartein sakht hoti gayin. Kitne users ho sakte hain, kya dikhaya jaa sakta hai, kya nahi. 2023 mein API lagbhag poori tarah paid kar diya gaya, aur daam itna rakha gaya ki chhoti cheezein chal hi nahi sakti thin.

Hazaaron app, jo saalon se chal rahe the, kuch hafton mein band ho gaye. Unka code theek tha. Unki machinein chal rahi thin. Bas darwaza band ho gaya.

Yeh Chapter 0.2 ki bhasha mein saaf hai: un app banane walon ka leverage kabhi unka tha hi nahi. Woh kisi aur ke darwaze pe khade the.

Aur yeh yaad rakhne laayak sabak hai: **kisi aur ke API pe banana Anil ki naali banana nahi hai. Woh kisi aur ki naali se paani lena hai.**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **API ko sirf ek technical cheez samajhna.**

Log sochte hain ki API bas ek raasta hai data laane ka, aur uska faisla technical hai.

Woh ek karobaari faisla hai. Kya khola jaaye, kise diya jaaye, kis daam pe, aur kab band kiya jaaye, yeh sab tay hota hai.

Iska seedha nateeja: log poora product kisi aur ke API pe bana dete hain, aur maan lete hain ki woh hamesha rahega. Uske do khatre hain: woh band ho sakta hai, aur woh mehnga ho sakta hai. Dono baar baar hote hain.

Yeh galti tempting isliye hai ki API istemaal karna bahut aasan hai. Ek line likho aur poori taakat mil jaati hai. Woh aasani hi khatra chhupa deti hai.

Sahi sawal, jab bhi aap kisi aur ke API pe kuch banao:

```
agar yeh kal band ho jaaye toh mera kya bachega?
agar iska daam das guna ho jaaye toh?
kya iske jaisa koi doosra hai?
kya main uska hissa hoon ya uska mukabla?
```

Aakhri sawal sabse zaroori hai. Jo log platform ke mukable mein aa jaate hain, unka darwaza sabse pehle band hota hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  API          waada, darwaza, taala     │  ← naya
    ├────────────────────────────────────────┤
    │  FRONT/BACK, UPTIME, BADA HONA          │
    ├────────────────────────────────────────┤
    │  REPLICA, QUEUE, CACHE, DATABASE        │
    ├────────────────────────────────────────┤
    │  INTERNET, PROTOCOL, OS, CPU, SWITCH    │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Aapne ek API banaya aur sau companies use kar rahi hain. Aapko usmein ek galti dikhi jise theek karna hai, lekin theek karne se woh sau toot jaayengi. Kya karoge?

> **Jawab:** Purana chalta rehne do, naya alag se do, aur logon ko waqt do.
>
> Yeh lagbhag hamesha ka jawab hai, aur uski keemat yeh hai ki ab aap do cheezein sambhal rahe ho, shayad saalon tak.
>
> Isiliye API banate waqt sabse zaroori kaam yeh hai ki **kam se kam waada karo.** Har cheez jo aap dikhate ho, woh hamesha ke liye dikhani padegi.
>
> Yeh Chapter 3.3 wali JavaScript ki baat hai: jo cheez phail gayi, use hataya nahi ja sakta.

**2. (samajh check)** Ek company apna API muft aur khula rakhti hai. Chapter 3.6 ke chaar wajahon mein se kaunsi ho sakti hai?

> **Jawab:** Lagbhag hamesha teesri: neeche wali parat pe kabza.
>
> Woh chahte hain ki log unke upar cheezein banayein, kyunki jitne zyada log unpe khade honge, utna hi unhe hataana mushkil hoga.
>
> Muft dena shuruaat hai, seema nahi. Jab kaafi log nirbhar ho jaate hain, tab shartein badalti hain.
>
> Yeh dhokha nahi hai, yeh ek jaani-pehchani chaal hai. Aur ise pehchan lena hi bachaav hai.

**3. (jodne wala)** Chapter 4.4 kehta tha ki jo protocol tay karta hai woh us ilaake ki shakal tay kar deta hai. API ke saath kya farak hai?

> **Jawab:** Bada farak hai, aur wahi asli baat hai.
>
> Protocol kisi ka nahi hota. HTTP ka koi maalik nahi hai, isliye koi use band nahi kar sakta.
>
> API ka maalik hota hai. Woh use kabhi bhi badal ya band kar sakta hai.
>
> Toh dono par khade hone mein zameen aasman ka farak hai:
>
> ```
> protocol pe khade ho   →  koi aapko hata nahi sakta
> API pe khade ho        →  ek company aapko hata sakti hai
> ```
>
> Yeh sabse kaam ki baaton mein se ek hai jo iss kitaab mein hai. Jab bhi kuch banao, poocho: **main kis cheez pe khada hoon, aur uska maalik kaun hai?**
