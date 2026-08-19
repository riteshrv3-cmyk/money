# Chapter 5.3  [SPINE]
## Models ko compare kaise karte hain

### Samvaad

**Madhav:** Har hafte koi kehta hai ki naya model purane se behtar hai. Woh naapa kaise gaya?

**Kabir:** Koi test hoga.

**Madhav:** Aisa test banao. Kya rakhoge usmein?

**Kabir:** Sawal, aur unke sahi jawab.

**Madhav:** Kitne?

**Kabir:** Kuch hazaar.

**Madhav:** Aur woh sawal kahan se aayenge?

**Kabir:** Kisi ne likhe honge. Ya kisi exam se liye honge.

**Madhav:** Ab ek problem. Woh exam kahan chhapa tha?

**Kabir:** Kitaab mein. Ya internet pe.

**Madhav:** Aur model ne kya padha tha?

**Kabir:** Internet.

**Madhav:** Toh?

**Kabir:** Toh shayad us exam ke sawal aur jawab uske data mein hain.

**Madhav:** Toh woh test mein kya kar raha hai?

**Kabir:** Yaad kiya hua bata raha hai. Test kar hi nahi raha.

**Madhav:** Iska pata kaise chalega?

**Kabir:** Naye sawal banao jo kabhi chhape hi nahi.

**Madhav:** Aur agle saal?

**Kabir:** Agle saal woh bhi internet pe hongay.

**Madhav:** Toh har test ki ek umar hai.

**Kabir:** Haan. Woh purana hote hi bekaar ho jaata hai.

**Madhav:** Ab doosri problem. Companies ko pata hai ki unhe kis test pe naapa jaayega. Woh kya karengi?

**Kabir:** Us test ke liye taiyaari karengi.

**Madhav:** Jaise?

**Kabir:** Aise data pe train karengi jo us test jaisa ho.

**Madhav:** Kya woh dhokha hai?

**Kabir:** Poora dhokha nahi. Lekin ab test woh nahi naap raha jo naapna tha.

**Madhav:** Ab teesri, aur sabse zaroori. Ek model ganit ke test mein 92 percent laata hai. Aapko kya pata chala?

**Kabir:** Ki woh ganit mein achha hai.

**Madhav:** Kya woh aapka kaam kar payega?

**Kabir:** Pata nahi. Woh mere kaam ka test nahi tha.

**Madhav:** Toh us number se aapko kya mila?

**Kabir:** Lagbhag kuch nahi.

**Madhav:** Aur aapko kya chahiye tha?

**Kabir:** Mere apne kaam pe naap.

### Naam

Un tay-shuda teston ko **benchmark** kehte hain.

Unki teen pakki kamzoriyan hain, aur teeno Kabir ne nikaali:

```
1.  DATA MEIN AA JAANA
    test model ke training data mein ho sakta hai
    phir woh test nahi, yaaddasht ki jaanch hai

2.  TEST KE LIYE TAIYAARI
    companies jaanti hain kaunsa test hai
    aur us taraf khinch jaati hain, jaan-boojh ke ya bina soche

3.  AAPKE KAAM SE RISHTA NAHI
    benchmark ek aam kaam naapta hai
    aapka kaam aam nahi hai
```

Isliye ek naya tareeka bhi chalta hai: do models ke jawab logon ko dikhao, unse behtar chunwaao, aur us se ek ranking banao. Yeh data mein aane wali problem se bacha leta hai.

Aur uski apni kamzori hai, aur woh ab aap jaante ho: **log woh chunte hain jo pasand aata hai, na ki jo sahi hai.** Chapter 2.8. Toh aisi ranking us model ki taraf jhukti hai jo achha likhta hai aur sehmat hota hai.

Ab woh cheez jo iss chapter ka asli jawab hai:

> **Ek chhota, apna test banao. Bees sawal, apne asli kaam se, jinke sahi jawab aapko pata hain.**

Bees kaafi hain. Woh kisi ke data mein nahi hain. Woh aapka asli kaam naapte hain. Aur har naya model aane pe woh bees minute mein chal jaate hain.

