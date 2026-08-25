# Chapter 5.6  [SPINE]
## Kaam ko line mein lagana

---

### Samvaad

**Madhav:** Aap ek app pe photo upload karte ho. App ko chaar kaam karne hain: photo rakhna, uska chhota version banana, aapke doston ko batana, aur aapko "ho gaya" dikhana. Kitna waqt lagega?

**Kabir:** Photo rakhna jaldi. Chhota version banana thoda waqt lega. Batana bhi.

**Madhav:** Maan lo chaar second lagte hain. Aapko "ho gaya" kab dikhega?

**Kabir:** Chaar second baad.

**Madhav:** Aur aap tab tak kya kar rahe ho?

**Kabir:** Ghoomta hua circle dekh raha hoon.

**Madhav:** Kya un chaaron kaamon ke liye aapka intezaar zaroori hai?

**Kabir:** Photo rakhna toh zaroori hai. Warna woh gayab ho jaayegi.

**Madhav:** Aur chhota version?

**Kabir:** Woh baad mein bhi ban sakta hai.

**Madhav:** Doston ko batana?

**Kabir:** Woh bhi baad mein.

**Madhav:** Toh kya karoge?

**Kabir:** Photo rakh do, aur baaki kaam kahin likh do ki karne hain. Phir turant "ho gaya" dikha do.

**Madhav:** Aur baaki kaam kaun karega?

**Kabir:** Koi doosra program jo us list ko dekhta rahe.

**Madhav:** Ab batao user ko kya dikha. Aur sach kya hai.

**Kabir:** User ko "ho gaya" dikha, aur sach yeh hai ki aadha hua hai.

**Madhav:** Kya yeh jhooth hai?

**Kabir:** Thoda toh hai.

**Madhav:** Kya user ko farak padta hai?

**Kabir:** Agar chhota version do second baad ban jaaye toh nahi padta.

**Madhav:** Aur agar woh kabhi na bane?

**Kabir:** Toh padta hai. Toh us list mein rakhe kaam kabhi kho nahi sakte.

**Madhav:** Bas. Ab woh list. Do log ek saath usmein daalein toh?

**Kabir:** Wahi purani problem. Taala.

**Madhav:** Aur ek kaam do log utha lein?

**Kabir:** Toh do baar hoga. Photo ka chhota version do baar ban jaayega.

**Madhav:** Kya bura hai?

**Kabir:** Uss case mein bura nahi. Lekin agar kaam "paise bhejo" hota toh?

**Madhav:** Toh?

**Kabir:** Toh do baar paise chale jaate.

**Madhav:** Toh kaam ko aisa banana padega ki do baar hone se bhi nuksaan na ho.

**Kabir:** Kaise?

**Madhav:** Har kaam pe ek pehchaan number daal do, aur karne se pehle dekh lo ki yeh number pehle to nahi ho chuka.

---

### Naam

Us list ka naam hai **queue**, yaani ek kataar.

Aur us poore tareeke ka naam hai kaam ko **turant** aur **baad mein** mein baant dena:

```
TURANT (user ka intezaar)     jo bina hue user ko nateeja nahi mil sakta
BAAD MEIN (queue)             jo baad mein ho sakta hai
```

Yeh sabse aam aur sabse zyada asar wala tareeka hai kisi bhi cheez ko tez dikhane ka. Aur dhyaan do ki usne kaam kam nahi kiya. Chaaron kaam abhi bhi ho rahe hain. Bas user ab unka intezaar nahi kar raha.

**Cheez tez nahi hui. Intezaar hat gaya.**

Queue ke saath teen niyam aate hain, aur teeno Kabir ne khud chhue:

```
1. KAAM KHO NA SAKE
   queue ko disk pe rakhna padta hai, RAM mein nahi

2. DO BAAR HO SAKTA HAI
   isliye har kaam aisa hona chahiye ki dobara hone pe nuksaan na ho
   (iske liye har kaam ko ek pehchaan number diya jaata hai)

3. KAAM FAIL HO SAKTA HAI
   toh use dobara koshish karni chahiye, kuch der baad
   aur agar baar baar fail ho toh use alag rakh do, taaki
   woh baaki sab ko na roke
```

Teesri baat pe ek naam hai: jo kaam baar baar fail hote hain unhe ek alag jagah rakh diya jaata hai, jise **dead letter queue** kehte hain. Woh us chitthi jaisi hai jo na pahunch payi aur na wapas ja payi, aur post office ke ek kone mein rakh di gayi.

---

### Asli duniya se ek example

Jab aap kisi shopping app pe order karte ho, toh "order confirmed" turant dikh jaata hai.

