# Chapter 6.6  [DEPTH]
## Sab ek saath aa jaayein toh kya tootta hai

---

*DEPTH chapter. Yahan aap seekhoge ki systems kis tarah girte hain, aur kyun woh dheere-dheere kharaab nahi hote, balki ek jhatke mein baith jaate hain.*

---

### Samvaad

**Madhav:** Ek system ek second mein sau sawal sambhal sakta hai. Ninanve aane lage. Kya haal hoga?

**Kabir:** Theek chalega. Thoda dheema.

**Madhav:** Ek sau ek?

**Kabir:** Ek sawal line mein rukega.

**Madhav:** Aur agle second mein bhi ek sau ek?

**Kabir:** Do ruk jaayenge.

**Madhav:** Aur yeh ek ghante tak chalta rahe?

**Kabir:** Line badhti jaayegi. Teen hazaar se zyada.

**Madhav:** Aur line mein khade log kya kar rahe hain?

**Kabir:** Intezaar.

**Madhav:** Kitna intezaar?

**Kabir:** Aakhri wale ko... poori line ka waqt. Bahut zyada.

**Madhav:** Aur jo aadmi tees second intezaar kar chuka hai, woh kya karega?

**Kabir:** Chhod dega. Ya refresh karega.

**Madhav:** Refresh karega toh?

**Kabir:** Ek naya sawal aa jaayega. Line aur badhegi.

**Madhav:** Aur purana sawal?

**Kabir:** Woh bhi line mein hi hai. Woh bhi kaam karwayega, chahe ab uska jawab koi na dekhe.

**Madhav:** Toh ab dhyaan se dekho. Bojh sirf ek pratishat zyada tha. Kya hua?

**Kabir:** Log ruke, phir chhod kar dobara aaye, jisse bojh aur badh gaya, jisse aur log ruke.

**Madhav:** Toh system ka bojh kitna badha?

**Kabir:** Do guna, teen guna. Khud badhta chala gaya.

**Madhav:** Aur system ek pratishat zyada ke liye taiyaar tha?

**Kabir:** Ek pratishat ke liye toh tha. Teen guna ke liye nahi.

**Madhav:** Bas. Ab batao, yeh dheere-dheere kharaab hua ya achanak?

**Kabir:** Achanak. Ninanve pe sab theek tha, ek sau ek pe sab kuch baith gaya.

**Madhav:** Toh kya karoge?

**Kabir:** Line ko badhne hi mat do. Ek seema ke baad naye sawal mana kar do.

**Madhav:** User ko mana karna? Woh toh bura hai.

**Kabir:** Sabko dheere-dheere marne dene se behtar hai. Kam se kam kuch logon ko jawab toh milega.

**Madhav:** Bas. Yeh iss chapter ka sabse zaroori faisla hai. **Sabko thoda thoda dena, ya kuch ko poora dena.** Aur bade systems lagbhag hamesha doosra chunte hain.

---

### Naam

Woh haalat jismein bojh khud ko badhata jaata hai, use **cascading failure** kehte hain, yaani girti hui shrinkhla.

Uska dhaancha hamesha ek jaisa hota hai:

```
1. bojh seema ke thoda upar gaya
2. jawab dheema hua
3. log ne intezaar chhod kar dobara koshish ki
4. bojh aur badha
5. aur dheema hua
6. wapas 3 pe

Bojh 1% badha. System 100% baith gaya.
```

Aur uske hal, jo lagbhag har bade system mein hote hain:

```
LINE PE SEEMA         ek had ke baad naye sawal mana karo
                      "abhi bahut bheed hai, thodi der baad"

PURANE SAWAL PHENK DO agar aadmi ja chuka hai toh uska kaam mat karo

BACHAV KA SWITCH      jab ek hissa girne lage toh use turant band karo
                      aur baaki chalne do
                      (nahi toh woh sabko apne saath le jaayega)

THODI DER RUK KAR     dobara koshish karo, lekin sabhi ek saath nahi
                      warna sab ek hi pal pe wapas aayenge
```

Aakhri wala dhyaan dene laayak hai. Agar sab log theek paanch second baad dobara koshish karein, toh woh ek saath aayenge aur system phir baith jaayega. Isliye har ek ko thoda alag intezaar diya jaata hai.

Aur ab woh baat jo iss chapter ki asli seekh hai:

**System dheere-dheere kharaab nahi hote. Woh ek seema tak bilkul theek chalte hain aur uske baad ek jhatke mein baith jaate hain.**

Isiliye "abhi toh sab theek chal raha hai" koi jaankari nahi hai. Aap seema se 20 pratishat neeche ho sakte ho ya 1 pratishat neeche, aur dono bilkul ek jaise dikhte hain.

---

### Asli duniya se ek example

