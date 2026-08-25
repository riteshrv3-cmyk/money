# Chapter 7.3  [SPINE]
## Har badlav ka record

---

### Samvaad

**Madhav:** Aap ek file pe kaam kar rahe ho. Kal aapne kuch badla aur aaj sab kuch toot gaya. Kya karoge?

**Kabir:** Wapas purana kar dunga.

**Madhav:** Purana kahan hai?

**Kabir:** Maine copy bana li thi. `file-purani.txt`.

**Madhav:** Aur uske pehle wali?

**Kabir:** `file-purani-2.txt`?

**Madhav:** Aur teen hafte pehle wali? Jo us din chal rahi thi jab sab theek tha?

**Kabir:** Woh nahi hai.

**Madhav:** Toh pehla sawal: har haalat kabhi bhi wapas mil sake. Kya rakhna padega?

**Kabir:** Har badlav.

**Madhav:** Poori file har baar?

**Kabir:** Woh bahut jagah legi.

**Madhav:** Toh?

**Kabir:** Sirf farak rakhun. Chapter 2.1 wali compression jaisi baat.

**Madhav:** Bas. Ab doosra sawal. Do log ek hi file pe kaam kar rahe hain. Kya hoga?

**Kabir:** Wahi purani problem. Ek doosre ke upar likh denge.

**Madhav:** Chapter 5.4 mein iska hal taala tha. Kya yahan taala theek hai?

**Kabir:** Toh ek aadmi kaam kare aur doosra baitha rahe. Ghanton tak.

**Madhav:** Toh?

**Kabir:** Dono kaam karein, apni apni copy pe, aur baad mein mila lein.

**Madhav:** Milane mein kya hoga?

**Kabir:** Agar dono ne alag jagah badla toh dono jud jaayenge.

**Madhav:** Aur agar dono ne ek hi line badli?

**Kabir:** Toh machine tay nahi kar sakti. Kisi insaan ko dekhna padega.

**Madhav:** Bas. Ab teesra sawal, aur yeh sabse kaam ka hai. Aapko ek nayi cheez try karni hai, jo shayad kaam na kare. Aur asli cheez chalti rehni chahiye.

**Kabir:** Toh main ek alag copy pe kaam karunga.

**Madhav:** Aur agar woh kaam kar gayi?

**Kabir:** Toh use asli mein mila dunga.

**Madhav:** Aur nahi kar gayi?

**Kabir:** Toh phenk dunga. Asli ko kuch nahi hua.

**Madhav:** Ab batao, isse kya mila?

**Kabir:** Main koshish kar sakta hoon bina kuch todne ke darr ke.

**Madhav:** Aur jab darr nahi hota toh?

**Kabir:** Toh main zyada koshish karta hoon.

---

### Naam

Us poori cheez ka naam hai **version control**, aur jo lagbhag sab log istemaal karte hain uska naam hai **git**.

Uske teen bade kaam wahi hain jo Kabir ne nikaale:

```
1. ITIHAAS       har badlav ka record, hamesha ke liye
                 kabhi bhi kisi bhi purani haalat pe wapas

2. MILAANA       kai log alag alag kaam karein, phir mila lein
                 jahan takraav ho wahan insaan tay kare

3. SHAKHA        nayi cheez alag jagah try karo
                 chal gayi toh mila do, nahi toh phenk do
```

Har record ke saath yeh bhi likha hota hai: kisne badla, kab badla, aur kyun badla.

Woh teesri baat sabse zyada nazarandaaz hoti hai aur sabse zyada kaam aati hai. Do saal baad jab koi poochta hai "yeh line yahan kyun hai," toh jawab record mein hota hai.

Aur ab woh baat jo iss chapter ki asli seekh hai:

**Version control ka asli faayda purani cheez wapas laana nahi hai. Woh himmat hai.**

Jab aap jaante ho ki kuch bhi wapas kiya ja sakta hai, toh aap koshish karte ho. Aap purani cheezein saaf karte ho. Aap badi cheezein badalte ho.

Bina uske, har badlav ek daanv hai, aur log daanv nahi lagate. Woh chhote chhote patch lagate hain, aur software dheere dheere aisa ho jaata hai jise koi chhoona nahi chahta.

Yeh wahi baat hai jo Chapter 7.2 mein jaanch ke baare mein thi. Dono ek hi cheez dete hain: **jaal, taaki aap kood sako.**

---

### Asli duniya se ek example

Git 2005 mein Linus Torvalds ne banaya tha, wahi jisne Linux banaya (Chapter 3.6).

