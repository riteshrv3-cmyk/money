# Chapter 2.7  [SPINE]
## Kya chhoda gaya, aur kyun

### Samvaad

**Madhav:** Web pe sab kuch hai. Kya sab training mein daala jaata hai?

**Kabir:** Shayad nahi. Kuch ganda bhi hoga.

**Madhav:** Toh kaun tay karega ki kya hataana hai?

**Kabir:** Company.

**Madhav:** Kaise? Kharabon pages hain. Kya koi padhega?

**Kabir:** Nahi. Machine se chhaanna padega.

**Madhav:** Machine ko kaise pata chalega ki kya bura hai?

**Kabir:** Kuch niyam banao. Ya ek chhota model train karo jo bataye.

**Madhav:** Aur us chhote model ko kisne sikhaya ki kya bura hai?

**Kabir:** Kisi insaan ne.

**Madhav:** Kitne insaan?

**Kabir:** Kuch sau, shayad.

**Madhav:** Toh kuch sau logon ke faisle kharabon pages pe laga diye jaate hain. Ab yeh dekho: unke faisle kis cheez se aaye?

**Kabir:** Unki apni soch se. Unke desh se, bhasha se, samay se.

**Madhav:** Toh woh chhannan neutral hai?

**Kabir:** Ho hi nahi sakta.

**Madhav:** Ab ek aur cheez. Sirf ganda hi nahi hataya jaata. Aur kya hataya jaata hai?

**Kabir:** Dohrav? Wahi cheez baar baar?

**Madhav:** Bilkul, aur woh bada hissa hai. Ek hi page hazaar jagah copy hua hota hai. Aur agar dohrav na hataya jaaye?

**Kabir:** Toh model use zyada wazan dega. Woh use zyada baar dekhega.

**Madhav:** Aur kya hataya jaata hai?

**Kabir:** Bakwaas. Aise pages jinme kuch likha hi nahi hai, sirf ads.

**Madhav:** Aur ek aur, jo sabse chalak hai. Woh text jo kisi doosre model ne likha ho.

**Kabir:** Woh kyun bura hai?

**Madhav:** Socho. Agar naya model purane model ke likhe pe train ho, toh woh kis cheez ki nakal seekh raha hai?

**Kabir:** Purane model ki galtiyon ki.

**Madhav:** Aur agla model uski?

**Kabir:** Har baar copy ki copy. Dheere dheere sab dhundhla ho jaayega.

**Madhav:** Aur ab web pe AI ka likha hua text kitna hai?

**Kabir:** Bahut, aur badh raha hai.

**Madhav:** Toh ek nayi problem paida ho gayi jo paanch saal pehle thi hi nahi: **saaf, insaan ka likha data ab ek scarce cheez hai.**

**Kabir:** Aur purana web zyada saaf hai.

**Madhav:** 2022 se pehle ka data ab ek aisi cheez hai jo dobara nahi banayi ja sakti.

### Naam

Data ki safai ke chaar bade kaam:

```
1.  DOHRAV HATAO       ek page hazaar jagah copy hai
                       na hataao toh use zyada wazan mil jaayega

2.  BAKWAAS HATAO      khaali pages, sirf ads, tooti hui likhawat
                       aksar poore data ka aadha se zyada

3.  NUKSAAN HATAO      nafrat, hinsa, khatarnak nirdesh
                       yahan koi neutral faisla mumkin nahi hai

4.  MACHINE KA LIKHA HATAO   warna copy ki copy ki copy
```

Chauthe wale ka ek naam bhi pad gaya hai: **model collapse**, jab har agli peedhi pichhli ke likhe pe train hoti hai aur dheere dheere kamzor hoti jaati hai.

Ab do baatein jo yahan se seedhi nikalti hain.

**Ek: safai neutral nahi ho sakti.**

Har hataane ka faisla kisi ka faisla hai. "Nuksaan" ki paribhasha desh, samay aur soch ke saath badalti hai. Kuch sau logon ne tay kiya, aur woh faisla kharabon pages pe laga diya gaya.

Yeh galti nahi hai, kyunki kuch na chunna bhi ek chunav hai. Aur yeh chhupa hua bhi nahi rehna chahiye. **Har model ke andar kisi ke faisle hain, aur woh faisle aapko nahi dikhte.**

**Do: jo hataya gaya woh model ki seema ban jaata hai.**

