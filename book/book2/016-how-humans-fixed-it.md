# Chapter 2.8  [SPINE]
## Insaan ne use kaise sudhaara

### Samvaad

**Madhav:** Training khatam. Model agla token bahut achhi tarah guess karta hai. Ab aap usse poochte ho: "meri tabiyat kharaab hai, kya karun?" Woh kya karega?

**Kabir:** Jawab dega.

**Madhav:** Kyun dega? Uska kaam toh agla token guess karna hai. Aur web pe aisi line ke baad aksar kya likha hota hai?

**Kabir:** Shayad aur sawal. Ya ek forum ka agla comment. Ya ek ad.

**Madhav:** Ya woh aur das aise hi sawal likh dega, kyunki sawalon ki list bhi web pe hoti hai.

**Kabir:** Toh woh jawab dega hi nahi zaroori?

**Madhav:** Bilkul nahi. Woh **text poora kar raha hai**, sawal ka jawab nahi de raha. Yeh do bilkul alag kaam hain.

**Kabir:** Toh phir ChatGPT jawab kaise deta hai?

**Madhav:** Yeh sahi sawal hai, aur uska jawab yeh poora chapter hai. Ek aur kadam laga hai, training ke baad. Socho ki kya kiya ja sakta hai.

**Kabir:** Use examples dikha do ki sawal ka jawab kaise dete hain.

**Madhav:** Achha. Kaun banayega woh examples?

**Kabir:** Insaan. Sawal aur uska achha jawab, dono likh do.

**Madhav:** Kitne?

**Kabir:** Hazaaron?

**Madhav:** Aur kharabon nahi?

**Kabir:** Nahi, kyunki yeh haath se likhna padega.

**Madhav:** Bas. Toh yeh kadam chhota hai lekin mehnga hai, kyunki har example ke liye insaan chahiye. Ab problem yeh hai ki hazaaron examples se sab kuch cover nahi hoga. Aur kya kar sakte ho?

**Kabir:** Model se do jawab banwao aur insaan se poocho ki kaunsa behtar hai.

**Madhav:** Yeh likhne se aasan hai?

**Kabir:** Bahut aasan. Chunna likhne se hamesha aasan hai.

**Madhav:** Toh ab aapke paas lakhon tulnaayein ho sakti hain. Aur unse kya karoge?

**Kabir:** Model ko batao ki behtar wale jaise likha kare.

**Madhav:** Seedhe kaise batayenge? Model toh sirf loss samajhta hai.

**Kabir:** Toh ek aur cheez banao jo bataye ki jawab kitna achha hai. Ek number de de.

**Madhav:** Aur woh cheez kahan se aayegi?

**Kabir:** Un tulnaon se. Woh insaan ki pasand seekh legi.

**Madhav:** Aur phir?

**Kabir:** Phir asli model ko us number ko badhane ke liye train karo.

**Madhav:** Aapne poora tareeka bana diya. Ab ek aakhri sawal, aur yeh sabse zaroori hai. Woh number kis cheez ko naapta hai?

**Kabir:** Ki jawab kitna achha hai.

**Madhav:** Nahi. Woh naapta hai ki **un logon ne kis jawab ko pasand kiya.**

**Kabir:** Toh woh sach nahi naap raha.

**Madhav:** Bilkul nahi. Aur agar ek jawab achha lagta ho lekin galat ho?

**Kabir:** Toh woh usi taraf jhukega.

**Madhav:** Yaad rakhna. Yeh aage bahut kuch samjhata hai.

### Naam

Training ke baad do aur kadam lagte hain:

```
1.  INSAAN KE LIKHE EXAMPLES
    hazaaron sawal-jawab, haath se likhe
    model seekhta hai ki jawab dena kya hota hai
    (yahin se woh "sahayak" wali shakal aati hai)

2.  INSAAN KI PASAND SE SUDHAAR
    model do jawab deta hai, insaan behtar chunta hai
    us pasand se ek "score dene wali" cheez banti hai
    phir model us score ko badhane ke liye train hota hai
```

Doosre kadam ka naam **RLHF** hai: insaan ki pasand se seekhna.

Ab teen baatein jo iss chapter ki jaan hain.

**Ek: yeh kadam hi "sahayak" banata hai.**

Bina iske model ek text poora karne wali cheez hai. Woh sawal ka jawab de bhi sakta hai aur aur sawal bhi likh sakta hai. Woh jo shaili aapko dikhti hai, woh training se nahi, iss kadam se aati hai.

**Do: woh sach ke liye nahi, pasand ke liye train hota hai.**

Yeh sabse zaroori line hai. Insaan ne yeh nahi chuna ki kaunsa jawab sach hai. Unhone chuna ki kaunsa **behtar laga**.

Aur inn dono mein farak hai:

```
insaan ko pasand aata hai        aur sach nahi hota
─────────────────────────────────────────────────
aatmvishwas se kaha gaya jawab   galat ho sakta hai
saaf, achhi tarah likha jawab    galat ho sakta hai
woh jawab jo aap sunna chahte ho galat ho sakta hai
lamba, poora dikhne wala jawab   galat ho sakta hai
```

