# Chapter 3.5  [SPINE]
## Bada karne se behtar kyun hota gaya

### Samvaad

**Madhav:** Design 2017 mein tay ho gaya. Uske baad kya badla?

**Kabir:** Model bade hote gaye.

**Madhav:** Aur kya?

**Kabir:** Data zyada. Machinein zyada.

**Madhav:** Bas teen cheezein. Ab batao: agar aap ek model ko das guna bada karo, toh kitna behtar hoga?

**Kabir:** Das guna?

**Madhav:** Nahi. Aur yeh dilchasp hai. Loss thoda girta hai, aur woh girna kaafi pakka hai. Itna pakka ki uske liye ek hisaab likha ja sakta hai.

**Kabir:** Yaani pehle se andaza lagaya ja sakta hai?

**Madhav:** Kaafi hadd tak. Agar aap itni machine aur itna data lagao, toh loss lagbhag itna hoga. Yeh 2020 ke aas-paas dikhna shuru hua.

**Kabir:** Toh yeh andaza lagane laayak ho gaya.

**Madhav:** Aur usi ne sab kuch badal diya. Socho kyun. Ek company ko karodon dollar kharch karne hain. Pehle woh kaise tay karti?

**Kabir:** Ummeed pe. Pata nahi ki kya milega.

**Madhav:** Aur ab?

**Kabir:** Ab woh andaza laga sakti hai ki itna kharch karne se itna behtar milega.

**Madhav:** Toh paisa aane laga.

**Kabir:** Kyunki risk kam ho gaya.

**Madhav:** Ab ek aur cheez. Loss dheere dheere girta hai, seedhi line mein. Lekin kaabiliyat?

**Kabir:** Woh bhi dheere dheere badhti hogi.

**Madhav:** Ek chhota model bilkul jodna nahi jaanta. Thoda bada, thoda bada, aur ek jagah pe achanak woh jodna shuru kar deta hai.

**Kabir:** Achanak?

**Madhav:** Bahar se achanak. Loss mein koi chhalang nahi hoti. Woh usi seedhi line pe girta rehta hai.

**Kabir:** Toh loss dheere gir raha hai aur kaabiliyat chhalang maar rahi hai?

**Madhav:** Aisa dikhta hai. Aur yahan ek asli bahas hai. Kuch log kehte hain ki woh sach mein chhalang hai. Doosre kehte hain ki humne naapne ka tareeka hi aisa chuna ki woh chhalang jaisi dikhe.

**Kabir:** Kaise?

**Madhav:** Agar aap yeh naapo ki "poora sawal sahi hua ya nahi," toh nateeja haan-na hai. Model dheere dheere behtar ho raha tha, lekin woh haan-na mein tab tak nahi dikha jab tak woh poora sahi na kar de.

**Kabir:** Toh chhalang naap mein thi, model mein nahi.

**Madhav:** Kuch mamlon mein saaf yehi dikha hai. Sab mein nahi. **Yeh ek khula sawal hai aur main aapko iska jawab nahi de sakta, kyunki abhi kisi ke paas nahi hai.**

### Naam

Woh hisaab jo batata hai ki kitna kharch karne se kitna faayda hoga, use **scaling laws** kehte hain.

Teen cheezein badhani padti hain, aur teeno saath:

```
MODEL     zyada parameters
DATA      zyada tokens
MACHINE   zyada hisaab
```

Aur ek zaroori baat: **inhe barabar badhana padta hai.** Ek bada model chhote data pe woh sab yaad kar lega aur naye pe kamzor rahega (Chapter 2.4 ka overfitting). Ek chhota model bade data se poora faayda nahi utha sakta.

Shuruaat mein log models ko bahut bada aur data ko bahut chhota rakh rahe the. 2022 ke aas-paas yeh dikha ki woh galat anupaat tha. Uske baad chhote models zyada data pe train hone lage, aur woh purane bade models se behtar nikle.

**Isiliye "kitne parameters" ab woh sawal nahi raha jo do saal pehle tha.**

Aur woh cheez jise log **emergence** kehte hain: kuch kaabiliyat chhote models mein bilkul nahi hoti aur ek paimane ke baad dikhne lagti hai.

Ismein do sawal alag hain, aur unhe alag rakhna zaroori hai:

```
KYA WOH SACH MEIN CHHALANG HAI?   ispe bahas hai, jawab tay nahi
KYA WOH PEHLE SE PATA CHAL SAKTI HAI? nahi. Yeh sab maante hain.
```

