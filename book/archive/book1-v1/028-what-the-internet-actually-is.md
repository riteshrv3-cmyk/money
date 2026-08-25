# Chapter 4.7  [SPINE]
## Internet actually hai kya

---

### Samvaad

**Madhav:** Internet kahan hai?

**Kabir:** Hawa mein? Cloud mein?

**Madhav:** Tumhara packet hawa se guzarta hai?

**Kabir:** Nahi. Taar se. Wifi thodi door tak hawa mein, phir taar.

**Madhav:** Aur samundar paar?

**Kabir:** Samundar ke neeche taar hote hain.

**Madhav:** Bilkul. Lagbhag saara internet dhaatu aur kaanch ke taar hain, zameen aur samundar ke neeche. Ab agla sawal. Woh taar kiske hain?

**Kabir:** Internet company ke?

**Madhav:** Kaunsi? Duniya mein hazaaron hain.

**Kabir:** Toh sabke apne apne hisse honge.

**Madhav:** Aur woh hisse aapas mein jude kaise?

**Kabir:** Kisi ne unhe joda hoga.

**Madhav:** Kisne? Koi sarkar? Koi company?

**Kabir:** Pata nahi.

**Madhav:** Do companies apne taar aapas mein isliye jodti hain kyunki dono ko faayda hai. Mere users ko tumhare tak pahunchna hai, tumhare mere tak. Woh aapas mein baat karke tay kar leti hain.

**Kabir:** Toh koi bada plan nahi hai?

**Madhav:** Koi nahi. Har jodi apna hisaab lagati hai. Poora internet un hazaaron alag-alag samjhauton ka jod hai.

**Kabir:** Toh phir woh chalta kaise hai? Kisi ko poora naksha toh pata hona chahiye.

**Madhav:** Kisi ko nahi pata. Ab yeh dhyaan se socho. Tumhara packet nikalta hai aur use bees machinein paar karni hain. Kya pehli machine ko poora raasta pata hai?

**Kabir:** Hona chahiye.

**Madhav:** Zaroorat kya hai? Use sirf itna pata ho ki agla kadam kaunsa hai.

**Kabir:** Aur agli machine ko uska agla kadam.

**Madhav:** Bas. Koi bhi poora raasta nahi jaanta. Har ek sirf itna jaanta hai ki iss disha ke liye agla kaun hai.

**Kabir:** Aur agar beech ka koi taar toot jaaye?

**Madhav:** Kya hoga, socho.

**Kabir:** Uske padosi ko pata chal jaayega ki woh raasta nahi hai. Woh doosra raasta chun lega.

**Madhav:** Aur woh baat kaise phailegi?

**Kabir:** Har ek apne padosi ko batayega.

**Madhav:** Toh poora jaal khud ko theek kar leta hai, bina kisi upar wale ke. Ab batao, internet band karne ke liye kya karna padega?

**Kabir:** Poora... sab kuch band karna padega. Ek jagah band karne se woh raasta badal lega.

**Madhav:** Isiliye woh aise banaya hi gaya tha. Aur ab ek aakhri sawal. Agar koi maalik nahi hai, koi manager nahi hai, koi poora naksha nahi hai, toh internet ko ek cheez kya banata hai?

**Kabir:** Sirf yeh ki sab ek hi niyam maan rahe hain.

**Madhav:** Bas. Internet koi cheez nahi hai. Woh ek sehmati hai.

---

### Naam

Internet ka ek line mein matlab:

> **Alag-alag maalikon ke jaal, jo ek doosre se isliye jude hain ki dono ko faayda hai, aur jo sirf isliye ek saath kaam karte hain ki sab ek hi protocol maante hain.**

Woh cheez jismein har machine sirf agla kadam jaanti hai, use **routing** kehte hain. Aur woh tareeka jisse padosi ek doosre ko batate hain ki kahan se kya pahuncha ja sakta hai, use **BGP** kehte hain.

Poori tasveer, neeche se upar:

```
TAAR          zameen aur samundar ke neeche, kisi ka apna maal
PATA          har machine ko ek nishaan (Ch 4.2)
PACKET        bada sandesh tukdon mein (Ch 4.3)
ROUTING       har machine sirf agla kadam jaanti hai
PROTOCOL      sab ek hi niyam maante hain (Ch 4.4)
NAAM          insaan ke liye naam, machine ke liye number (Ch 4.5)
TAALA         raaste mein koi padh na sake (Ch 4.6)
```

In saaton mein se ek bhi kisi ek maalik ka nahi hai.

Aur ab woh cheez jo iss poore part ka nichod hai:

**Internet ka koi centre nahi hai, isliye use band karna mushkil hai. Lekin uske kuch jode aise hain jinpe bahut kuch tika hai, aur woh kuch haathon mein hain.** Naam ki jad. Samundar ke neeche ke bade taar. Bharose wali list jo aapke phone mein pehle se hai.

