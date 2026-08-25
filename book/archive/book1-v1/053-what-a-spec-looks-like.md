# Chapter 8.3  [SPINE]
## Ek spec kaisa dikhta hai

---

### Samvaad

**Madhav:** Ab aapko kuch banana hai. Aap khud code nahi likhoge. Aap kisi ko batayenge, ya AI se karwayenge. Kya doge unhe?

**Kabir:** Bataunga ki kya banana hai.

**Madhav:** "Ek chat app banao." Bas?

**Kabir:** Nahi. Aur detail chahiye.

**Madhav:** Kitni? Chalo dekhte hain. "Users ek doosre ko message bhej sakein." Kya yeh kaafi hai?

**Kabir:** Nahi. Message kitna lamba? Photo bhej sakte hain?

**Madhav:** Achha. Aur?

**Kabir:** Purane message dikhenge? Kitne?

**Madhav:** Aur?

**Kabir:** Delete kar sakte hain? Sirf apna, ya doosre ka bhi?

**Madhav:** Aur ab sabse zaroori wala sawal, jo lagbhag koi nahi poochta. Agar bhejne mein galti ho jaaye toh kya dikhega?

**Kabir:** Woh... maine socha hi nahi.

**Madhav:** Aur agar internet beech mein chala jaaye?

**Kabir:** Message ruk jaayega. Aur baad mein chala jaayega?

**Madhav:** Ya kho jaayega. Kaunsa chahiye?

**Kabir:** Ruk kar baad mein jaana chahiye.

**Madhav:** Toh use kahin rakhna padega. Aur user ko kya dikhega us beech mein?

**Kabir:** Ek nishaan ki abhi bheja nahi gaya.

**Madhav:** Ab dekho. Humne abhi tak sirf ek cheez ki baat ki hai, message bhejna. Aur usmein paanch faisle nikal aaye.

**Kabir:** Aur woh paanch mein se teen galtiyon ke baare mein the.

**Madhav:** Bas. **Ek spec ka aadha hissa yeh hota hai ki jab cheezein galat ho jaayein tab kya ho.** Aur woh aadha hissa hi hamesha chhoota hai.

**Kabir:** Aur banane wala use khud tay kar leta hai.

**Madhav:** Aur uska tay kiya hua aapke tay kiye hue se alag hoga. Aur woh baad mein pata chalega. Ab aakhri baat. Kaise pata chalega ki kaam poora ho gaya?

**Kabir:** Jab woh chalne lage.

**Madhav:** "Chalne lage" kya hai? Aap kaise jaanchoge?

**Kabir:** Mujhe pehle se likhna padega ki kya kya hona chahiye.

**Madhav:** Toh spec ka aakhri hissa kya hai?

**Kabir:** Yeh ki kaise pata chalega ki ho gaya.

---

### Ek spec ke paanch hisse

```
1. YEH KYUN
   kis insaan ki kaunsi problem hal ho rahi hai
   agar yeh nahi likh sakte, toh baaki sab bekaar hai

2. YEH KYA KARTA HAI
   seedha raasta, kadam ke hisaab se
   user kya karta hai, system kya karta hai

3. YEH KYA NAHI KARTA
   jo cheezein jaan-boojh ke nahi ki ja rahi
   (yeh hissa jitna bada, utna spec achha)

4. JAB GALAT HO TAB KYA
   internet gaya, do log ek saath, data galat,
   cheez mili nahi, ijaazat nahi
   ← yahi sabse zyada chhoota hai aur sabse zyada mayne rakhta hai

5. KAISE PATA CHALEGA KI HO GAYA
   woh cheezein jo jaanchi ja sakti hain
   "achha lagta hai" jaanch nahi hai
```

---

### Ek poora chhota spec

Chat app ka ek hissa, poora likha hua:

```
YEH KYUN
   User apna purana message dhoondhna chahta hai. Abhi use
   haath se scroll karna padta hai, jo mahinon purane chat
   mein lagbhag namumkin hai.

YEH KYA KARTA HAI
   1. User ek shabd likhta hai
   2. System uske apne saare chats mein woh shabd dhoondhta hai
   3. Nateeje naye se purane ke kram mein dikhte hain
   4. Har nateeje mein message aur uske aas-paas ka thoda hissa
   5. Nateeje pe click karo toh us chat mein us jagah pahunch jao

YEH KYA NAHI KARTA
   - photo aur video ke andar nahi dhoondhta
   - group chat mein doosron ke message nahi dhoondhta
   - "milte julte" shabd nahi dhoondhta, sirf wahi shabd
   - hindi aur angrezi ke beech tarjuma nahi karta

JAB GALAT HO TAB KYA
   - kuch nahi mila       →  "kuch nahi mila" dikhao,
                             khaali screen nahi
   - internet nahi hai    →  jo phone pe pehle se hai usmein
                             dhoondho, aur batao ki adhoora hai
   - search dheemi hai    →  2 second baad "dhoondh raha hoon"
                             dikhao, aur rok bhi sako
   - shabd bahut chhota   →  ek akshar pe mat dhoondho,
                             kam se kam do

KAISE PATA CHALEGA KI HO GAYA
   - 10,000 message wale chat mein search 1 second se kam
   - ek aisa shabd jo teen chats mein hai, teeno dikhein
   - nateeje pe click karne se sahi message pe pahuncho
   - internet band karke bhi kuch nateeje aayein
   - ek akshar likhne pe kuch na ho
```

