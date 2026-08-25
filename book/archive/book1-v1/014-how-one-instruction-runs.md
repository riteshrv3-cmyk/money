# Chapter 2.3  [DEPTH]
## Ek instruction chalti kaise hai

---

*DEPTH chapter. Yahan aap dekhoge ki "program chal raha hai" ka asli matlab kya hai. Chhod sakte ho, lekin iske baad "computer dheema ho gaya" jaisi baat pehli baar samajh mein aati hai.*

---

### Samvaad

**Madhav:** Chapter 1.6 mein tumne kaha tha ki program bhi numbers hain, aur machine unhe "karti" hai. Ab batao, karti kaise hai?

**Kabir:** Pata nahi. Padhti hogi aur kar deti hogi.

**Madhav:** Chalo ek insaan se samjhte hain. Tum ek rasoiye ho. Tumhe ek parchi milti hai jispe likha hai: "pyaaz kaato." Tum kya karte ho, kadam ke hisaab se?

**Kabir:** Parchi uthata hoon. Padhta hoon. Phir kaatta hoon.

**Madhav:** Aur agli parchi?

**Kabir:** Woh uthata hoon.

**Madhav:** Toh teen kadam hain, baar baar. **Uthao, samjho, karo.** Machine bilkul yehi karti hai. Ab thoda gehra chalte hain. Parchiyan rakhi kahan hain?

**Kabir:** Ek dher mein.

**Madhav:** Aur tumhe kaise pata ki agli kaunsi hai?

**Kabir:** Main upar wali uthata hoon. Ya... mujhe yaad rehta hai ki main kahan tak pahuncha.

**Madhav:** Machine ke paas yaaddasht nahi hoti. Uske paas ek chhota khaana hota hai jismein likha hota hai: "abhi main nirdesh number 47 pe hoon." Kaam khatam, toh usmein 48 likh deti hai.

**Kabir:** Toh woh khaana ek ginti karne wala hai.

**Madhav:** Bas. Ab ek aur cheez. Tum pyaaz kaat rahe ho. Pyaaz kahan hai?

**Kabir:** Mere haath mein. Ya saamne ke plate mein.

**Madhav:** Aur baaki saara saaman?

**Kabir:** Almari mein, peeche.

**Madhav:** Kyun saamne nahi rakhte sab?

**Kabir:** Jagah nahi hai. Aur zaroorat bhi nahi.

**Madhav:** Machine mein bhi wahi hai. Uske paas kuch bahut chhote khaane hote hain, ekdam paas mein, jismein sirf woh numbers rehte hain jinpe abhi kaam ho raha hai. Baaki sab door rakha hota hai.

**Kabir:** Kitne chhote khaane?

**Madhav:** Aam taur pe solah se kuch dozen. Har ek mein ek number.

**Kabir:** Sirf itne? Bees arab transistor hain aur khaane sirf solah?

**Madhav:** Yehi baat samajhne laayak hai. Bees arab transistor kaam **karne** mein lagte hain, rakhne mein nahi. Rakhna alag jagah hota hai, aur woh door hoti hai.

**Kabir:** Door matlab kitni door?

**Madhav:** Chip ke andar hi, lekin chip ke hisaab se door. Aur ab sabse zaroori baat: **door se laane mein waqt lagta hai.** Ek nirdesh chalane mein ek kadam lagta hai. Door se ek number uthane mein sau kadam lag sakte hain.

**Kabir:** Sau guna?

**Madhav:** Aur agar woh number aur bhi door ho, disk pe, toh das lakh kadam.

**Kabir:** Toh machine ka zyadatar waqt...

**Madhav:** Intezaar mein jaata hai. Chip khaali baithi rehti hai, number ke aane ka intezaar karti hui.

**Kabir:** Yeh toh bekaar hai. Kuch kiya nahi jaa sakta?

**Madhav:** Bahut kuch kiya jaata hai, aur poora Chapter 2.4 usi pe hai. Abhi bas yeh pakad lo: machine ki asli seema uski speed nahi hai. Uski seema yeh hai ki number use time pe milte hain ya nahi.

---

### Naam

Woh teen kadam, baar baar, unka naam hai **fetch, decode, execute**. Uthao, samjho, karo.

Woh ginti wala khaana jo batata hai ki abhi kaunsa nirdesh chal raha hai, use **program counter** kehte hain.

Woh chhote khaane jo ekdam paas hain, unhe **registers** kehte hain.

Aur woh poora hissa jo yeh sab karta hai, use **CPU** kehte hain, yaani woh jagah jahan nirdesh chalte hain.

Ab poori tasveer:

```
    ┌──────────────────────────────────────────────┐
    │  CPU                                         │
    │                                              │
    │   program counter:  "abhi nirdesh 47 pe"     │
    │                                              │
    │   registers:  [ 12 ][ 5 ][ 0 ][ 99 ] ...     │  ekdam paas
    │                                              │
    │   yahan jod, ghatao, tulna hoti hai          │
    └───────────────────┬──────────────────────────┘
                        │  yahan waqt lagta hai
    ┌───────────────────┴──────────────────────────┐
    │  MEMORY: laakhon numbers, sab door           │
    └──────────────────────────────────────────────┘
```