"Koi maalik nahi hai" aur "taakat sab jagah barabar hai" do alag baatein hain. Pehli sach hai, doosri nahi.

---

### Asli duniya se ek example

Internet ki neev 1960 ke dashak mein padi thi, aur uske peeche ek khaas soch thi: aisa jaal banao jo tukde-tukde hone par bhi chalta rahe. Ek beech ka daftar nahi, kyunki beech ka daftar ek nishana hota hai.

Us soch ka nateeja aaj bhi dikhta hai. Jab samundar ke neeche ka koi bada taar toot jaata hai, aur woh har saal kai baar hota hai, toh poore desh ka internet band nahi hota. Woh dheema ho jaata hai, kyunki traffic lambe raaston se ghoom kar jaata hai.

Aur ulta bhi hua hai. Kuch mauke aise aaye jab kisi ek company ne galti se yeh keh diya ki "ye saare pate mere paas hain," aur uske padosiyon ne maan liya, aur duniya ka bada hissa traffic galat jagah pahunch gaya.

Kyunki BGP mein padosi ek doosre pe bharosa karte hain. Koi upar wala jaanch nahi karta. Poora internet, aaj bhi, kaafi hadd tak iss baat pe khada hai ki log sach bolenge.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki internet kisi ek jagah hai.**

Log "cloud" sunkar aasman jaisa kuch sochte hain. Cloud kisi ki building mein rakhi machinein hain, kisi sheher mein, bijli aur AC ke saath. Aap uska pata Google Maps pe dekh sakte ho.

Iska seedha nateeja: log samajh nahi paate ki unka data kis desh mein pada hai, kaunse kanoon uspe lagte hain, aur ek building mein aag lagne se unki cheezein kyun ja sakti hain.

Aur doosri taraf ka galat samajh bhi utna hi aam hai: yeh sochna ki internet itna failaa hua hai ki uspe kisi ka bas nahi. Bas chalta hai. Poore desh ka internet band kiya ja chuka hai, kai baar, kyunki ek desh ke andar aksar gine-chune taar hote hain jo bahar jaate hain.

Sahi tasveer beech mein hai: **koi ek maalik nahi hai, lekin gine-chune jode hain jahan bahut kuch tika hai.**

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  INTERNET     koi maalik nahi           │  ← naya
    │               har machine sirf agla     │
    │               kadam jaanti hai          │
    │               ek sehmati, ek cheez nahi │
    ├────────────────────────────────────────┤
    │  TAALA, NAAM, PROTOCOL, PACKET, PATA    │
    ├────────────────────────────────────────┤
    │  OS, PROCESS, CPU, RAM/DISK, SWITCH     │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek samundar ke neeche ka taar toot jaata hai. Poore desh ka internet band ho jaayega?

> **Jawab:** Lagbhag kabhi nahi. Woh dheema ho jaayega.
>
> Kyunki har machine ko sirf agla kadam pata hai, aur woh badla ja sakta hai. Traffic doosre raaste se ghoom kar jaata hai, jo lamba hai, isliye latency badh jaati hai.
>
> Lekin agar ek desh mein sirf ek ya do taar bahar jaate hon, toh yeh sach mein poora band kar sakta hai. Isiliye ek desh ka internet kitna mazboot hai, yeh uske bahar jaane wale raaston ki ginti pe tikta hai.

**2. (samajh check)** Internet mein koi manager nahi hai. Toh kya kuch bhi band nahi kiya ja sakta?

> **Jawab:** Kiya ja sakta hai, aur teen jagahon se aksar kiya jaata hai.
>
> **Naam:** naam hata do, cheez pahunch se bahar ho jaati hai, chahe machine chal rahi ho.
>
> **Raasta:** internet company apne yahan se us pate tak jaana band kar de.
>
> **Machine:** jis company ke server pe cheez rakhi hai, woh use hata de.
>
> Dhyaan do ki teeno mein se koi bhi "internet" ko band nahi kar raha. Har ek kisi ek jode ko kaat raha hai. Aur teeno jode kisi na kisi ke haath mein hain.

**3. (jodne wala)** Chapter 4.1 mein Kabir ne kaha tha ki network ki value judav mein hai. Ab yeh chapter kehta hai ki internet ek sehmati hai. Dono ko jodo.

> **Jawab:** Judav sirf taar se nahi banta. Woh sehmati se banta hai.
>
> Do machinein taar se judi ho sakti hain aur phir bhi ek doosre ko na samajh paayein, agar dono alag niyam maan rahi hon.
>
> Toh asli judav protocol mein hai, dhaatu mein nahi.
>
> Aur isse ek gehri baat nikalti hai jo Chapter 8.5 mein poori khulegi: **network wali duniya mein sabse badi taakat cheez banane wale ke paas nahi hoti. Woh us niyam ke paas hoti hai jise sab maan lete hain.**
