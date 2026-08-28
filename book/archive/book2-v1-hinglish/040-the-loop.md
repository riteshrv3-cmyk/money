# Chapter 6.4  [SPINE]
## The loop

### Samvaad

**Madhav:** Ab tak: model likhta hai, program kaam karta hai, nateeja wapas aata hai. Uske baad kya?

**Kabir:** Model jawab de deta hai.

**Madhav:** Aur agar kaam poora nahi hua? Maan lo aapne kaha "meri saari purani chat mein doctor ka zikr dhoondho aur ek summary banao."

**Kabir:** Pehle dhoondhna padega. Phir padhna. Phir likhna.

**Madhav:** Kitne kadam?

**Kabir:** Teen ya chaar.

**Madhav:** Toh ek tool call kaafi nahi hai.

**Kabir:** Nahi. Uske baad model ko dekhna padega ki kya mila, aur phir agla kadam chunna padega.

**Madhav:** Toh kya karna padega?

**Kabir:** Poora chakkar dobara chalao. Nateeje ke saath.

**Madhav:** Kitni baar?

**Kabir:** Jab tak kaam poora na ho.

**Madhav:** Kaun tay karega ki poora hua?

**Kabir:** Model. Woh keh dega ki bas, ab jawab yeh hai.

**Madhav:** Aur agar woh kabhi na kahe?

**Kabir:** Toh woh chalta rahega.

**Madhav:** Hamesha?

**Kabir:** Toh ek seema lagani padegi. Bees kadam ke baad rok do.

**Madhav:** Bas. Ab yeh dekho: har kadam pe context mein kya jud raha hai?

**Kabir:** Model ka likha, aur tool ka nateeja.

**Madhav:** Toh bees kadam ke baad?

**Kabir:** Context bahut bhar chuka hoga.

**Madhav:** Aur phir?

**Kabir:** Shuruaat katni padegi. Aur usmein mera asli sawal tha.

**Madhav:** Toh bees kadam baad woh kya kar raha hoga?

**Kabir:** Woh bhool chuka hoga ki karna kya tha.

**Madhav:** Yeh agents ki sabse aam nakaami hai. Ab ek aur. Kadam paanch pe usne ek chhoti galti ki. Kadam chhe pe kya hoga?

**Kabir:** Woh us galti ke upar aage badhega.

**Madhav:** Aur kadam bees pe?

**Kabir:** Woh bahut door ja chuka hoga, galat disha mein.

**Madhav:** Aur kya use pata chalega?

**Kabir:** Nahi. Kyunki uske liye ab wahi galti hi sachai hai.

**Madhav:** Toh do problem hain aur dono ek hi cheez se aati hain.

**Kabir:** Ki har kadam pichhle pe khada hai.

### Naam

Us dohrav ko **agent loop** kehte hain:

```
1.  model dekhta hai: kaam, aur ab tak kya hua
2.  woh tay karta hai: agla kadam kya hai
3.  program woh kadam chalata hai
4.  nateeja context mein judta hai
5.  wapas 1 pe

    rukta hai jab: model kahe ki ho gaya
                   ya seema aa jaaye
                   ya koi insaan roke
```

**Ek agent iske alaawa kuch nahi hai.** Ek model, kuch tools, aur ek dohrav. Bas.

Yeh sunne mein chhota lagta hai aur uska asar bada hai, kyunki ab woh cheez ek kadam ki jagah pachaas kadam chal sakti hai.

Ab teen baatein jo har agent mein mayne rakhti hain.

**Ek: context har kadam pe bharta hai.**

Model ka likha, tool ka nateeja, phir agla, phir agla. Bees kadam baad woh bahut bada ho chuka hota hai, aur shuruaat kat ne lagti hai (Ch 4.4).

Aur shuruaat mein hi aapka asli kaam likha tha.

**Isliye achhe agents apna asli lakshya baar baar dohraate hain**, har kadam pe, taaki woh kate nahi.

**Do: galtiyan jud ti jaati hain.**

Har kadam pichhle ko sach maan kar aage badhta hai. Ek chhoti galti kadam paanch pe, kadam bees tak ek badi galti ban chuki hoti hai.

Aur model apni galti khud nahi pehchan sakta (Ch 5.2). Toh woh apne aap wapas nahi aayega.

Isliye har kadam pe bahar se jaanch honi chahiye, jahan mumkin ho: code chala kar dekho, file dekho, nateeja milaao. Chapter 5.4 ka niyam, ab har kadam pe.

**Teen: seema hamesha honi chahiye.**

