# Chapter 5.2  [SPINE]
## Ek crore mein se ek dhoondna

---

### Samvaad

**Madhav:** Ek kitaab hai, hazaar page ki. Usmein ek shabd dhoondhna hai. Kya karoge?

**Kabir:** Pehle page se padhna shuru karunga.

**Madhav:** Aurat se kitne page padhne padenge?

**Kabir:** Aadhe, aam taur pe. Paanch sau.

**Madhav:** Ab wahi kitaab, lekin peeche ek index hai. Ab?

**Kabir:** Index mein shabd dhoondhunga, woh page number dega, main seedha wahan jaunga.

**Madhav:** Index mein dhoondhne mein kitna waqt?

**Kabir:** Woh alphabet mein hai, toh jaldi.

**Madhav:** Kitni jaldi? Socho. Index mein das hazaar shabd hain. Tum beech mein khologe.

**Kabir:** Agar mera shabd usse pehle hai toh aadha index gaya. Phir uske beech mein.

**Madhav:** Har kadam pe kitna bachta hai?

**Kabir:** Aadha.

**Madhav:** Das hazaar se ek tak pahunchne mein kitne kadam?

**Kabir:** Baar baar aadha... das hazaar, paanch hazaar, dhai hazaar... lagbhag chaudah kadam.

**Madhav:** Aur bina index ke paanch hazaar kadam. Ab isse bada karo. Das lakh cheezein.

**Kabir:** Bina index: paanch lakh kadam. Index se... bees kadam ke aas-paas.

**Madhav:** Das crore?

**Kabir:** Bina index: paanch crore. Index se sattaais, attaais kadam.

**Madhav:** Dhyaan do. Data das hazaar guna bada hua aur index wale kadam chaudah se sattaais ho gaye. Data lakhon guna badhta hai aur kaam mushkil se dugna hota hai.

**Kabir:** Yeh toh bahut bada farak hai.

**Madhav:** Yeh sabse bade farakon mein se ek hai jo poore computer ki duniya mein hai. Ab agla sawal. Agar index itna achha hai, toh har cheez ka index kyun nahi bana lete?

**Kabir:** Bana lo.

**Madhav:** Index kahan rakha jaayega?

**Kabir:** Disk pe. Woh bhi jagah lega.

**Madhav:** Aur jab ek nayi cheez jodi jaaye?

**Kabir:** Index mein bhi jodni padegi.

**Madhav:** Aur agar das index hain?

**Kabir:** Toh das jagah jodna padega. Har baar likhne mein das guna kaam.

**Madhav:** Toh index kya deta hai aur kya leta hai?

**Kabir:** Padhna tez karta hai, likhna dheema karta hai. Aur jagah leta hai.

**Madhav:** Ab batao, kaunse cheezon ka index banaoge?

**Kabir:** Jinse main sach mein dhoondhta hoon.

**Madhav:** Aur jinse kabhi nahi dhoondhta?

**Kabir:** Unka index bekaar hai. Sirf nuksaan hai.

---

### Naam

Us peeche wali list ka naam hai **index**.

Aur woh tareeka jismein har kadam pe aadha hissa chhod diya jaata hai, use **binary search** kehte hain, aur database uska ek bada roop istemaal karte hain jise **B-tree** kehte hain.

Sabse zaroori tasveer:

```
cheezein        bina index         index ke saath
─────────────────────────────────────────────────
1,000           ~500 kadam         ~10 kadam
10 lakh         ~5,00,000          ~20 kadam
10 crore        ~5,00,00,000       ~27 kadam
1 arab          ~50 crore          ~30 kadam
```

Baayan column data ke saath badhta hai. Daayan column lagbhag badhta hi nahi.

Yeh farak itna bada hai ki iske bina aaj ki koi bhi badi cheez chal hi nahi sakti. Google, bank, ticket, sab isi ek hisaab pe khade hain.

Aur uska sauda, jo Kabir ne nikaala:

```
INDEX DETA HAI       padhna lagbhag turant
INDEX LETA HAI       har likhne pe extra kaam
                     aur disk pe jagah
```

Isliye ek aisa system jismein bahut padha jaata hai aur kam likha jaata hai, usmein bahut index hote hain. Aur jismein har second lakhon cheezein likhi jaati hain, usmein bahut kam.

---

### Asli duniya se ek example

Ek chhoti company ka app theek chalta hai jab uske paas das hazaar users hain. Woh badhta hai, aur ek din das lakh pe pahunch kar sab kuch dheema ho jaata hai.