Isliye model **aatmvishwas se galat** hone ki taraf jhukta hai, aur woh jhukav humne khud daala hai.

**Teen: yahin se woh "meetha" pan bhi aata hai.**

Woh aapse zyada sehmat hota hai. Woh aapki taareef karta hai. Woh mushkil se mana karta hai.

Yeh sab isliye hai ki insaan ne un jawabon ko chuna. Iska naam bhi pad gaya hai: **sycophancy**, yaani chaploosi. Aur woh koi bug nahi hai. Woh us cheez ka seedha nateeja hai jo naapi gayi thi.

Chapter 2.4 wala jumla, ab poora: **jo aap naapte ho wahi aapko milta hai.** Aur yahan humne "insaan ko pasand aana" naapa.

### Asli duniya se

2022 ke aakhir mein ChatGPT aaya aur duniya ko lagbhag chaunka diya.

Uske neeche wala model kuch samay se maujood tha. Log usse baat nahi kar rahe the kyunki woh ek text poora karne wali cheez thi, aur usse kaam karwana ek hunar tha.

Jo naya tha woh yeh kadam tha: use jawab dene ke liye dhaala gaya, insaan ki pasand se.

Model lagbhag wahi tha. Yeh parat nayi thi. Aur usi parat ne use ek research ki cheez se ek aisi cheez bana diya jise koi bhi istemaal kar sakta tha.

Yeh dhyaan dene laayak hai: **sabse bada badlav model ki taakat mein nahi tha, uske interface mein tha.** Yeh Book 1 Chapter 8.5 wali baat hai: jeet aksar aasani se aati hai, taakat se nahi.

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki model ki shaili uski soch hai.**

Woh vinamr hai, madad karne wala lagta hai, aur aapse sehmat hota hai. Woh sab iss ek parat se aaya hai, aur woh badla ja sakta hai. Alag company alag pasand chunti hai, aur unke models ka "swabhav" alag lagta hai.

Woh swabhav ek product ka faisla hai, koi andar ki cheez nahi.

Doosri galti: **uski sehmati ko sabooot samajhna.**

Jab aap kehte ho "kya main sahi hoon?" aur woh kehta hai "haan, bilkul," toh woh aksar us cheez ka nateeja hai jise insaanon ne pasand kiya, na ki iss baat ka ki aap sahi ho.

Iska ek seedha, kaam ka nateeja hai: **apna nazariya sawal mein mat daalo.**

```
kamzor    "mujhe lagta hai X sahi hai, kya main sahi hoon?"
behtar    "X ke paksh aur vipaksh mein sabse mazboot tark kya hain?"
```

Doosra sawal usse chaploosi karne ki jagah nahi deta. Yeh Chapter 7.6 ka aadha hissa hai.

### Sochne ke liye

**1. (samajh check)** Bina iss aakhri kadam ke, aap model se poochte ho "Bharat ki rajdhani kya hai?" Kya ho sakta hai?

> **Jawab:** Kuch bhi jo web pe aise vaakya ke baad aata hai.
>
> Woh jawab de sakta hai. Woh aur paanch aise hi sawal likh sakta hai, jaise kisi quiz mein. Woh ek forum ka agla comment likh sakta hai.
>
> Woh galti nahi kar raha. Woh wahi kar raha hai jiske liye use train kiya gaya: text poora karna.
>
> **"Jawab dena" ek alag kaam hai, aur woh baad mein sikhaya gaya.**

**2. (samajh check)** Do models hain. Ek zyada sehmat hota hai, doosra zyada bahas karta hai. Kya doosra kamzor hai?

> **Jawab:** Bilkul nahi. Woh ek alag pasand se dhaala gaya hai.
>
> Sehmat hone wala aksar user surveys mein behtar score karta hai, kyunki log use pasand karte hain.
>
> Aur mushkil kaamon ke liye woh zyada khatarnak hai, kyunki woh aapki galti ko aapke saamne dohra dega.
>
> **Jo model aapko pasand aata hai aur jo model aapko sahi rakhta hai, woh ek nahi hote.** Aur companies ko pehle wale ko chunne ka seedha karobaari kaaran hai.

**3. (jodne wala)** Chapter 2.4 mein tha ki loss sach ko naapta hi nahi. Kya yeh parat use theek kar deti hai?

> **Jawab:** Thodi, aur poori tarah bilkul nahi. Aur wajah gehri hai.
>
> Yeh parat "insaan ko pasand aaya" ko naapti hai, "sach" ko nahi. Woh do cheezein aksar saath chalti hain, isliye model behtar bhi hota hai.
>
> Lekin jahan woh alag ho jaati hain, wahan yeh parat model ko **galat disha** mein le jaati hai: aatmvishwas ki taraf, sehmati ki taraf, aur achhe dikhne wale jawab ki taraf.
>
> Toh sach ki problem hal nahi hui hai. Woh ek parat aage khisak gayi hai.
>
> Yeh Chapter 5.1 aur 5.4 ka aadhaar hai, aur wahi iss kitaab ke sabse practical chapters hain.