Yeh koi jugaad nahi hai. **Yeh un logon ka asli tareeka hai jo isse sach mein kaam karwaate hain.**

### Asli duniya se

Ek jaani-pehchani cheez baar baar hui hai: koi model kisi benchmark pe kamaal karta hai aur asli kaam mein use karne wale kehte hain ki woh purane se kharaab lagta hai.

Aur dono sach hote hain. Benchmark ne jo naapa woh sach mein behtar hua. Aur woh cheez jo un logon ke kaam mein mayne rakhti thi, woh usmein thi hi nahi.

Isiliye badi companies apne khud ke, andar ke test rakhti hain, aur woh public nahi hote. Public na hone ki wajah seedhi hai: **jo test public ho jaata hai, woh agle saal bekaar ho jaata hai.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **benchmark ke number ko sachai maan lena.**

"92 percent" ek naap hai ek khaas test ka, ek khaas waqt pe. Woh aapke kaam ke baare mein kuch nahi kehta.

Doosri galti: **do numbers ke chhote farak ko mayne dena.**

Ek model 91.2 aur doosra 91.8. Yeh farak aksar shor hai. Aur woh khabar ban jaata hai.

Book 1 Chapter 2.2 wali baat: **pratishat mein badlav khabar hai, guna mein badlav badlav hai.** Yahan bhi wahi lagta hai. Ek benchmark pe 2 point ka farak lagbhag kuch nahi hai. Daam mein das guna ka farak sab kuch hai.

Teesri galti, aur yeh sabse mehngi hai: **naya model aane pe apna system badal dena, bina naape.**

Naya model aapke khaas kaam mein purane se kharaab ho sakta hai, chahe woh har public test mein aage ho.

Isliye woh bees sawal wala apna test hi asli bachaav hai. **Uske bina aap khabar ke aadhaar pe faisle le rahe ho.**

### Sochne ke liye

**1. (samajh check)** Aap apne product mein AI istemaal karte ho. Naya model aata hai jo har benchmark mein aage hai. Aap kya karoge?

> **Jawab:** Apne bees sawal chalao, dono models pe, aur khud dekho.
>
> Aur sirf sahi-galat mat dekho. Yeh bhi dekho: daam kya hai, raftaar kya hai, aur jawab ki shakal badli toh nahi (kyunki aapka baaki code us shakal pe khada ho sakta hai).
>
> **Benchmark aapko yeh batata hai ki dekhna chahiye. Woh aapko yeh nahi batata ki badal do.**

**2. (samajh check)** Ek benchmark do saal purana hai aur sab models usmein 95 se upar hain. Kya woh benchmark ab bhi kaam ka hai?

> **Jawab:** Nahi, do wajahon se.
>
> **Ek:** woh ab data mein aa chuka hai. Sab uske jawab jaante hain.
>
> **Do:** jab sab 95 se upar hain, toh woh test ab farak dikha hi nahi sakta. Uski poori range khatam ho gayi.
>
> Isiliye naye benchmark banate rehna padta hai, aur har ek ki umar do-teen saal hoti hai.
>
> **Ek test jismein sab paas ho jaate hain, woh test nahi rehta.**

**3. (jodne wala)** Chapter 4.3 mein tha ki ek hi sawal kai baar poochne se pata chalta hai ki model sthir hai ya nahi. Kya woh apne test mein daala ja sakta hai?

> **Jawab:** Haan, aur woh use kaafi behtar bana deta hai.
>
> Har sawal paanch baar chalao. Ab aapko do cheezein milti hain: kitni baar sahi, aur kitna sthir.
>
> Ek model jo paanch mein se chaar baar sahi hai aur ek baar bilkul alag jawab deta hai, woh us model se alag hai jo paanchon baar wahi jawab deta hai.
>
> **Aur woh farak aapke system ke liye aksar sahi-galat se zyada mayne rakhta hai**, kyunki aap us pe bharosa karke aage kuch bana rahe ho.
