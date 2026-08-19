# Chapter 6.8  [SPINE]
## Yeh sab chalane ka kharcha kitna hai

---

### Samvaad

**Madhav:** Ab ek sawal jo iss kitaab mein pehli baar poocha ja raha hai. Yeh sab chalane mein paisa kitna lagta hai?

**Kabir:** Pata nahi. Server mehnge honge.

**Madhav:** Ek chhota server, jo ek chhoti site ke liye kaafi hai, mahine ka lagbhag paanch se bees dollar. Yeh sasta hai ya mehnga?

**Kabir:** Sasta.

**Madhav:** Ab ek text message rakhne ka kharcha. Ek message lagbhag 100 byte hai. Ek GB mein kitne messages?

**Kabir:** Ek GB matlab sau karod byte. Toh ek karod messages.

**Madhav:** Aur ek GB rakhne ka kharcha mahine ka lagbhag do rupaye.

**Kabir:** Toh ek karod messages, do rupaye mahina?

**Madhav:** Bas. Ab photos. Ek photo lagbhag 3 MB. Ek GB mein kitni?

**Kabir:** Lagbhag 300.

**Madhav:** Toh 300 photos ka kharcha utna hi hai jitna ek karod messages ka.

**Kabir:** Tees hazaar guna zyada.

**Madhav:** Ab video. Ek ghanta lagbhag 1 GB. Toh ek ghante ka video ek karod messages ke barabar hai.

**Kabir:** Yeh farak toh maine socha hi nahi tha.

**Madhav:** Isiliye har text wala app lagbhag muft chal sakta hai aur har video wala app paisa maangta hai. Ab ek aur cheez. Data rakhna sasta hai. Data **bhejna** kitna mehnga hai?

**Kabir:** Woh alag hai?

**Madhav:** Bilkul alag, aur yahi sabse badi jaal hai. Cloud pe data andar laana aksar muft hai. Bahar bhejna paisa leta hai, aur woh rakhne se kai guna mehnga hai.

**Kabir:** Kyun?

**Madhav:** Karobaari wajah hai. Andar aana sasta rakho taaki log aayein, aur bahar jaana mehnga rakho taaki jaana mushkil ho.

**Kabir:** Woh lock-in hai, Chapter 6.5 wala.

**Madhav:** Bilkul. Ab aakhri hissa, aur yeh sabse bada hai. Ek server mahine ka bees dollar ka hai. Aur ek engineer?

**Kabir:** Bahut zyada.

**Madhav:** India mein ek achha engineer mahine ka lagbhag ek se do lakh rupaye. Yaani hazaar se do hazaar dollar. Kitne servers ke barabar?

**Kabir:** Sau se do sau server.

**Madhav:** Toh agar aap ek engineer ka ek mahina lagakar server ka kharcha aadha kar dete ho, aur aapke paas das server hain, toh?

**Kabir:** Toh maine faayde se bees guna zyada kharch kar diya.

**Madhav:** Bas. Yeh sabse aam galti hai jo chhoti companies karti hain: machine ka paisa bachane ke liye aadmi ka waqt jala dena.

---

### Naam

Lagbhag mote andaze, taaki paimana dimaag mein baithe:

```
CHHOTA SERVER          mahine ke $5 - $20
BADA SERVER            mahine ke $200 - $2,000
DATA RAKHNA            ~$0.02 per GB per mahina
DATA BAHAR BHEJNA      ~$0.05 - $0.12 per GB   ← rakhne se kai guna
DOMAIN NAAM            saal ke $10 - $15
EK ENGINEER            mahine ke $1,000 - $10,000+
```

Ab isse teen niyam nikalte hain, aur teeno kaam ke hain.

**Ek: likhawat lagbhag muft hai, dekhne-sunne wali cheezein mehngi.**

```
1 karod text message   ≈  2 rupaye mahina
300 photos             ≈  2 rupaye mahina
1 ghanta video         ≈  2 rupaye mahina
```

Isiliye jo product likhawat pe khada hai woh aksar muft chal sakta hai, aur jo video pe khada hai woh kabhi muft nahi ho sakta.

**Do: bhejna rakhne se mehnga hai.**

Ek video jo ek baar rakha gaya aur das lakh baar dekha gaya, uska kharcha rakhne mein nahi, bhejne mein hai. Isiliye CDN (Chapter 5.5) sirf speed ke liye nahi hai, woh paise ke liye bhi hai.

**Teen: aadmi ka waqt machine se bahut mehnga hai.**

Yeh sabse zaroori niyam hai aur sabse zyada toda jaata hai. Ek engineer ka ek mahina sau server ke barabar hai. Isliye "yeh cheez thodi mehngi hai lekin isse kaam aasan ho jaata hai" lagbhag hamesha sahi sauda hai, jab tak paimana bahut bada na ho jaaye.

Aur yahin Chapter 6.5 ka cloud wala sawal apne aap hal ho jaata hai. Cloud per machine mehnga hai. Lekin agar woh ek aadmi ka mahina bacha deta hai, toh usne apna daam kai baar chuka diya.

---

### Asli duniya se ek example

WhatsApp ke paas 2014 mein 55 log the aur lagbhag 45 crore users. Yeh Chapter 0.2 mein leverage ke udaharan mein aaya tha.

