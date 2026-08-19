# Chapter 2.1  [SPINE]
## Rules ya examples

### Samvaad

**Madhav:** Book 1 mein humne dekha ki program nirdeshon ki list hai. Ek insaan likhta hai: agar yeh, toh woh. Ab main aapko ek kaam deta hoon. Aisa program likho jo bataye ki ek number even hai ya odd.

**Kabir:** Aasan. Do se bhaag do, bacha kuch toh odd.

**Madhav:** Kitni lines?

**Kabir:** Ek.

**Madhav:** Ab doosra kaam. Aisa program likho jo bataye ki ek email spam hai ya nahi.

**Kabir:** Kuch shabd dekh lo. "Lottery", "free", "click here".

**Madhav:** Achha. Ab spam bhejne wala "free" ki jagah "fr33" likh deta hai.

**Kabir:** Toh woh bhi list mein daal do.

**Madhav:** Aur "f r e e"?

**Kabir:** Woh bhi.

**Madhav:** Aur kal woh kuch naya likhega?

**Kabir:** Toh main woh bhi jodunga.

**Madhav:** Kab tak?

**Kabir:** Hamesha. Yeh kabhi khatam nahi hoga.

**Madhav:** Aur aapki maa aapko likhti hai ki "beta free time mein call karna," toh?

**Kabir:** Woh spam mein chala jaayega.

**Madhav:** Toh aap aur shartein jodoge. Aur woh shartein aapas mein takraayengi. Ab teesra kaam. Aisa program likho jo bataye ki photo mein billi hai ya nahi.

**Kabir:** Kaan dekh lo. Nukeele kaan.

**Madhav:** Kaan kis rang ka hai?

**Kabir:** Koi bhi rang.

**Madhav:** Kis jagah pe?

**Kabir:** Photo mein kahin bhi.

**Madhav:** Kitne bade?

**Kabir:** Kuch bhi.

**Madhav:** Aur billi peeche se dikhi ho? Ya sirf aadhi dikhe? Ya andhere mein ho?

**Kabir:** Yeh toh likha hi nahi ja sakta.

**Madhav:** Kyun nahi? Aap billi pehchan lete ho. Aapke andar toh koi tareeka hai.

**Kabir:** Hai, lekin main use bata nahi sakta.

**Madhav:** Ab ruko. Yeh ek bahut zaroori baat hai. **Aap woh kaam kar sakte ho jise aap likh nahi sakte.**

**Kabir:** Haan.

**Madhav:** Aur ek program woh kaam nahi kar sakta jise koi likh na sake.

**Kabir:** Toh phir aaj ki cheezein billi kaise pehchanti hain?

**Madhav:** Yehi sawal hai. Do raaste hain aur ab tak humne sirf ek dekha hai. Doosra kya ho sakta hai? Aapne billi kaise seekhi thi?

**Kabir:** Kisi ne mujhe billi dikhayi hogi. Bachpan mein. Kai baar.

**Madhav:** Kisi ne aapko niyam bataye the?

**Kabir:** Nahi. Bas billi dikhayi thi aur kaha tha "yeh billi hai."

**Madhav:** Kitni baar?

**Kabir:** Bahut baar.

**Madhav:** Toh doosra raasta kya hai?

**Kabir:** Niyam mat batao. Examples dikhao. Bahut saare.

**Madhav:** Aur machine unse kya banayegi?

**Kabir:** Apne niyam? Jo woh khud nikaal le?

**Madhav:** Aur kya woh niyam koi padh paayega?

**Kabir:** Shayad nahi. Mere andar wale niyam bhi koi nahi padh sakta.

**Madhav:** Bas. Ab aapko poori Book 2 ki shakal dikh gayi.

### Naam

Do hi tareeke hain machine se kaam karwane ke, aur sirf do:

```
RULES SE
├── insaan niyam likhta hai
├── niyam padhe ja sakte hain, badle ja sakte hain, samjhaye ja sakte hain
├── galti ho toh pata chal jaata hai ki kaunsa niyam galat tha
└── kaam nahi karta jab niyam likhe hi na ja sakein

EXAMPLES SE
├── insaan examples deta hai, niyam nahi
├── machine khud kuch banati hai
├── woh cheez padhi nahi ja sakti
├── galti ho toh pata nahi chalta ki kyun
└── kaam karta hai wahan jahan niyam likhe hi nahi ja sakte
```

Doosre tareeke ka naam hai **machine learning**.

Ab ek line jo iss poori kitaab ki neev hai:

> **Doosra tareeka isliye nahi bana ki woh behtar hai. Woh isliye bana ki kuch kaam pehle tareeke se ho hi nahi sakte.**

Yeh dhyaan mein rakhna, kyunki iska ulta bhi sach hai: **jahan niyam likhe ja sakte hain, wahan niyam behtar hain.**

Niyam sasta hai, tez hai, samjhaya ja sakta hai, aur galti hone pe theek kiya ja sakta hai. Ek even-odd wala program ML se banana bewakoofi hogi.

