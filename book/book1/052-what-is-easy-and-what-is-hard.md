# Chapter 8.2  [SPINE]
## Kya banana aasan hai, kya mushkil

---

### Samvaad

**Madhav:** Ab aap naksha samajh gaye. Lekin design karne ke liye ek aur cheez chahiye. Do kaam batata hoon, aap batao kaunsa bada hai. Ek: login banana. Do: search banana.

**Kabir:** Dono ek jaise lagte hain.

**Madhav:** Login lagbhag ek hafte ka kaam hai. Achha search kai mahine ka.

**Kabir:** Kyun?

**Madhav:** Login mein kya karna hai?

**Kabir:** Naam aur password lo, milao, andar aane do.

**Madhav:** Aur search mein?

**Kabir:** Shabd lo, aur... jo cheezein us se milti hain woh do.

**Madhav:** "Milti hain" ka matlab kya hai? Agar main "kitab" likhun aur cheez mein "kitaab" likha ho?

**Kabir:** Woh bhi milna chahiye.

**Madhav:** Aur "book" likha ho?

**Kabir:** Shayad woh bhi.

**Madhav:** Aur agar sau cheezein milein, toh pehle kaunsi dikhegi?

**Kabir:** Jo sabse zyada milti hai.

**Madhav:** "Sabse zyada" kaise naapoge?

**Kabir:** Hmm. Pata nahi.

**Madhav:** Bas. Yahi farak hai. Login mein sahi jawab ek hai aur woh saaf hai. Search mein "sahi jawab" ki koi paribhasha hi nahi hai.

**Kabir:** Toh mushkil kaam woh hai jismein sahi jawab tay nahi hota.

**Madhav:** Yeh ek pehchaan hai. Aur bhi hain. Ek aur jodi. Ek: photo upload karna. Do: video call banana.

**Kabir:** Video call mushkil hoga. Live hai.

**Madhav:** Kyun mushkil hai?

**Kabir:** Kyunki der nahi ho sakti. Chapter 4.3, purani awaaz kisi kaam ki nahi.

**Madhav:** Toh doosri pehchaan kya hui?

**Kabir:** Jo cheez asli waqt mein honi chahiye woh mushkil hai.

**Madhav:** Ek aur. Ek: apni site pe payment lena. Do: apna khud ka payment system banana.

**Kabir:** Doosra bahut mushkil. Usmein bank, kanoon, suraksha sab hai.

**Madhav:** Toh teesri pehchaan?

**Kabir:** Jismein paisa ya kanoon jud jaaye woh bahut mushkil ho jaata hai.

**Madhav:** Aur aakhri. Ek: naya app banana. Do: ek purane app mein ek chhota feature jodna, jo dus saal purana hai aur jise bees log likh chuke hain.

**Kabir:** Naya banana aasan hoga.

**Madhav:** Kyun? Naye mein toh sab kuch shuru se banana hai.

**Kabir:** Lekin purane mein mujhe pata hi nahi ki kya kahan hai, aur kya toot jaayega.

**Madhav:** Bas. Chauthi pehchaan, aur woh sabse zyada nazarandaaz hoti hai: **purani cheez ko chhoona nayi banane se mehnga hota hai.**

---

### Char pehchaanein

```
1. SAHI JAWAB SAAF HAI YA NAHI
   saaf   →  aasan   (login, hisaab, form, list)
   dhundhla → mushkil (search, sujhav, "achha" kya hai)

2. WAQT KI SAKHTI
   baad mein chalega → aasan
   turant chahiye    → mushkil (call, game, live)

3. PAISA YA KANOON
   nahi juda  →  aasan
   juda hua   →  bahut mushkil (payment, sehat, bachche ka data)

4. NAYA YA PURANA
   khaali kaagaz  →  aasan
   purani cheez   →  mushkil, aur anumaan hamesha galat (Ch 7.5)
```

---

### Mota andaza, ek aadmi ke liye

Yeh sirf paimana dene ke liye hai. Har aankda haalat pe badalta hai, lekin **aapas ka anupaat** aksar sach rehta hai.

```
KUCH DIN
├── ek form, jo data leta hai aur database mein rakhta hai
├── ek list dikhana
├── login, agar kisi bane banaye ka istemaal karo
├── ek chhoti website
└── email bhejna, kisi bani banayi service se

KUCH HAFTE
├── login khud banana (theek se, suraksha ke saath)
├── payment lena, kisi bani banayi service se
├── file aur photo upload
├── notification bhejna
├── ek chhota mobile app
└── ek admin panel

KUCH MAHINE
├── achha search
├── kisi purane bade system mein ek nayi cheez jodna
├── ek app jo offline bhi chale aur baad mein mila le
├── theek se scale karna (Part 6 ki cheezein)
└── ek aisa system jo kai company istemaal karein

EK SAAL YA ZYADA
├── apna payment system
├── video call ya live stream, apna
├── apna database ya search engine
├── kuch aisa jismein kanoon ki sakhti ho
└── kuch aisa jo hazaaron logon ke saath ek saath badle
```

Aur ek cheez jo iss poori list se zyada zaroori hai:

**Har list mein neeche wali cheezein aksar isliye mushkil nahi hain ki unka hisaab mushkil hai. Woh isliye mushkil hain ki unke andar anginat haalatein hain, ya unka "sahi" tay nahi hai.**