---

### Do baatein jo iss spec mein chhupi hain

**Ek: "yeh kya nahi karta" wala hissa sabse taakatwar hai.**

Usne ek anginat kaam ko ek karne laayak kaam bana diya. Bina uske, "search banao" ka matlab hai photo ke andar dhoondhna, tarjuma karna, milte julte shabd samajhna, aur woh saal bhar ka kaam ho jaata hai.

**Har cheez jo aap saaf-saaf hata dete ho, woh kaam ko chhota karti hai.**

**Do: "jab galat ho tab kya" wala hissa aapke faisle hain, banane wale ke nahi.**

Agar aap nahi likhoge, toh woh kuch na kuch chunega. Aur uska chunav aksar sabse aasan wala hoga: khaali screen, koi message nahi, ya chup-chaap fail.

---

### Asli duniya se ek example

Jab aap kisi AI se kuch banwane ki koshish karte ho, toh yeh farak turant dikhta hai.

"Ek chat app banao" se kuch aisa milta hai jo dikhta toh chat app jaisa hai, aur usmein woh saare faisle kisi aur ne kar liye hain: kya nahi hoga, galat hone pe kya dikhega, kitna bada chalega.

Wahi baat pooray spec ke saath karo, aur nateeja bilkul alag hota hai.

Aur yeh Chapter 8.2 ki baat ko poora karta hai: **AI ne likhne ki keemat giraayi hai. Isliye ab woh hissa jo bacha hai, yaani yeh tay karna ki kya likhwana hai, pehle se zyada mayne rakhta hai, kam nahi.**

Jo aadmi spec likh sakta hai, uske liye AI ek bahut bada guna hai. Jo nahi likh sakta, uske liye AI woh cheez banata hai jo usne maangi thi, aur woh cheez usse chahiye hi nahi thi.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki spec lambi honi chahiye.**

Ek achha spec chhota hota hai aur usmein faisle hote hain. Ek bura spec lamba hota hai aur usmein bas baatein hoti hain.

Agar aapki spec mein "system fast hona chahiye" likha hai, toh usmein kuch bhi nahi likha. "10,000 message mein 1 second se kam" ek faisla hai.

Doosri galti: **seedhe raaste ko poora kaam samajhna.**

Zyadatar spec sirf hissa 2 likhte hain, aur wahi sabse chhota hissa hai. Asli kaam hisse 3 aur 4 mein hai.

Teesri galti: **yeh maan lena ki spec ek baar mein likh li jaayegi.**

Aap likhna shuru karoge aur aadhe sawal aapko tab dikhenge jab aap likh rahe honge. Yehi spec ka asli faayda hai. **Woh sochne pe majboor karti hai, kaagaz pe, code se pehle.**

---

### Sochne ke liye

**1. (samajh check)** Ek spec mein likha hai "user apni profile photo badal sakta hai." Paanch sawal poochho jo iss mein nahi likhe.

> **Jawab:** Kuch aam wale:
>
> Photo ka size kitna bada ho sakta hai? Kaunse tarah ki file? Kya woh kaati jaayegi ya chhoti ki jaayegi? Purani photo hat jaayegi ya rakhi jaayegi? Agar upload beech mein ruk jaaye toh? Agar photo aapatti-janak ho toh? Kitni baar badal sakta hai? Kya doosron ko turant dikhegi ya cache mein purani rahegi?
>
> Aakhri wala dhyaan dene laayak hai, kyunki woh Chapter 5.5 se aata hai. **Naksha jaante ho, toh spec ke sawal apne aap dikhne lagte hain.**

**2. (samajh check)** Aap "yeh kya nahi karta" wale hisse mein das cheezein daal dete ho. Kya yeh spec ko kamzor karta hai?

> **Jawab:** Ulta. Woh use bahut mazboot karta hai.
>
> Har cheez jo aap hata dete ho, woh kaam ko chhota, saaf, aur poora hone laayak banati hai.
>
> Aur woh bahas ko pehle le aati hai. Agar kisi ko lagta hai ki hatai gayi cheez zaroori hai, toh woh abhi bolega, na ki jab kaam ho chuka ho.
>
> **Spec ka sabse mehnga hissa woh hai jo likha hi nahi gaya, kyunki sabne maan liya ki woh saaf hai.**

**3. (jodne wala)** Chapter 7.1 kehta tha ki bug un haalaton mein hote hain jinke baare mein kisi ne socha nahi. Spec ka chautha hissa usse kaise judta hai?

> **Jawab:** Woh seedha uska ilaaj hai.
>
> Chautha hissa aapko majboor karta hai ki galat haalaton ko pehle sochein, banane se pehle, na ki tab jab woh asli mein ho jaayein.
>
> Woh saari haalatein nahi pakadta, kyunki woh anginat hain. Lekin woh sabse aam wali pakad leta hai: internet gaya, cheez mili nahi, ijaazat nahi, do log ek saath, data galat.
>
> Aur woh ek aur kaam bhi karta hai: **jo haalatein aap likh dete ho, unka jawab ab ek faisla hai, ek durghatna nahi.**