Kadamon ki seema, waqt ki seema, aur paise ki seema. Kyunki ek loop jo galat disha mein chal pada hai, woh apne aap nahi rukega. Woh sirf mehnga hota jaayega.

### Asli duniya se

Iss loop ka sabse dikhne wala roop woh AI hai jo code likhta hai aur chalata hai.

Woh code likhta hai, chalata hai, error dekhta hai, theek karta hai, dobara chalata hai. Yeh loop kai baar chalta hai, aur aksar sahi jawab pe pahunch jaata hai.

Aur dhyaan do ki yeh yahan itna achha kyun chalta hai: **kyunki har kadam pe ek asli, bahar se jaanch hai.** Code chalta hai ya nahi. Test paas hota hai ya nahi.

Ab isse tulna karo ek aise agent se jo aapke liye "market research" karta hai. Wahan har kadam pe jaanch kya hai? Kuch nahi. Woh bees kadam chal sakta hai aur pura galat ho sakta hai, aur kisi ko pata nahi chalega.

**Isliye agents un kaamon mein achhe chalte hain jinme har kadam jaancha ja sake, aur un mein kharaab jinme nahi.**

Yeh ek pakka, kaam ka niyam hai. Aur woh Book 1 Chapter 8.2 se seedha aata hai: **jinka sahi jawab saaf hai woh kaam aasan hain, jinka dhundhla hai woh mushkil.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki agent ke andar koi plan hai.**

Koi plan kahin rakha hua nahi hai. Har kadam pe woh poora context dobara padhta hai aur agla kadam chunta hai.

Agar plan kahin hai, toh woh us likhawat mein hai jo ab tak ban chuki hai. Aur agar woh likhawat bhatak gayi, toh plan bhi bhatak gaya.

Doosri galti: **yeh maan lena ki zyada kadam matlab behtar nateeja.**

Aksar ulta hota hai. Har kadam ek aur mauka hai bhatakne ka, aur context ka bharna. Ek agent jo teen kadam mein kaam karta hai, aksar us se behtar hai jo tees mein karta hai.

Teesri galti: **agent ko woh kaam dena jismein koi jaanch nahi hai.**

Woh chalta rahega, aatmvishwas ke saath, aur aakhir mein ek poora jawab dega. Aur aapke paas yeh jaanne ka koi tareeka nahi hoga ki woh kadam saat pe hi galat ho gaya tha.

### Sochne ke liye

**1. (samajh check)** Aapka agent bees kadam baad bhool jaata hai ki karna kya tha. Do ilaaj batao.

> **Jawab:**
>
> **Ek:** asli kaam har kadam pe dobara likho, taaki woh kabhi kate nahi. Yeh sabse saada aur sabse asardar ilaaj hai.
>
> **Do:** kaam ko chhote hisson mein todo, aur har hisse ke liye alag loop chalao, saaf shuruaat ke saath.
>
> Doosra behtar hai jab kaam bada ho, kyunki chhota loop kam bhatakta hai.
>
> **Aur ek teesra jo aksar bhula diya jaata hai:** kam kadam ka lakshya rakho. Har hataya gaya kadam ek hataya gaya khatra hai.

**2. (samajh check)** Ek agent code likhta hai aur ek agent "business plan" banata hai. Kaunsa zyada bharosemand hoga, aur kyun?

> **Jawab:** Code wala, aur wajah model mein nahi hai.
>
> Code mein har kadam pe ek asli jaanch hai: woh chalta hai ya nahi, test paas hota hai ya nahi. Galti turant dikhti hai aur agla kadam use theek kar sakta hai.
>
> Business plan mein koi jaanch nahi hai. Har kadam theek dikhta hai, aur bees kadam baad bhi theek dikhta hai, chahe woh poora galat ho.
>
> **Agent ki bharosemandi kaam ki jaanch se aati hai, model ki taakat se nahi.**

**3. (jodne wala)** Book 1 Ch 8.4 mein tha ki thoda badlo, dekho, phir aage badho. Kya woh yahan lagta hai?

> **Jawab:** Bilkul lagta hai, aur agents mein woh sabse zyada zaroori hai.
>
> Ek agent jo bees kadam chala kar aakhir mein sab kuch dikhata hai, woh us badlav jaisa hai jo ek saath sab jagah laga diya gaya.
>
> Ek agent jo har teen kadam pe rukta hai aur dikhata hai ki ab tak kya hua, woh us badlav jaisa hai jo thoda thoda karke lagta hai.
>
> Aur Book 1 ka doosra niyam bhi lagta hai: **wapas jaane ka raasta pehle banao.** Agent file badalne wala hai? Pehle copy rakh lo. Chapter 6.3 ka wahi sabak, ab loop ke saath.