Us waqt tak sirf ek cheez hui hai: aapka order likh liya gaya hai. Baaki sab kuch queue mein pada hai. Payment ki jaanch, saaman ka reservation, godaam ko sandesh, aapko email, delivery ka plan.

Isiliye kabhi kabhi aapko "order confirmed" ke das minute baad "sorry, saaman khatam ho gaya" wala message aata hai. Woh galti nahi hai. Woh iss design ka seedha nateeja hai.

Company ne jaan-boojh ke yeh chuna hai. Wajah karobaari hai: agar checkout mein aath second lagein toh log chhod kar chale jaate hain. Aath second ka intezaar us thodi si gadbad se zyada mehnga hai jo baad mein maafi maang kar theek ki ja sakti hai.

Yeh Chapter 5.4 wala sauda hai, phir se: **thodi galti, ya bahut intezaar.**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **"ho gaya" ko "sach mein poora ho gaya" samajhna.**

Aaj ke lagbhag har bade system mein "ho gaya" ka matlab hai "humne pakka likh liya hai ki yeh hoga."

Yeh dhokha nahi hai, jab tak woh sach mein ho jaaye. Lekin iska matlab hai ki beech mein ek khidki hai jismein cheez aadhi hui padi hai.

Iska seedha nateeja: log samajh nahi paate ki paise "bhej diye" ke baad bhi kai ghante kyun lag jaate hain, ya order confirm hone ke baad cancel kyun ho jaata hai.

Aur banane walon ke liye ek doosri galti hai: queue daal dena aur yeh maan lena ki ab woh kaam ho hi jaayega. Queue kaam hone ki guarantee nahi hai. Woh sirf yeh guarantee hai ki kaam **yaad rakha jaayega**. Kya woh ho paayega, yeh ek alag sawal hai, aur usko koi na koi dekhta rehna chahiye.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  QUEUE        turant vs baad mein       │  ← naya
    │               kaam kam nahi hua,        │
    │               intezaar hat gaya         │
    ├────────────────────────────────────────┤
    │  CACHE, TRANSACTION, INDEX, DATABASE    │
    ├────────────────────────────────────────┤
    │  INTERNET, OS, CPU, RAM/DISK, SWITCH    │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek email bhejne wala app hai. User "send" dabata hai. Kaunse kaam turant hone chahiye aur kaunse queue mein?

> **Jawab:** Turant: email ko pakka likh lo, aur "bhej diya" dikha do.
>
> Queue mein: asli email ko doosre server tak pahunchana, koshish karna, fail ho toh dobara koshish karna, attachment sambhalna.
>
> Wajah: doosre server tak pahunchne mein kuch second se kuch ghante lag sakte hain, aur woh aapke control mein nahi hai. User ko utni der rokna bekaar hai.
>
> Aur isiliye email kabhi kabhi der se pahunchte hain aur kabhi wapas aa jaate hain, "bhej diya" dikhne ke ghanton baad.

**2. (samajh check)** Ek kaam queue mein hai: "user ke khaate se sau rupaye kaato." Woh galti se do baar utha liya jaata hai. Kya karoge?

> **Jawab:** Har kaam ko ek pehchaan number do, aur karne se pehle dekho ki woh number pehle ho chuka hai ya nahi.
>
> Yaani kaam ko aisa banao ki dobara chalane se kuch naya na ho.
>
> Yeh soch bahut kaam ki hai: **maan lo ki har cheez do baar hogi, aur cheez ko aisa banao ki isse farak na pade.**
>
> Kyunki bade systems mein cheezein sach mein do baar hoti hain. Network ka jawab kho jaata hai, koshish dobara hoti hai, aur pehli baar sach mein ho chuki thi.

**3. (jodne wala)** Chapter 4.3 mein UDP tha, jismein kho gaya toh chhod diya jaata hai. Queue usse kaise alag hai?

> **Jawab:** Ulta hai, aur wajah wahi purani hai: kya purana kaam ab bhi kaam ka hai?
>
> UDP: awaaz ka ek tukda kho gaya. Use dobara laane ka koi faayda nahi, kyunki woh purana ho chuka hai. Chhod do.
>
> Queue: "paise kaato" wala kaam kho gaya. Woh purana nahi hota. Woh aaj bhi utna hi zaroori hai. Isliye use kabhi chhoda nahi ja sakta.
>
> Toh ek hi sawal, do ulte jawab, aur farak sirf yeh hai ki **kaam ki keemat waqt ke saath girti hai ya nahi.**
>
> Yeh sawal aage bar bar poochna kaam ka hai. Woh lagbhag hamesha yeh tay kar deta hai ki system ka design kaisa hoga.
