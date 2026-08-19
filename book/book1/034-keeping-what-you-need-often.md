# Chapter 5.5  [SPINE]
## Jo baar baar chahiye use paas rakhna

---

### Samvaad

**Madhav:** Ek website ka home page hai. Ek second mein das hazaar log use kholte hain. Har baar database se poora data laaya jaata hai. Problem?

**Kabir:** Das hazaar baar wahi kaam. Bekaar.

**Madhav:** Kya karoge?

**Kabir:** Ek baar laao aur rakh lo. Agli baar wahi de do.

**Madhav:** Rakhoge kahan?

**Kabir:** RAM mein. Woh tez hai.

**Madhav:** Kitna tez? Chapter 2.3 se yaad karo.

**Kabir:** RAM lagbhag 200 kadam, disk das lakh. Toh paanch hazaar guna.

**Madhav:** Ab problem batao.

**Kabir:** Agar database mein data badal jaaye toh mera rakha hua purana ho jaayega.

**Madhav:** Toh kya karoge?

**Kabir:** Jab data badle tab rakha hua hata dun.

**Madhav:** Aur agar data das jagah rakha hai, das alag machinon pe?

**Kabir:** Toh das jagah hatana padega. Aur kisi ek pe na hata toh woh purana deta rahega.

**Madhav:** Aur agar tumhe pata hi na ho ki data badla?

**Kabir:** Toh main hamesha purana deta rahunga.

**Madhav:** Toh ek doosra tareeka socho. Sochne mein aasan.

**Kabir:** Waqt lagao. Paanch minute baad apne aap phenk do, chahe badla ho ya nahi.

**Madhav:** Ab uski keemat kya hai?

**Kabir:** Paanch minute tak log purana dekh sakte hain.

**Madhav:** Toh do tareeke hain: badalne pe hatao, ya waqt pe hatao. Pehla sahi hai lekin mushkil. Doosra aasan hai lekin thoda purana deta hai.

**Kabir:** Aur teesra? Dono?

**Madhav:** Aksar dono. Ab aakhri problem. RAM chhoti hai. Sab kuch usmein nahi aayega. Kya phenkoge?

**Kabir:** Jo sabse kam istemaal ho raha hai.

**Madhav:** Kaise pata chalega?

**Kabir:** Yaad rakhunga ki kis cheez ko aakhri baar kab maanga gaya. Sabse purani phenk dunga.

**Madhav:** Bas. Ab ek aakhri baat. Cache mein cheez na mile toh?

**Kabir:** Toh database se laani padegi. Yaani woh baar dheemi.

**Madhav:** Toh cache se hamesha faayda hota hai?

**Kabir:** Nahi. Agar har baar naya sawal aaye aur cache mein kabhi kuch na mile, toh cache sirf extra kaam hai.

**Madhav:** Toh cache kis cheez pe chalta hai?

**Kabir:** Iss baat pe ki wahi cheez baar baar maangi jaaye.

**Madhav:** Aur agar na maangi jaaye?

**Kabir:** Toh cache bekaar hai.

---

### Naam

Us paas rakhi hui copy ko **cache** kehte hain.

```
CACHE HIT     maangi hui cheez cache mein mil gayi. Tez.
CACHE MISS    nahi mili. Ab asli jagah se laani padegi. Dheemi + extra kaam.

HIT RATE      sau sawalon mein se kitne cache se mile
```

Cache kab phenka jaaye, uske do tareeke:

```
WAQT SE       paanch minute baad apne aap. Aasan, thoda purana de sakta hai.
BADLAV SE     jab asli data badle tab hatao. Sahi, lekin har jagah hatana padta hai.
```

Aur jab jagah bhar jaaye toh kya phenkein: aksar woh jo sabse lambe waqt se kisi ne nahi maanga.

Ab woh sabse zaroori baat, jise ek line mein rakh lo:

**Cache tez isliye hai kyunki woh purana ho sakta hai. Woh do alag cheezein nahi hain. Woh ek hi cheez hai.**

Agar cache kabhi purana na ho, toh use har baar jaanch karni padegi ki data badla ya nahi, aur phir woh cache hai hi nahi.

Isiliye har cache ke saath yeh sawal aata hai: **kitna purana chalega?** Share bazaar ke daam mein: ek second bhi nahi. Ek news article mein: paanch minute theek hai. Ek company ke "About Us" page mein: ek din bhi chalega.

Aur cache sirf ek jagah nahi hota. Aapke ek sawal ke raaste mein aksar chaar-paanch cache hote hain, aur unmein se koi bhi purana de sakta hai.

```
aapka browser         →  cache
raaste ka CDN         →  cache
server ki RAM         →  cache
database ki RAM       →  cache
CPU ki cache          →  cache (Chapter 2.3)
```