Chapter 7.1 wali baat, ab design ke kaam mein lagi hui.

---

### Ek aur cheez: khareedo ya banao

Har cheez ke liye ek aur sawal hai:

```
KHAREEDO / ISTEMAAL KARO jab
├── woh cheez aapka product nahi hai
├── woh cheez sab ke liye ek jaisi hai (login, payment, email)
└── uski galtiyan mehngi hain aur doosron ne unhe already jhel liya hai

KHUD BANAO jab
├── wahi cheez aapka product hai
├── ya woh cheez aapke liye khaas tarah se alag hai
└── ya uspe nirbhar hona bahut khatarnak hai (Ch 6.4)
```

Zyadatar log ulta karte hain. Woh login khud banate hain, jo unka product nahi hai, aur woh khaas cheez khareed lete hain jo unka product hai.

---

### Asli duniya se ek example

Instagram 2012 mein ek arab dollar mein bika. Us waqt uske paas 13 log the.

Unhone bahut kuch khud nahi banaya. Server kirye pe the, bahut si cheezein bane banaye tukdon se thin, aur unka apna kaam kaafi chhota tha.

Unka asli kaam do cheezon mein tha: photo pe filter, aur ek aisa feed jo tez khule.

Baaki sab kuch woh tha jo kisi aur ne bana rakha tha.

Yeh design ki taakat hai. **Woh yeh nahi tha ki unhone bahut kuch banaya. Woh yeh tha ki unhone bahut kam banaya, aur sahi cheez banayi.**

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **cheez ke dikhne se uski mushkil ka andaza lagana.**

Ek button jo kehta hai "sab dost bulao" bahut chhota dikhta hai. Uske peeche contact ki ijaazat, alag alag phone ke alag niyam, email bhejna, spam se bachna, aur duplicate sambhalna hota hai.

Aur ek page jo bahut bhara hua dikhta hai, woh aksar ek list hoti hai jo do din mein ban jaati hai.

**Jo dikhta hai woh kaam ka naap nahi hai.** Kaam un haalaton mein hai jo dikhti nahi.

Doosri galti: **"AI se ab yeh sab aasan ho gaya."**

AI ne kuch cheezein sach mein bahut sasti kar di hain, khaaskar woh jo pehle likhi ja chuki hain aur jinka sahi jawab saaf hai.

Woh chaar pehchaanein nahi badli hain. Jo cheez isliye mushkil thi ki uska "sahi" tay nahi tha, woh aaj bhi mushkil hai. Jo cheez isliye mushkil thi ki uske andar paisa aur kanoon hai, woh aaj bhi mushkil hai. Aur purani cheez ko chhoona aaj bhi mehnga hai.

**AI ne likhne ki keemat giraayi hai. Usne samajhne ki keemat nahi giraayi.** Aur design samajhne ka kaam hai.

---

### Sochne ke liye

**1. (samajh check)** Ek aadmi kehta hai "main WhatsApp jaisa app banaunga, do mahine mein." Chaar pehchaanon pe chalao.

> **Jawab:** Messages bhejna aur dikhana: sahi jawab saaf hai, waqt ki sakhti kam hai. Woh hissa sach mein kuch hafton mein ban sakta hai.
>
> Lekin: end to end taala (suraksha, jahan galti bahut mehngi hai), video call (asli waqt), lakhon logon pe chalna (Part 6), aur har phone pe kaam karna.
>
> Toh "WhatsApp jaisa" ek chhota kaam hai aur "WhatsApp" ek bahut bada kaam hai. Farak sirf paimane ka nahi hai, woh chaaron pehchaanon ka hai.
>
> Aur yahi sawal sahi tareeka hai kisi bhi bade idea ko naapne ka: **usmein se woh chhota hissa nikaalo jo pehli teen pehchaanon mein aasan hai.**

**2. (samajh check)** Ek team ne apna khud ka login system banaya. Woh chal raha hai. Kya yeh sahi faisla tha?

> **Jawab:** Aksar nahi.
>
> Login sabke liye ek jaisa hai, kisi ka product nahi hai, aur usmein galti ki keemat bahut zyada hai. Yeh teeno "khareedo" wale niyam hain.
>
> "Chal raha hai" kaafi nahi hai. Login ki galtiyan chalne mein nahi dikhti. Woh us din dikhti hain jab koi dhoondh leta hai.
>
> Ek apwaad hai: agar aapka product hi login ya pehchaan hai, toh khud banana hi sahi hai.

**3. (jodne wala)** Chapter 7.5 kehta tha ki anumaan gyaan ka naap hai. Yeh chapter chaar pehchaanein deta hai. Dono ko jodo.

> **Jawab:** Chaar pehchaanein aapko batati hain ki aapka gyaan kitna kam hai.
>
> Jaha sahi jawab saaf hai, wahan aap jaante ho ki kya banana hai, toh anumaan theek hoga.
>
> Jaha sahi jawab dhundhla hai, wahan aapko yeh bhi nahi pata ki aap kya bana rahe ho, isliye anumaan lagbhag bekaar hai.
>
> Toh yeh chaar pehchaanein ek aur kaam bhi karti hain: **woh batati hain ki aapke anumaan par kitna bharosa kiya jaa sakta hai.**
>
> Ek "kuch din" wala kaam aksar sach mein kuch din ka hota hai. Ek "kuch mahine" wala kaam kuch bhi ho sakta hai.