Ab usi ko kharche ke nazariye se dekho.

Unka product lagbhag poori tarah likhawat pe khada tha. Text message. Woh sabse sasti cheez hai jo koi bhi rakh aur bhej sakta hai.

Unhone jaan-boojh ke bahut kam cheezein rakhi thin. Messages phone pe pahunchte hi server se hata diye jaate the.

Agar unka product video pe khada hota, toh wahi 45 crore users ka kharcha kai hazaar guna zyada hota, aur 55 log usse kabhi nahi chala paate.

**Woh 55 ki ginti sirf achhe engineering se nahi aayi. Woh product ki shakal se aayi.** Jo cheez woh bech rahe the, uska kharcha hi lagbhag zero tha.

Yeh soch ne laayak hai jab aap kuch banane ki soch rahe ho: **aap kaunsi cheez rakh aur bhej rahe ho, aur uska kharcha kaise badhega jab log das guna ho jaayein?**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki technology ka kharcha machinon mein hai.**

Lagbhag har software company mein sabse bada kharcha log hain, machinein nahi. Aksar teen-chauthai se zyada.

Iska seedha nateeja: log mahinon lagakar machine ka kharcha aadha karte hain aur us mehnat mein us bachat se zyada kharch kar dete hain.

Doosri galti: **yeh maan lena ki "muft" wala product sach mein muft hai.**

Har muft cheez ka kharcha koi utha raha hai. Chapter 3.6 mein hum poochh chuke hain: **kaun utha raha hai, aur badle mein kya le raha hai?**

Aur jab aap dekhte ho ki ek product bahut mehngi cheez muft de raha hai, jaise unlimited video, toh do mein se ek baat sach hai: ya toh unhe kahin aur se bahut paisa mil raha hai, ya woh chal nahi payega.

Teesri galti: sirf aaj ka kharcha dekhna. Sahi sawal hai: **jab yeh sau guna bada hoga tab yeh kharcha kaise badhega?** Kuch kharche users ke saath seedha badhte hain aur kuch lagbhag nahi badhte. Farak wahin se aata hai ki koi karobaar chal sakta hai ya nahi.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  KHARCHA      likhawat sasti,           │  ← naya
    │               video mehnga              │
    │               bhejna > rakhna           │
    │               aadmi >> machine          │
    ├────────────────────────────────────────┤
    │  CLOUD, SHRINKHLA, API, UPTIME          │
    ├────────────────────────────────────────┤
    │  QUEUE, CACHE, DATABASE, INTERNET       │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Do app hain. Ek mein log text likhte hain, doosre mein video daalte hain. Dono ke ek lakh users hain. Kharche mein kitna farak hoga?

> **Jawab:** Hazaaron guna.
>
> Text wala app ek chhote server aur thodi si jagah mein chal jaayega. Uska kharcha mahine ka kuch hazaar rupaye ho sakta hai.
>
> Video wala app har user ke har video ko rakhega aur har dekhne pe bhejega. Lakhon rupaye mahina, aasani se.
>
> Aur isiliye unke karobaar bhi bilkul alag honge. Text wala app dher saare muft users rakh sakta hai. Video wale app ko shuru se hi paise ka koi raasta chahiye.
>
> **Product ki shakal uske karobaar ki shakal tay kar deti hai.**

**2. (samajh check)** Aapka cloud ka bill dekhne pe pata chalta hai ki sabse bada hissa "data transfer" hai, machinein nahi. Kya ho raha hai?

> **Jawab:** Aap bahut data bahar bhej rahe ho, aur woh rakhne se kai guna mehnga hai.
>
> Aam wajah: bade photos ya video har baar server se seedha bheje ja rahe hain, bina kisi paas wali copy ke.
>
> Ilaaj CDN hai. Woh cheez ek baar bahar bhejta hai aur uske baad copies se deta hai, jo sasta bhi hai aur tez bhi.
>
> Yeh dhyaan dene laayak hai: **ek hi hal aksar do alag problem solve karta hai.** CDN Chapter 5.5 mein speed ke liye aaya tha, aur yahan paise ke liye wapas aa gaya.

**3. (jodne wala)** Chapter 0.2 ka formula tha: size x scarcity x leverage. Iss chapter ke numbers usmein kahan lagte hain?

> **Jawab:** Woh leverage wale dial ko naapne ka tareeka dete hain.
>
> Ravi ka kaam har baar khatam ho jaata tha. Anil ki naali ek baar bani aur chalti rahi.
>
> Software mein woh sawal aise dikhta hai: **jab ek aur user aata hai, toh mera kharcha kitna badhta hai?**
>
> Agar lagbhag zero badhta hai, jaise text wale app mein, toh leverage bahut upar hai. Ek baar banao, das lakh ko do.
>
> Agar har user ke saath seedha badhta hai, jaise video ya kisi aadmi ki mehnat wale kaam mein, toh leverage kam hai, chahe cheez technology hi kyun na ho.
>
> Aur yahin Chapter 0.3 ki chetavni sach nikalti hai: **level 3 pe hone se leverage apne aap nahi milta.** Woh iss baat se aata hai ki agla user aapko kya kharcha deta hai.