Isiliye "refresh karo, chal jaayega" itni baar kaam karta hai. Aap ek cache ko chhod kar aage ki taraf poochh rahe ho.

---

### Asli duniya se ek example

Jab aap koi video dekhte ho, woh aksar us company ke asli server se nahi aata. Woh aapke sheher ya aapke desh mein rakhi ek copy se aata hai.

Aisi copiyon ke jaal ko **CDN** kehte hain. Duniya bhar mein hazaaron jagah, popular cheezein pehle se rakhi hui.

Wajah Chapter 4.3 se aati hai: bandwidth badhayi ja sakti hai, latency nahi. Roshni se tez kuch nahi ja sakta. Agar video doosre mahadweep se aayega toh ek chakkar mein 200 millisecond lagenge, chahe sadak kitni bhi chaudi ho.

Toh hal doori kam karna hai, aur uska ek hi tareeka hai: cheez ko paas rakh do.

Aur iska ek gehra nateeja hai. **Internet ka bahut bada hissa asal mein cache hai.** Aap jo dekhte ho uska bada hissa asli jagah se nahi aata. Woh kisi copy se aata hai jo aapke paas rakhi hai.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **cache ko sirf ek speed ka jugaad samajhna.**

Log sochte hain cache lagane se cheez tez ho jaayegi, bina kisi keemat ke.

Keemat purana data hai, aur woh keemat hamesha chukani padti hai. Cache ka poora matlab hi yeh hai ki aap asli jagah se nahi pooch rahe.

Iska seedha nateeja: log ghanton yeh dhoondhte hain ki unka badlav dikh kyun nahi raha, jabki unhone data theek badal diya tha. Woh kisi cache mein atka hua hai, aur aksar unhe pata bhi nahi hota ki woh cache maujood hai.

Ek purani kahavat hai ki computer science mein sirf do mushkil cheezein hain: cache ko kab hataya jaaye, aur cheezon ke naam rakhna. Woh mazaak hai, lekin pehli baat sach hai.

Aur ek doosri galti isi ke saath aati hai: har jagah cache laga dena. Agar hit rate kam hai toh cache sirf nuksaan hai. Woh jagah leta hai, kaam badhata hai, aur purana data deta hai, sab bina kisi faayde ke.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  CACHE        paas rakhi copy           │  ← naya
    │               tez = purana ho sakta hai │
    │               ek hi sikke ke do pehlu   │
    ├────────────────────────────────────────┤
    │  TRANSACTION, SHAKAL, INDEX, DATABASE   │
    ├────────────────────────────────────────┤
    │  INTERNET, OS, CPU, RAM/DISK, SWITCH    │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek site pe har user ka apna alag page hai, aur har user din mein ek baar aata hai. Cache lagane se kya hoga?

> **Jawab:** Lagbhag kuch nahi, aur thoda nuksaan.
>
> Har sawal alag hai, toh cache mein kabhi kuch nahi milega. Hit rate lagbhag zero.
>
> Aur har baar cache mein daalne ka extra kaam hoga, aur RAM bhi bharegi.
>
> Cache **dohrav** pe chalta hai, bilkul waise jaise compression (Chapter 2.1). Dohrav nahi, toh faayda nahi.
>
> Yeh poochna hamesha pehla kadam hai: **kya wahi cheez baar baar maangi ja rahi hai?**

**2. (samajh check)** Aapne apni website ka logo badla lekin purana hi dikh raha hai. Kya kya ho sakta hai?

> **Jawab:** Raaste mein kisi bhi cache mein purana atka hai.
>
> Aapka browser, ya CDN, ya server ki apni copy.
>
> Isiliye website banane wale aksar file ke naam mein ek number jod dete hain, jaise `logo-v2.png`. Naya naam matlab naya sawal, aur kisi cache mein woh hai hi nahi.
>
> Yeh ek achhi chaal hai: **cache ko hatane ki koshish mat karo, use chakma do.**

**3. (jodne wala)** Chapter 4.5 mein DNS ke jawab bhi kuch ghante ke liye rakhe jaate the. Woh bhi cache tha. Dono mein saanjha kya hai?

> **Jawab:** Dono mein wahi sauda hai, aur wahi problem.
>
> DNS mein: pata paas rakh lo, tez ho jao, aur jab pata badle toh kuch ghante purana chalta rahe.
>
> Yahan: data paas rakh lo, tez ho jao, aur jab data badle toh kuch der purana chalta rahe.
>
> Aur dono mein wahi hal hai: waqt ki seema chhoti kar do badlav se pehle.
>
> Yeh iss kitaab ki ek badi baat hai: **jab aap ek shakal pehchan lete ho, toh woh har jagah dikhne lagti hai.** Cache CPU mein hai, DNS mein hai, browser mein hai, database mein hai. Ek hi soch, chhe jagah.