Wajah yeh thi ki Linux pe duniya bhar mein hazaaron log kaam karte the, jo ek doosre ko jaante nahi the aur ek doosre pe bharosa nahi karte the. Us waqt ka koi bhi tool itne logon ke liye nahi bana tha.

Usne use lagbhag do hafte mein likha.

Aaj woh lagbhag har software company mein hai, aur woh muft hai.

Ab Chapter 3.6 ke chaar wajahon pe lagao: usne ise isliye banaya ki use khud chahiye tha aur mil nahi raha tha. Chauthi wajah. Aur uska asar aaj lagbhag har programmer pe roz padta hai.

Chapter 0.2 ke dials: leverage kalpana se bahar, paisa lagbhag zero. Wahi shakal jo Chapter 4.8 mein protocol likhne walon ki thi.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki version control sirf code ke liye hai.**

Woh kisi bhi aisi cheez ke liye hai jo badalti hai aur jiska itihaas mayne rakhta hai: likhawat, hisaab, settings, kaanooni kaagaz, kitaab ke chapters.

Ismein bhi ek sachai chhupi hai. Zyadatar log apne kaam ki koi asli itihaas nahi rakhte. Unke paas `final.doc`, `final-2.doc`, `final-FINAL.doc` hote hain, jo wahi purana tareeka hai jo Kabir ne shuruaat mein bataya tha aur jo turant toot gaya tha.

Doosri galti: **git ko bas ek jagah samajhna jahan file rakhi jaati hain.**

File rakhna uska sabse chhota kaam hai. Uska asli kaam yeh yaad rakhna hai ki cheezein **kaise badli**, aur usse aap sawal poochh sakte ho: yeh kab toota? Kis badlav se toota? Us waqt kya soch thi?

Aur ek teesri, jo shuruaat mein sabko hoti hai: yeh sochna ki har badlav ek bada kaam hona chahiye. Chhote, baar baar kiye gaye records se itihaas kaam ka rehta hai. Ek bade record mein pachas cheezein ek saath hoti hain, aur uske baad aap yeh nahi dhoondh sakte ki kaunsi cheez se kya toota.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  VERSION CONTROL   itihaas, milaana,    │  ← naya
    │                    shakha               │
    │  kaam: himmat, purani copy nahi         │
    ├────────────────────────────────────────┤
    │  JAANCH, BUG, KHARCHA, API              │
    ├────────────────────────────────────────┤
    │  QUEUE, CACHE, DATABASE, INTERNET       │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek app do mahine se theek chal raha tha aur aaj achanak ek purana feature toot gaya. Aapke paas poora itihaas hai. Kaise dhoondhoge?

> **Jawab:** Beech se dhoondho.
>
> Do mahine ke beech ka koi ek din chuno aur dekho ki us din cheez chalti thi ya nahi. Agar chalti thi toh galti uske baad hui, warna pehle. Phir usi tarah aadha karte jao.
>
> Sau badlaon mein se galat wala saat kadam mein mil jaayega.
>
> Yeh Chapter 5.2 wali binary search hai, ab code ke itihaas pe lagi hui. **Ek hi soch, nayi jagah.** Git mein iske liye ek banaya banaya hukum bhi hai.

**2. (samajh check)** Do log ek hi line badalte hain aur machine tay nahi kar pati. Kya yeh ek problem hai jise theek karna chahiye?

> **Jawab:** Nahi. Yeh sahi vyavhaar hai.
>
> Machine ko pata nahi hai ki kaunsa badlav sahi hai. Sirf woh do log jaante hain ki woh kya kar rahe the.
>
> Agar machine apne aap koi ek chun leti, toh woh chup-chaap kisi ka kaam mita deti, aur kisi ko pata bhi na chalta.
>
> **Rukna aur poochna, chup-chaap galat kar dene se hamesha behtar hai.** Yeh soch poore software mein baar baar dikhti hai.

**3. (jodne wala)** Chapter 7.2 mein jaanch ka asli kaam "darr hataana" tha. Version control ka bhi wahi hai. Toh dono mein farak kya hai?

> **Jawab:** Dono jaal hain, lekin alag khatre ke liye.
>
> **Jaanch** batati hai ki abhi kuch toota hai ya nahi. Woh aage ki taraf dekhti hai.
>
> **Itihaas** batata hai ki kab toota aur kis wajah se, aur wapas jaane deta hai. Woh peeche ki taraf dekhta hai.
>
> Ek ke bina doosra aadha hai. Jaanch ke bina aapko pata hi nahi chalega ki kuch toota. Itihaas ke bina aap jaan toh loge ki toota hai, lekin na wajah milegi na wapas ja paoge.
>
> Isiliye har team mein dono hote hain, aur dono ek hi cheez ke liye hain: **badalne ki aazadi.**