Har saal kisi na kisi badi ticket ki bikri, sale, ya result ke din yeh dohraya jaata hai. Site pehle dheemi hoti hai, phir error dene lagti hai, phir poori tarah baith jaati hai.

Aur aksar company ne bojh ka andaza sahi lagaya hota hai. Unhone shayad das guna machinein bhi laga rakhi hoti hain.

Jo cheez tootti hai woh ginti nahi hoti, woh **shrinkhla** hoti hai. Log refresh karte hain, har refresh ek naya sawal hai, aur bojh us ginti se bahut aage nikal jaata hai jiska andaza lagaya gaya tha.

Isiliye achhe systems in dinon mein ek "line" wala page dikhate hain. Woh page kuch nahi karta, sirf aapko rokta hai. Woh bura anubhav hai, aur woh jaan-boojh ke chuna gaya hai, kyunki uska vikalp yeh hai ki kisi ko kuch na mile.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki zyada machinein lagane se yeh problem hal ho jaayegi.**

Machinein seema ko upar khiska deti hain. Woh shrinkhla ko nahi rokti.

Agar aap das guna machinein laga do, toh aap das guna bojh sambhal loge. Aur jis din bojh gyarah guna hoga, us din bilkul wahi cheez hogi, sirf bade paimane pe.

Asli hal seema badhana nahi hai. Asli hal yeh hai ki **seema paar hone pe system ko sahi tarah se mana karna aana chahiye.**

Doosri galti: yeh sochna ki mana karna kharaab service hai.

Ek system jo dus hazaar logon ko turant mana kar deta hai aur nabbe hazaar ko theek se jawab deta hai, woh us system se kahin behtar hai jo ek lakh logon ko chhe minute intezaar karake sabko error deta hai.

Yeh galti tempting isliye hai ki mana karna dikhta hai aur dheema hona chhupa rehta hai. Manager ko "humne 10% users ko mana kiya" bura lagta hai aur "sab dheema chal raha tha" kam bura lagta hai, jabki doosra kaafi bura hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  SHRINKHLA    bojh khud ko badhata hai  │  ← naya
    │  SEEMA        paar hone pe mana karo    │  ← naya
    │               dheere nahi, jhatke mein  │
    ├────────────────────────────────────────┤
    │  CLOUD, API, UPTIME, BADA HONA          │
    ├────────────────────────────────────────┤
    │  QUEUE, CACHE, DATABASE, INTERNET       │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek system fail hone lagta hai aur uske saare users ko "10 second baad dobara koshish karein" ka message milta hai. Kya problem hai?

> **Jawab:** Sab log theek das second baad ek saath wapas aayenge.
>
> System ko thodi der araam milega aur phir ek hi pal mein poora bojh wapas aa jaayega, shayad pehle se bhi bada.
>
> Isliye har user ko thoda alag intezaar dena chahiye, jaise 8 se 15 second ke beech koi bhi.
>
> Yeh chhoti si baat lagti hai aur woh kai bade systems ko bacha chuki hai. **Ek saath wapas aana khud ek hamla ban jaata hai.**

**2. (samajh check)** Aapka system 100 per second sambhal sakta hai aur abhi 60 aa rahe hain. Kya aap surakshit ho?

> **Jawab:** Pata nahi, aur yeh iss chapter ki asli seekh hai.
>
> 60 par sab theek dikhta hai. 95 par bhi sab theek dikhta hai. Aapko dono mein farak nahi dikhega.
>
> Aur bojh aksar thoda thoda nahi badhta. Ek tweet, ek khabar, ek sale, aur woh das guna ho jaata hai.
>
> Isliye achhe systems mein yeh naapa jaata hai ki **abhi seema se kitna neeche hain**, na ki sirf yeh ki sab theek chal raha hai ya nahi.

**3. (jodne wala)** Chapter 5.6 mein queue thi, jismein kaam line mein lagta tha. Kya queue iss problem ko hal karti hai ya badhati hai?

> **Jawab:** Dono, aur yeh dhyaan dene laayak hai.
>
> **Hal karti hai:** user ko intezaar nahi karna padta, kyunki uska kaam line mein daal kar use "ho gaya" keh diya jaata hai.
>
> **Badhati hai:** agar kaam aane ki raftaar hone ki raftaar se zyada rahi, toh line badhti jaayegi, hamesha. Woh chup-chaap badhti hai kyunki user ko dikhta hi nahi.
>
> Aur ek din woh itni lambi ho jaati hai ki usmein pada kaam ab bekaar ho chuka hota hai. Log ko ek ghante purani notification milti hai.
>
> Isliye har queue ke saath do cheezein dekhi jaati hain: **woh kitni lambi hai, aur kitni tezi se badh rahi hai.** Lambai se pata chalta hai ki abhi kya haal hai. Raftaar se pata chalta hai ki aage kya hoga.
