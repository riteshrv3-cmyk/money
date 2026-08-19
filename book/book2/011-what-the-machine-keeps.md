# Chapter 2.3  [SPINE]
## Machine actually rakhti kya hai

### Samvaad

**Madhav:** Training ke baad kya bachta hai? Woh numbers. Lekin woh numbers hain kya? Kya woh yaad ki hui baatein hain?

**Kabir:** Shayad. Usne internet padha, toh usne yaad kar liya hoga.

**Madhav:** Chalo naapte hain. Internet pe jitna text hai, uska size lagbhag kitna hoga? Sirf likhawat.

**Kabir:** Bahut. Kai lakh GB?

**Madhav:** Aur ek bade model ki file kitni badi hai?

**Kabir:** Aapne kaha tha kuch sau GB.

**Madhav:** Toh kya usmein woh sab text aa sakta hai?

**Kabir:** Nahi. Woh hazaaron guna chhota hai.

**Madhav:** Toh usne yaad nahi kiya. Phir usne kya rakha?

**Kabir:** Sirf zaroori cheezein?

**Madhav:** Kaun tay karta hai ki kya zaroori hai?

**Kabir:** Koi nahi. Woh khud nikla hoga.

**Madhav:** Ek udaharan se dekhte hain. Aapne hazaaron vaakya padhe jinmein "raja" aur "rani" the. Aapne un vaakyon ko yaad rakha?

**Kabir:** Nahi.

**Madhav:** Toh aapke paas kya bacha?

**Kabir:** Yeh ki raja aur rani jaisi cheezein hain. Ek aadmi hai, ek aurat, dono ka rutba bada hai.

**Madhav:** Kya woh kisi ek vaakya mein likha tha?

**Kabir:** Nahi. Woh sabse mila kar bana.

**Madhav:** Aur woh sab vaakya ab kahan hain?

**Kabir:** Gaye. Sirf nichod bacha.

**Madhav:** Toh training kya kar rahi hai?

**Kabir:** Woh dohrav nichod rahi hai. Book 1 wali compression jaisi.

**Madhav:** Aur uski keemat kya hai? Compression mein kya hota tha?

**Kabir:** Kuch hamesha ke liye chala jaata hai. Lossy wali.

**Madhav:** Toh model se kya chala jaata hai?

**Kabir:** Jo cheez sirf ek baar aayi ho. Jiska koi pattern na ho.

**Madhav:** Aur agar aap usse woh cheez poochhoge jo sirf ek baar likhi gayi thi?

**Kabir:** Woh nahi jaanta hoga. Lekin woh... shayad kuch bana dega jo aisa lagta ho.

**Madhav:** Kyun banayega? Chup kyun nahi rahega?

**Kabir:** Kyunki uska kaam hi agla token chunna hai. Woh kabhi khaali nahi de sakta.

**Madhav:** Aapne abhi hallucination ka aadha jawab nikaal liya. Chapter 5.1 mein hum ise poora karenge. Ab aakhri sawal. Ek aisa number uthao, un arbon mein se ek. Uska kya matlab hai?

**Kabir:** Pata nahi.

**Madhav:** Kisi ko pata hai?

**Kabir:** Shayad nahi.

**Madhav:** Kisi ko nahi. Aur yeh koi rahasya nahi hai jo koi chhupa raha ho. Woh number kisi ek cheez ke liye hai hi nahi. Woh arbon ke saath milkar kaam karta hai.

### Naam

Un numbers ko **weights** kehte hain, aur unki ginti ko **parameters**.

Jab koi kehta hai "70 billion parameter model," toh uska matlab hai: usmein 70 arab numbers hain.

Ab teen baatein jo iss chapter ki jaan hain.

**Ek: model ek nichod hai, ek copy nahi.**

```
internet ka text     lakhon GB
model ki file        kuch sau GB
```

Isliye woh yaad nahi kar sakta. Woh patterns rakhta hai.

Ek apwaad dhyaan dene laayak hai: **jo cheez data mein hazaaron baar dohrayi gayi ho, woh lagbhag yaad ki hui jaisi ho sakti hai.** Ek mashhoor kavita, ek aam code ka tukda, ek prasiddh vaakya. Woh itni baar aaya ki uska nichod hi woh khud hai.

Aur isse ek asli problem nikalti hai jo abhi adaalaton mein hai: agar model kisi ki likhi cheez lagbhag jaisi ki taisi likh de, toh woh seekhna hai ya nakal? Iska jawab abhi tay nahi hua hai, aur log dono taraf hain.

**Do: nichodna lossy hai.**

Jo baar baar aaya woh mazbooti se bacha. Jo ek baar aaya woh lagbhag gaya. Aur model ko yeh khud pata nahi hota ki kya bacha aur kya gaya.

**Teen: ek weight ka koi matlab nahi hota.**

