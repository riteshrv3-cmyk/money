# Chapter 4.5  [SPINE]
## Numbers ki jagah naam

---

### Samvaad

**Madhav:** Har machine ka ek pata hai, jaise `142.250.183.14`. Ab tumhe koi website kholni ho toh?

**Kabir:** Woh number yaad rakhna padega.

**Madhav:** Tumhe kitne numbers yaad hain?

**Kabir:** Do teen phone number. Bas.

**Madhav:** Aur tum roz kitni websites khologe?

**Kabir:** Bees, tees.

**Madhav:** Toh?

**Kabir:** Naam chahiye. Number ki jagah naam.

**Madhav:** Toh ek list bana lo. Naam ke saamne number.

**Kabir:** Theek hai.

**Madhav:** Woh list rakhoge kahan?

**Kabir:** Apne phone mein.

**Madhav:** Duniya mein lagbhag 35 crore naam hain. Aur roz naye jud rahe hain. Sabki list tumhare phone mein?

**Kabir:** Nahi. Bahut badi ho jaayegi. Aur purani bhi ho jaayegi.

**Madhav:** Toh?

**Kabir:** Ek jagah list rakh do. Sab wahan se poochein.

**Madhav:** Duniya ke saare sawal ek machine se? Ek second mein karodon sawal.

**Kabir:** Woh baith jaayegi.

**Madhav:** Aur agar woh ek machine band ho jaaye?

**Kabir:** Toh poora internet band. Naam kaam hi nahi karenge.

**Madhav:** Toh ek jagah bhi nahi chalega, har jagah bhi nahi chalega. Beech ka raasta socho.

**Kabir:** List ko baant do. Har machine ka apna hissa.

**Madhav:** Kaise baantoge? Naam toh koi bhi ho sakta hai.

**Kabir:** Naam mein hi kuch dhaancha daal do. Jaise pate mein hota hai: desh, sheher, gali, ghar.

**Madhav:** Peeche se aage, ya aage se peeche?

**Kabir:** Pehle bada, phir chhota. Jaise `.com` bada, uske andar `google`, uske andar `mail`.

**Madhav:** Bas. Ab har hisse ka apna rakhwala ho sakta hai. Jo `.com` sambhalta hai, use har `.com` ka pata nahi rakhna padta. Use sirf itna rakhna hai ki `google.com` kaun sambhalta hai.

**Kabir:** Aur woh phir aage bata dega.

**Madhav:** Toh ek sawal ke liye kitne kadam?

**Kabir:** Do teen. Har kadam pe list chhoti hoti jaayegi.

**Madhav:** Ab aakhri problem. Woh do-teen kadam har baar? Har website ke liye, har baar?

**Kabir:** Nahi. Jawab yaad rakh lo kuch der ke liye.

**Madhav:** Kitni der?

**Kabir:** Kuch ghante? Kyunki pate kabhi kabhi badalte hain.

**Madhav:** Aur agar tumne bees ghante rakh liya aur pata beech mein badal gaya?

**Kabir:** Toh main galat jagah jaunga jab tak purani jaankari na hate.

**Madhav:** Isiliye jab koi website apna server badalti hai, toh kuch logon ke liye woh turant chalti hai aur kuch ke liye kuch ghante purani jagah pe hi jaati rehti hai.

---

### Naam

Us naam wali system ka naam hai **DNS**, yaani naam ko pate mein badalne wala jaal.

Naam ka dhaancha, peeche se aage:

```
mail  .  google  .  com  .
 │         │        │     │
 │         │        │     └── sabse upar wali jad
 │         │        └── kaun `.com` sambhalta hai
 │         └── kaun `google.com` sambhalta hai
 └── uske andar ka ek hissa
```

Ek sawal ka safar:

```
1. tumhara phone poochta hai: mail.google.com kahan hai?
2. koi nahi jaanta toh jad se poocha jaata hai:
   "`.com` kaun sambhalta hai?"
3. `.com` wale se: "google.com kaun sambhalta hai?"
4. google wale se: "mail.google.com ka pata kya hai?"
5. pata mil gaya. Ab yaad rakh liya jaata hai, kuch ghante ke liye.
```

Us yaad rakhne ko **cache** kehte hain, aur us waqt ki seema ko **TTL**.

Ab woh baat jo iss chapter ko bahut aage tak le jaati hai:

**Naam ka maalik alag hota hai, machine ka maalik alag.**

Aap ek naam kirye pe lete ho, saal ke hisaab se. Machine kahin aur hai. Agar aap machine badal do toh naam wahi rehta hai, bas uska ishara nayi jagah kar dete ho.