Yeh sabse aam kahani hai jo har badhne wale product mein hoti hai, aur uski wajah lagbhag hamesha yehi hoti hai: kahin ek jagah poori list padhi ja rahi thi.

Das hazaar par woh 5,000 kadam the, jo itne tez the ki kisi ko dikha hi nahi. Das lakh par woh 5,00,000 kadam ho gaye.

Kuch nahi badla. Code wahi hai. Machine wahi hai. Sirf data bada ho gaya, aur ek aisa hissa jo badhne ke saath badhta tha, woh saamne aa gaya.

Isiliye yeh sawal hamesha poocha jaata hai: **jab yeh cheez sau guna badi hogi, tab kya hoga?** Kuch cheezein badhne pe wahi rehti hain, kuch dugni ho jaati hain, aur kuch sau guna. Farak wahin se aata hai.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki dheema hone ka ilaaj badi machine hai.**

Jab kuch dheema hota hai toh pehla khayal aata hai: bada server le lo.

Lekin agar aapka kaam data ke saath seedha badhta hai, toh dugni machine sirf dugna sambhalegi. Aur data das guna hone wala hai.

Index badalne se kaam **paanch lakh kadam se bees kadam** ho jaata hai. Koi machine woh farak nahi de sakti.

Yeh galti tempting isliye hai ki machine khareedna ek din ka kaam hai aur samajhna ki dheema kyun hai, woh mehnat hai. Aur kyunki machine badhane se thoda faayda hota bhi hai, toh lagta hai ki disha sahi thi.

Sahi soch:

```
pehle poocho    yeh kaam data ke saath kaise badhta hai?
                lagbhag wahi rehta hai, ya seedha badhta hai?
phir poocho     kya main use badalne ka tareeka badal sakta hoon?
aakhir mein     kya mujhe badi machine chahiye?
```

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  INDEX        har kadam pe aadha chhodo │  ← naya
    │               padhna tez, likhna dheema │
    ├────────────────────────────────────────┤
    │  DATABASE     chaar problem             │
    ├────────────────────────────────────────┤
    │  INTERNET, PROTOCOL, PATA               │
    ├────────────────────────────────────────┤
    │  OS, CPU, RAM/DISK, SWITCH              │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek app hai jismein har second das hazaar naye messages aate hain, aur log unhe kabhi kabhi dhoondhte hain. Bahut index rakhoge ya kam?

> **Jawab:** Kam. Sirf woh jo sach mein chahiye.
>
> Har index har likhne pe kaam badhata hai. Das hazaar likhne per second, das index, matlab ek lakh extra kaam har second.
>
> Padhna kam hai, toh index ka faayda kam baar milta hai aur nuksaan har baar.
>
> Ulta case: ek aisi jagah jahan data raat mein ek baar aata hai aur din bhar log dhoondhte hain. Wahan jitne index chaho.

**2. (samajh check)** Index se dhoondhna itna tez hai. Toh phir kuch cheezein aaj bhi dheemi kyun hain?

> **Jawab:** Kyunki index tabhi kaam karta hai jab aap **usi cheez se** dhoondho jiska index bana hai.
>
> Naam ka index hai aur aap naam se dhoondhoge toh turant. Aap tarikh se dhoondhoge toh index bekaar hai, poori list padhni padegi.
>
> Aur kuch sawal aise hain jinka index ban hi nahi sakta. "Aisa har message dhoondho jismein kahin bhi yeh shabd ho" ek mushkil sawal hai, aur uske liye alag tarah ka index banana padta hai.
>
> Yeh Book 2 mein wapas aayega. Wahan aap dekhoge ki "matlab se dhoondhna" ek bilkul nayi tarah ka index maangta hai.

**3. (jodne wala)** Chapter 2.3 kehta tha ki hisaab sasta hai aur data laana mehnga. Index uss baat se kaise judta hai?

> **Jawab:** Index ka poora kaam hi yeh hai ki **kam data laana pade**.
>
> Woh hisaab nahi bachata. Woh yeh bachata hai ki disk se kitne tukde uthane padenge.
>
> Bina index: das lakh cheezein disk se uthao aur dekho.
>
> Index ke saath: bees tukde uthao, phir seedha sahi jagah jao.
>
> Toh index ek hisaab ka jugaad nahi hai. Woh doori ka jugaad hai. Aur wahi wajah hai ki uska faayda itna bada hai.