Aur uski keemat bhi saaf hai. Jo cheez examples se bani hai, woh:

```
padhi nahi ja sakti      andar sirf numbers hain
samjhayi nahi ja sakti   "yeh spam kyun hai" ka jawab nahi milta
pakki nahi hoti          woh aksar sahi hoti hai, hamesha nahi
apne data jaisi hoti hai jo dikhaya gaya, wahi seekha gaya
```

Aakhri wali sabse zyada mayne rakhti hai, aur Chapter 2.7 aur 2.8 usi pe hain.

### Asli duniya se

1959 mein Arthur Samuel ne ek program likha jo checkers khelta tha. Uski khaas baat yeh thi ki usne apne banane wale ko harana shuru kar diya.

Samuel checkers mein bahut achha nahi tha. Usne program ko yeh nahi sikhaya ki achhi chaal kya hoti hai. Usne use khud ke khilaaf hazaaron game khilaye aur har game ke nateeje se use apne andar ke numbers badalne diye.

Program ne woh seekha jo Samuel jaanta hi nahi tha.

Yeh 1959 hai. Idea purana hai. Jo naya hai woh yeh hai ki ab hamare paas woh do cheezein hain jo tab nahi thin: bahut saara data, aur bahut saari machine. Book 1 Chapter 2.2 wali baat, phir se: **idea pehle se tha, paimana baad mein aaya.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki ML har problem ke liye behtar hai.**

Bahut si companies aisi cheezon pe ML lagati hain jinke liye das lines ka niyam kaafi hota. Nateeja: mehnga, dheema, samjhaya na ja sakne wala, aur us niyam se kam bharosemand jo woh replace kar raha tha.

Sahi sawal ek hi hai: **kya main is kaam ke niyam likh sakta hoon?**

```
haan, aur woh niyam sthir hain    →  niyam likho
haan, lekin woh hazaaron hain     →  shayad ML
nahi, koi likh hi nahi sakta      →  ML, ya kuch nahi
```

Doosri galti, ulti taraf se: **yeh sochna ki ML jaadu hai jo kisi bhi problem ko hal kar dega.**

Woh us data se bandha hua hai jo use dikhaya gaya. Agar us data mein jawab nahi hai, toh model mein bhi nahi hoga. Yeh Chapter 2.7 ka poora vishay hai.

### Sochne ke liye

**1. (samajh check)** In teen kaamon ko baanto: (a) GST ka hisaab, (b) ek awaaz se aadmi pehchanna, (c) tarikh ki shakal jaanchna.

> **Jawab:** (a) aur (c) niyam hain. (b) ML hai.
>
> GST ka hisaab ek formula hai, aur woh kanoon mein likha hai. Use ML se karna galat hoga: aap ek pakki cheez ko andaza bana denge.
>
> Tarikh ki shakal jaanchna bhi ek niyam hai, chahe woh thoda ulajha hua ho.
>
> Awaaz se aadmi pehchanne ke niyam koi nahi likh sakta. Aap khud pehchanate ho aur bata nahi sakte kaise.
>
> **Yeh sawal har naye kaam pe poochna chahiye, aur uska jawab aksar "niyam" hota hai.**

**2. (samajh check)** Ek spam filter ML se banaya gaya aur woh aapki maa ka email spam mein daal deta hai. Aap wajah kaise dhoondhoge?

> **Jawab:** Yeh mushkil hai, aur wahi ML ki asli keemat hai.
>
> Niyam wale system mein aap dekh lete ki kaunsa niyam laga. Yahan koi niyam hai hi nahi, sirf numbers hain.
>
> Jo kiya ja sakta hai: usse milte-julte examples dhoondho aur dekho ki unka kya hota hai. Ek-ek shabd hata kar dekho ki kab faisla badalta hai. Yaani aap bahar se prayog kar rahe ho, andar padh nahi rahe.
>
> Isiliye jahan "kyun" ka jawab dena zaroori hai, wahan ML pe sawal uthta hai: loan mana karna, naukri se hataana, ilaaj tay karna.

**3. (jodne wala)** Book 1 Ch 1.6 kehta tha ki machine har woh kaam kar sakti hai jiske liye nirdesh likhe ja sakein. ML us baat ko todta hai ya nahi?

> **Jawab:** Nahi todta, aur yeh dekhna dilchasp hai.
>
> ML mein bhi nirdesh likhe gaye hain. Bas woh nirdesh yeh nahi hain ki "billi kaise pehchano." Woh nirdesh yeh hain ki "examples dekh kar apne numbers kaise badlo."
>
> Yaani insaan ne **seekhne ka tareeka** likha, kaam nahi.
>
> Aur woh tareeka bhi ek program hai, jise koi padh sakta hai. Jo padha nahi ja sakta woh nateeja hai, tareeka nahi.
>
> Book 1 ka niyam bacha hua hai: **jiske liye nirdesh likhe ja sakein.** Bas nirdesh ek parat upar chale gaye.