Aur iska ulta bhi sach hai, aur woh khatarnak hai: **jo naam ka rakhwala hai, woh use kisi aur jagah bhi bhej sakta hai.** Naam ki poori taakat ek list mein likhi ek line pe tiki hai, aur woh line kisi aur ke paas hai.

---

### Asli duniya se ek example

2021 mein Facebook, Instagram aur WhatsApp lagbhag chhe ghante ke liye poori duniya se gayab ho gaye.

Server chal rahe the. Data theek tha. Lekin ek galat badlav ki wajah se unke pate baantne wali jaankari internet se hat gayi. Naam ka jawab dene ka koi raasta hi nahi bacha.

Aur uska ek nateeja aur nikla jo dilchasp hai: unke apne office ke darwaze bhi unhi systems se chalte the, jo unhi naamon pe khade the. Log andar nahi ja paaye us jagah ko theek karne, jisne unhe bahar kar diya tha.

Yeh Chapter 0.4 ki baat hai, ek dum saaf: **jo cheez achhi tarah chalti hai woh dikhti nahi. Woh sirf toot ne pe dikhti hai.** Aur us din duniya ne dekha ki naam poore internet ki neev mein baitha hai.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki website ka naam khareedne se aap uske maalik ban jaate ho.**

Aap naam khareedte nahi. Aap use kirye pe lete ho, aksar saal ke hisaab se. Kiraya rukta hai toh naam kisi aur ko mil sakta hai.

Aur iska ek gehra nateeja hai. Poori company ka naam, uske saare link, uska email, uske customer ka bharosa, sab ek entry pe tike hote hain jiske aap maalik nahi hain.

Isliye purani companies apna naam bees-tees saal ke liye ek saath le leti hain. Woh kanjoosi ka ulta hai, aur woh isliye hai ki unhe pata hai ki neeche kya hai.

Yeh galti tempting isliye hai ki naam permanent lagta hai. Woh aapke card pe likha hai, aapke sign board pe hai. Lekin woh sirf ek list mein ek line hai, aur list kisi aur ki hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  NAAM         insaan naam yaad rakhta,  │  ← naya
    │               machine pata istemaal     │
    │  CACHE        jawab kuch der yaad rakho │  ← naya
    ├────────────────────────────────────────┤
    │  PROTOCOL, PACKET, PATA, NETWORK        │
    ├────────────────────────────────────────┤
    │  OS, PROCESS, CPU, RAM/DISK, SWITCH     │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek company apna server badalti hai. Kuch logon ke liye website turant nayi jagah khulti hai, kuch ke liye do ghante tak purani. Kyun?

> **Jawab:** Cache ki wajah se.
>
> Jinhone haal hi mein woh naam poocha tha, unke paas purana jawab abhi bhi pada hai, aur woh tab tak rahega jab tak uska waqt khatam na ho.
>
> Isiliye jab koi company jagah badalne wali hoti hai, toh woh pehle us waqt ko chhota kar deti hai, kuch din pehle. Phir badlav karti hai. Phir waqt wapas bada kar deti hai.
>
> Yeh cache ka aam sauda hai, jo aage Part 6 mein poora khulega: **cache tez banata hai aur purana bhi rakhta hai. Dono ek hi cheez ke do hisse hain.**

**2. (samajh check)** DNS ko ek hi jagah kyun nahi rakha gaya, jab woh zyada simple hota?

> **Jawab:** Do wajahein, aur dono Chapter 4.1 se aati hain.
>
> Ek: karodon sawal ek second mein. Koi ek machine woh nahi utha sakti.
>
> Do: agar woh ek machine gir jaaye toh poora internet naam ke bina reh jaayega. Ek jagah rakhne ka matlab hai ek jagah todne se sab tootega.
>
> Isiliye use pedh ki tarah baanta gaya, jahan har shakha apna hissa sambhalti hai.
>
> Yeh dhaancha aage phir milega. **Jab kuch bahut bada ho jaaye, toh use baanto, aur baantne ka tareeka naam mein hi daal do.**

**3. (jodne wala)** Chapter 4.4 kehta tha ki jo protocol tay karta hai woh us ilaake ki shakal tay kar deta hai. DNS mein woh taakat kiske paas hai?

> **Jawab:** Un logon ke paas jo sabse upar wali jad aur bade hisse sambhalte hain.
>
> Woh yeh tay kar sakte hain ki naye tarah ke naam bane ya nahi, aur unke niyam kya honge.
>
> Aur theory mein, woh kisi naam ko hata bhi sakte hain. Aisa hua bhi hai.
>
> Yeh Chapter 4.8 ka rasta hai. Internet ka "koi maalik nahi hai" bilkul sach hai, aur phir bhi kuch jagahein aisi hain jahan taakat sach mein baithi hai. Naam un mein se sabse badi jagah hai.