Agar kisi vishay ko safai ne kaat diya, toh model us vishay pe kamzor rahega, chahe woh vishay poori tarah jaayaz ho. Dawa, sehat, kanoon aur sex se judi jaayaz baatein aksar iss chhannan mein pis jaati hain.

Toh model ki kamzori ke ab teen alag kaaran ho gaye:

```
duniya mein woh cheez kam likhi gayi   (Ch 2.6)
nichodne mein woh gayab ho gayi        (Ch 2.3)
safai ne use jaan-boojh ke kaat diya   (yeh chapter)
```

Bahar se teeno ek jaise dikhte hain: model ko woh cheez nahi pata.

### Asli duniya se

Common Crawl ek public jaal hai jo saalon se web ko ikattha karta hai. Woh lagbhag har bade model ke data mein kisi na kisi shakal mein hai.

Uska kachcha roop lagbhag bekaar hai: usmein tooti hui pages, dohrav, aur bahut sara kachra hai. Har company use apne tareeke se chhaanti hai, aur woh chhannan hi unka ek bada raaz hota hai.

Do companies ek hi kachcha data le sakti hain aur bilkul alag model bana sakti hain, sirf chhannan ke faislon se.

Yeh dhyaan dene laayak hai: **model ka bada hissa us data mein hai jo dikhaya nahi jaata, aur uska bada hissa un faislon mein hai jo likhe nahi jaate.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki model "poora internet" jaanta hai.**

Woh internet ka ek chhaana hua, saaf kiya hua, kaante gaye hisse wala roop jaanta hai, ek tarikh tak, aur usmein se bhi sirf patterns.

Doosri galti: **safai ko sirf achhi cheez samajhna.**

Safai zaroori hai. Uske bina model bakwaas aur nuksaan dohrayega.

Aur wahi safai model ki seemayein bhi banati hai, aur unmein kuch seemayein galat jagah pe hoti hain. Jab model kisi bilkul jaayaz sawal pe ruk jaata hai, toh aksar wajah yahi hoti hai, ya uske baad wali parat (Chapter 2.8).

**Dono baatein ek saath sach hain: safai ke bina model kharaab hota, aur safai ke saath usmein kisi aur ke faisle bhare hue hain.**

### Sochne ke liye

**1. (samajh check)** Model kisi bilkul saadhaaran medical sawal pe jawab dene se mana kar deta hai. Teen alag wajahein ho sakti hain. Batao.

> **Jawab:**
>
> **Ek:** us vishay ka data safai mein kaat diya gaya, isliye woh us pe kamzor hai (yeh chapter).
>
> **Do:** uske baad ek aur parat lagayi gayi jo use aise vishayon pe rokti hai (agla chapter).
>
> **Teen:** product ke upar ek alag filter hai, model ke bahar, jo jawab ko rok deta hai.
>
> Teeno bahar se ek jaise dikhte hain aur teeno ke ilaaj alag hain. Aur aapko yeh kabhi nahi bataya jaata ki kaunsa laga.

**2. (samajh check)** AI ka likha text web pe badh raha hai. Iska naye models pe kya asar hoga?

> **Jawab:** Naya saaf data mehnga hota jaayega.
>
> Kyunki ab web se utha hua data mein AI ka likha mila hua hai, aur uspe train karna copy ki copy banana hai.
>
> Do nateeje dikh rahe hain: 2022 se pehle ke data ki keemat badh gayi hai, aur companies ab aise data ke liye paise de rahi hain jo pakka insaan ka likha hai.
>
> **Ek muft cheez scarce ban rahi hai, humari aankhon ke saamne.** Book 1 Ch 0.2 ke hisaab se, yeh batata hai ki taakat kahan khisak rahi hai.

**3. (jodne wala)** Chapter 2.4 mein tha ki "jo aap naapte ho wahi milta hai." Safai us baat ka kaunsa roop hai?

> **Jawab:** Safai woh cheez hai jo loss naap hi nahi sakti.
>
> Loss sirf yeh naapta hai ki agla token kitni achhi tarah guess hua. Woh yeh nahi naap sakta ki text nuksaandeh hai, ya jhoota hai, ya bakwaas hai.
>
> Toh woh cheezein pehle hi hata di jaati hain, training se pehle.
>
> **Yaani safai bhi ek tarah ka lakshya hai, bas woh formula mein nahi likha, data mein likha gaya.** Aur agla chapter ek teesra tareeka batata hai: training ke baad insaan se seedha sikhana.