Doosri baat zyada mayne rakhti hai. Aap scaling laws se loss ka andaza laga sakte ho. Aap yeh andaza nahi laga sakte ki agla model kaunsa naya kaam kar lega.

**Kharcha andaza laga sakte ho. Kaabiliyat nahi.**

### Asli duniya se

2019 se 2023 tak models tez badhe: karodon parameters se kharabon tak.

Uske baad shakal badal gayi. Ab jo behtari aa rahi hai woh sirf size se nahi aa rahi. Woh aa rahi hai behtar data se, behtar dhalai se (Chapter 2.8), aur us tareeke se jismein model jawab dene se pehle apne liye khud kuch likh leta hai.

Aur ek wajah bhi hai jo saaf hai: **aasan data khatam ho raha hai.** Web ek baar hi hai. Aur ab usmein AI ka likha bhi mila hua hai (Chapter 2.7).

Toh "bas aur bada kar do" ka daur dheema pad raha hai. Woh khatam nahi hua, lekin woh ab akela raasta nahi hai.

Yeh dhyaan dene laayak hai, kyunki 2023 mein har koi keh raha tha ki bas paimana hi sab kuch hai. Woh ek waqt ki baat thi, hamesha ka niyam nahi.

### Yahan log kya galat samajhte hain

Sabse aam galti: **scaling laws ko prakriti ka niyam samajhna.**

Woh niyam nahi hain. Woh us range mein dekhi gayi ek line hai jismein log ne prayog kiye. Aage jaakar woh mud sakti hai, aur mudti hui dikh bhi rahi hai.

Doosri galti: **yeh sochna ki bade model hamesha behtar hain.**

Ek chhota naya model ek bade purane se behtar ho sakta hai, aur aksar hota hai. Kyunki size sirf teen mein se ek cheez hai.

Aur teesri, jo sabse mehngi hai: **yeh sochna ki agla model kya kar payega, yeh koi jaanta hai.**

Kisi ko nahi pata. Companies ko bhi nahi. Woh train karte hain aur phir dekhte hain ki kya nikla.

Iska aapke liye ek seedha matlab hai: **jab koi kahe ki "agle saal AI yeh kar lega," toh woh andaza hai, jaankari nahi.** Chahe woh kahin se bhi keh raha ho.

### Sochne ke liye

**1. (samajh check)** Ek company kehti hai "hamara model das guna bada hai." Aap kya poochoge?

> **Jawab:** Kam se kam teen cheezein.
>
> **Data kitna badha?** Agar sirf model bada hua aur data wahi raha, toh woh shayad behtar nahi hoga, aur overfit ho sakta hai.
>
> **Naapa kaise?** Bade hone se loss girta hai. Loss girna aur kaam mein behtar hona alag baatein hain (Chapter 2.4).
>
> **Mere kaam pe kaisa hai?** Aam benchmarks se aapke apne kaam ka koi seedha rishta nahi hai. Chapter 5.3.

**2. (samajh check)** Kaabiliyat "achanak" aane ka ek udaharan aap khud soch sakte ho?

> **Jawab:** Sochne ka tareeka yeh hai: aisa kaam dhoondho jo tab tak bilkul galat rehta hai jab tak poora sahi na ho jaaye.
>
> Do teen ank ka guna. Ek lambi shrinkhla ka tark. Kisi ajeeb niyam ko poori tarah nibhana.
>
> In sab mein aadha sahi hona zero hai. Toh model dheere dheere behtar ho raha hota hai aur naap mein kuch nahi dikhta, jab tak woh poora na kar le.
>
> **Aur wahi un logon ka tark hai jo kehte hain ki chhalang naap mein thi.** Agar aap "kitne ank sahi hue" naapo, toh line seedhi dikhne lagti hai.

**3. (jodne wala)** Book 1 Ch 2.2 mein tha ki pratishat mein badlav khabar hai aur guna mein badlav badlav hai. Scaling laws pe woh kaise lagta hai?

> **Jawab:** Seedha lagta hai, aur woh iss poore field ki shakal samjha deta hai.
>
> Model 10 pratishat bade hone se kuch nahi hota. Woh naap mein bhi mushkil se dikhta hai.
>
> Model sau guna bade hone se ek nayi duniya khulti hai.
>
> Isliye yeh field chhoti behtari se nahi, badi chhalangon se chalta hai, aur unke beech mein lambe shant daur hote hain.
>
> Aur isiliye kharcha itna bada hai. **Guna mein badlav ke liye guna mein paisa chahiye**, aur wahi tay karta hai ki kaun khel sakta hai. Chapter 7.1.