Aap ek weight nahi padh sakte. Aap yeh nahi keh sakte ki "yeh wala Dilli ke liye hai." Gyaan kisi ek jagah nahi hai, woh arbon numbers mein bikhra hua hai.

Isiliye model se koi ek cheez "nikaali" nahi ja sakti. Agar aap chahte ho ki woh kisi ek baat ko bhool jaaye, toh koi aisi jagah nahi hai jise mitaya ja sake.

### Asli duniya se

Models ke size aksar aise likhe jaate hain:

```
7 billion parameters      ek achhi machine pe chal sakta hai
70 billion                ek server chahiye
sabse bade                kai machinein saath
```

Har parameter aam taur pe do byte leta hai. Toh 70 arab parameter ka matlab hai lagbhag 140 GB, sirf rakhne ke liye. Chalane ke liye woh RAM mein aana chahiye.

Yeh Book 1 Chapter 2.2 ka hisaab hai, seedha lagaya hua. Aur yeh batata hai ki kaunsa model kahan chal sakta hai, bina kisi marketing ke.

Ek baat jo badal rahi hai: parameters ki ginti pehle jitni mayne nahi rakhti. Ab chhote models bade purane models se behtar nikal rahe hain, kyunki training ka data aur tareeka behtar hua hai.

**Toh "kitne parameters" ab woh sawal nahi raha jo do saal pehle tha.** Chapter 5.3 mein hum dekhenge ki ab kya naapa jaata hai.

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki model ke andar ek database hai.**

Log sochte hain ki usne tathya kahin rakh liye hain, aur sawal aane pe woh unhe dekh kar jawab deta hai.

Aisa kuch nahi hai. Koi list nahi hai jise koi khol sake. Koi jagah nahi hai jahan "Bharat ki rajdhani" likha ho.

Iske do seedhe nateeje hain jo roz dikhte hain:

**Ek:** aap use "update" nahi kar sakte jaise database ko karte ho. Ek nayi baat batane ke liye ya toh dobara train karo, ya woh baat sawal ke saath bhejo (jo Chapter 7 mein aayega).

**Do:** woh nahi jaanta ki woh kya nahi jaanta. Ek database bata sakta hai ki "yeh entry nahi hai." Yahan koi entry hai hi nahi, toh khali jagah bhi nahi hai jo dikh sake.

Doosri galti: **parameters ki ginti ko kaabiliyat ka naap samajhna.** Do saal pehle woh kaafi hadd tak sach tha. Ab nahi hai.

### Sochne ke liye

**1. (samajh check)** Model ko kisi ek galat baat bhoolni hai. Kya aap use mita sakte ho?

> **Jawab:** Nahi, aur yeh ek asli problem hai jispe abhi kaam ho raha hai.
>
> Woh baat kisi ek jagah nahi hai. Woh arbon numbers mein bikhri hui hai, doosri lakhon baaton ke saath mili hui.
>
> Jo kiya jaata hai woh do mein se ek hai: ya toh dobara train karo (bahut mehnga), ya upar ek parat lagao jo us jawab ko rok de (jo asli mein hataana nahi hai, chhupana hai).
>
> Yeh sirf technical baat nahi hai. Kanoon kehta hai ki logon ko "bhula diye jaane ka haq" hai, aur ek aisi cheez jismein kuch mitaya hi nahi ja sakta, us haq ke saath seedha takrati hai.

**2. (samajh check)** Model ki file 140 GB hai aur internet ka text lakhon GB. Isse aap ek practical baat kya nikaal sakte ho?

> **Jawab:** Ki jo cheez kam baar likhi gayi hai, uspe model kamzor hoga.
>
> Aam cheezein hazaaron baar aayin, woh mazbooti se bachi. Aapke sheher ka koi chhota niyam, ya kisi khaas kaam ka tareeka, shayad das baar aaya, aur woh lagbhag nahi bacha.
>
> Iska seedha istemaal: **jab kaam aam ho, model pe bharosa kiya ja sakta hai. Jab kaam khaas ho, use jaankari saath bhejni padegi.**
>
> Yeh Chapter 7.6 ka aadha hissa hai.

**3. (jodne wala)** Book 1 Ch 2.1 mein lossy compression thi, jismein woh phenka jaata tha jo aankh ko dikhta nahi. Yahan kya phenka jaata hai?

> **Jawab:** Woh jo dohraya nahi gaya.
>
> Compression mein tay tha ki kya phenkna hai: woh jo aankh nahi pakadti. Insaan ne woh niyam likha tha.
>
> Yahan koi niyam nahi likha gaya. Jo bacha woh isliye bacha ki woh baar baar aaya, aur jo gaya woh isliye gaya ki woh kam aaya.
>
> Aur ek aur farak, jo bada hai: **ek compressed photo ko wapas khola ja sakta hai. Model ko wapas khol kar training data nahi nikala ja sakta.** Woh ek taraf ka rasta hai.