Aur sabse kaam ki baat, jise log aakhir tak nahi samajh paate:

```
ek nirdesh chalana        →  1 kadam
paas wale khaane se number →  1 kadam
memory se number          →  lagbhag 200 kadam
disk se number            →  lagbhag 10 lakh kadam
```

CPU tez hai. Number laana dheema hai. **Zyadatar programs isliye dheere nahi hain ki hisaab bahut hai. Woh isliye dheere hain ki data door hai.**

Yeh baat aage kai jagah dohrayi jaayegi: Part 6 mein jab database aayenge, Part 7 mein jab server aayenge, aur Book 2 mein jab AI ka kharcha samjhenge.

---

### Asli duniya se ek example

1980 ke aas-paas CPU aur memory lagbhag ek hi raftaar se chalte the. Number maangna aur number milna, dono ek jaisa waqt lete the.

Uske baad CPU har saal lagbhag 50 pratishat tez hote gaye, aur memory sirf 10 pratishat ke aas-paas.

Chalees saal baad woh farak sau guna se zyada ho chuka hai. Iss badhti hui khaai ka apna naam pad gaya: **memory wall**.

Aaj ki chips ka bahut bada hissa hisaab karne mein nahi, balki iss khaai ko chhupane mein lagta hai. Numbers pehle se mangwa lena, paas mein copy rakh lena, aur jab tak ek number aa raha ho tab tak koi doosra kaam kar lena.

Yeh dhyaan dene laayak hai: chip ka aadhe se zyada design us problem ka hal hai jo chip ke andar hai hi nahi. Woh doori ka hal hai.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki tez processor matlab tez computer.**

Log GHz dekh kar phone khareedte hain, jaise woh ek hi number sab kuch bata deta ho.

Lekin agar CPU zyadatar waqt intezaar mein baithi hai, toh use aur tez karne se kuch nahi hoga. Woh bas aur jaldi intezaar karegi.

Isiliye aksar purane computer mein SSD daalne se woh naye jaisa lagne lagta hai, jabki CPU wahi purani hai. Aapne hisaab tez nahi kiya. Aapne **doori kam ki**.

Yeh galti tempting isliye hai ki speed ka ek hi number dikhaya jaata hai, aur "tez" ek hi shabd hai. Lekin computer mein kam se kam do alag "tez" hote hain: hisaab kitni jaldi hota hai, aur data kitni jaldi pahunchta hai. Doosra wala aksar zyada mayne rakhta hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  CPU          uthao, samjho, karo      │  ← naya
    │  DOORI        paas tez, door dheema    │  ← naya
    ├────────────────────────────────────────┤
    │  PAIMANA, COMPRESSION, SIZE            │
    ├────────────────────────────────────────┤
    │  PROGRAM, ENCODING, BINARY, SWITCH     │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

Har sawal pe ek minute socho, phir neeche jawab padho.

**1. (samajh check)** Ek program ko das lakh numbers jodne hain. Doosre ko sirf sau numbers jodne hain, lekin har number disk se laana padta hai. Kaunsa tez hoga?

> **Jawab:** Pehla, aur bahut aage se.
>
> Das lakh jod = das lakh kadam ke aas-paas.
>
> Sau numbers disk se = sau guna das lakh = dus karod kadam.
>
> Doosra program das hazaar guna kam hisaab kar raha hai aur phir bhi sau guna dheema hai.
>
> Isse ek rule nikalta hai jo poori kitaab mein kaam aayega: **hisaab sasta hai, data laana mehnga hai.** Jab bhi kuch dheema ho, pehle yeh poocho ki data kahan se aa raha hai, na ki yeh ki hisaab kitna hai.

**2. (samajh check)** Rasoiye wale example mein, aap saamne ki plate mein kya rakhoge aur almari mein kya?

> **Jawab:** Saamne woh jo abhi lag raha hai, ya abhi lagne wala hai. Almari mein baaki sab.
>
> Aur agar aapko pata ho ki agla kaam kya hai, toh aap use pehle se nikaal kar rakh lenge, taaki us waqt chalna na pade.
>
> Machine bilkul yehi karti hai, aur uske teen naam hain jo aage milenge: paas mein copy rakhna (cache), pehle se mangwa lena (prefetch), aur intezaar ke waqt koi doosra kaam kar lena.
>
> Teeno ek hi soch hain: **doori ko chhupa do.**

**3. (jodne wala)** Chapter 1.6 mein tay hua tha ki program aur data dono numbers hain, machine ek ko padhti hai aur doosre ko karti hai. Ab yeh chapter kehta hai ki dono laane mein waqt lagta hai. Isse kya nikalta hai?

> **Jawab:** Ki nirdesh laana bhi utna hi mehnga hai jitna data laana.
>
> Machine ko har kadam pe kam se kam do baar door jaana padta hai: ek baar agla nirdesh laane, ek baar us nirdesh ka data laane.
>
> Isiliye asli chips mein nirdeshon ke liye alag paas wali jagah hoti hai, data ki paas wali jagah se alag.
>
> Aur isiliye chhota program aksar tez chalta hai. Isliye nahi ki usmein kam kaam hai, balki isliye ki woh poora paas wali jagah mein aa jaata hai aur use baar baar door jaana nahi padta.
