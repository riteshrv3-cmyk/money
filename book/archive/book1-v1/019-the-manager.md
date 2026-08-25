# Chapter 3.4  [SPINE]
## Woh manager jo machine baantta hai

---

### Samvaad

**Madhav:** Tumhare phone mein abhi kitne app khule hain?

**Kabir:** Chaar paanch. Aur peeche kuch aur bhi chal rahe honge.

**Madhav:** Aur CPU kitni hai?

**Kabir:** Ek chip.

**Madhav:** Chapter 2.3 mein humne dekha ki CPU ek waqt mein ek nirdesh chalati hai. Toh paanch app ek saath kaise chal rahe hain?

**Kabir:** Ho sakta hai chip mein kai hisse hon.

**Madhav:** Aath hisse hote hain aam taur pe. Aur app peeche milakar tees-chalees. Ab?

**Kabir:** Toh sach mein saath nahi chal rahe honge.

**Madhav:** Toh kya ho raha hai?

**Kabir:** Baari baari?

**Madhav:** Kitni jaldi baari badalti hogi ki tumhe pata hi na chale?

**Kabir:** Bahut jaldi. Second ke kuch hisson mein.

**Madhav:** Har app ko lagbhag das millisecond milte hain, phir agla. Tumhari aankh us farak ko pakad hi nahi sakti, isliye sab ek saath lagta hai.

**Kabir:** Toh baari kaun tay karta hai?

**Madhav:** Yehi sawal hai. Socho, kya app khud tay kar sakte hain?

**Kabir:** Nahi. Har app apni hi baari lena chahega.

**Madhav:** Aur agar ek app kabhi na chhode?

**Kabir:** Toh baaki sab ruk jaayenge. Phone hang ho jaayega.

**Madhav:** Toh?

**Kabir:** Koi upar wala hona chahiye. Koi jo sabse zyada taakat rakhta ho aur baari tay kare.

**Madhav:** Aur woh khud kya hai?

**Kabir:** Woh bhi ek program hi hoga.

**Madhav:** Aur agar woh bhi ek program hai, toh use apni taakat kahan se milti hai? App use hata kyun nahi sakte?

**Kabir:** Kyunki... woh pehle chalu hota hai?

**Madhav:** Ek wajah yeh hai. Doosri wajah chip ke andar hai. Chip ke do modes hote hain. Ek mein program sab kuch kar sakta hai. Doosre mein kuch cheezein rok di jaati hain. App doosre mode mein chalte hain.

**Kabir:** Toh app chahkar bhi kuch nahi kar sakta?

**Madhav:** Nahi. Agar woh koshish kare toh chip use rok deti hai aur manager ko bula leti hai.

**Kabir:** Achha. Toh manager sirf baari nahi baantta.

**Madhav:** Aur kya baantega, socho. Do app ek saath RAM maangte hain.

**Kabir:** Toh koi tay kare ki kisko kaunsa hissa mile. Aur ek app doosre ka hissa na padh paaye.

**Madhav:** Aur agar padh le?

**Kabir:** Toh mera bank app mere doosre app ka data padh lega.

**Madhav:** Ab tum samajh gaye ki manager kyun hai. Aur bhi? Do app ek saath file kholna chahein?

**Kabir:** Wahi baat. Koi tay kare kaun kholega, aur kis order mein.

**Madhav:** Camera? Ek waqt mein kaun istemaal karega?

**Kabir:** Wahi.

**Madhav:** Ab ek line mein bolo ki manager karta kya hai.

**Kabir:** Jo cheezein ek hain aur maangne wale kai, unhe baantta hai. Aur sabko ek doosre se alag rakhta hai.

---

### Naam

Us manager ka naam hai **operating system**. Windows, Android, iOS, Linux, macOS.

Uske chaar bade kaam:

```
BAARI BAANTNA     kaunsa program ab chalega, aur kitni der
                  (har program ko lagta hai woh akela chal raha hai)

JAGAH BAANTNA     RAM ka kaunsa hissa kise mile
                  (aur koi doosre ka hissa na dekh sake)

SAAMAN BAANTNA    screen, camera, speaker, network, ek hain aur
                  maangne wale kai

ALAG RAKHNA       ek program doosre ko na chhoo sake
                  (yeh sabse zaroori hai, aur kam dikhta hai)
```

Aur woh sabse andar wala hissa jiske paas poori taakat hoti hai, use **kernel** kehte hain.

Ab woh cheez jo Kabir ne nikaali, use naam dena zaroori hai. Har program ko lagta hai ki poori machine sirf uski hai. Use nahi pata ki koi aur bhi chal raha hai. Use nahi pata ki uski baari beech mein rok kar kisi aur ko de di jaati hai.

Yeh jhooth jaan-boojh ke bola jaata hai, aur woh hi poore operating system ka asli product hai.

Aur ab Chapter 0.4 ki baat wapas dekho. Yeh abstraction ka sabse saaf udaharan hai. OS neeche wali sachai, ki ek chip hai aur woh baari baari chal rahi hai, poori tarah chhupa deta hai.

---

### Asli duniya se ek example

Purane phone aur computer mein yeh alag rakhna itna sakht nahi tha. Ek app doosre ka data padh sakta tha. Ek app crash hota tha toh poori machine baith jaati thi.

Aaj ke phone mein har app apne dabbe mein band hota hai. Woh doosre app ki files nahi dekh sakta. Woh camera ya location tab tak nahi le sakta jab tak aap ijaazat na do.

Isiliye jab aap koi app install karte ho toh woh poochta hai. Woh shishtachar nahi hai. Woh iss baat ka nateeja hai ki OS ne use koi taakat di hi nahi, aur woh sirf manager se maang sakta hai.

Aur isiliye ek kharaab app aapka phone ab utni aasani se barbaad nahi kar pata jitna pehle karta tha. Woh apne dabbe se bahar nahi ja sakta.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki operating system woh cheez hai jo screen pe dikhti hai.**

Log Windows ka matlab samajhte hain woh neela background, woh menu, woh icons. Woh saara hissa upar ki ek parat hai. Use hataya ja sakta hai aur OS phir bhi chalega.

Asli OS woh hissa hai jo dikhta hi nahi: kaun kab chalega, kiski jagah kahan hai, kaun kya chhoo sakta hai.

Iska seedha nateeja: log samajh nahi paate ki server pe OS bina kisi screen ke kaise chalta hai. Aur woh yeh bhi nahi samajh paate ki phone dheema kyun hai, kyunki woh sirf woh dekh rahe hain jo dikh raha hai.

Yeh galti tempting isliye hai ki OS ka jo hissa aapse milta hai, wahi ek hissa hai jo dikhne ke liye banaya gaya hai. Baaki sab apne aap ko chhupane ki koshish kar raha hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  OS           baari, jagah, saaman      │  ← naya
    │               aur sabko alag rakhna     │
    ├────────────────────────────────────────┤
    │  LANGUAGE, TRANSLATOR, CHUNAV           │
    ├────────────────────────────────────────┤
    │  CPU, RAM/DISK, DOORI                   │
    ├────────────────────────────────────────┤
    │  PROGRAM, BINARY, SWITCH                │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek app hang ho jaata hai lekin aap use band kar sakte ho aur baaki phone chalta rehta hai. Kaun band kar raha hai use, aur woh kaise kar pa raha hai?

> **Jawab:** OS kar raha hai, aur woh isliye kar pa raha hai kyunki app ke paas kabhi asli taakat thi hi nahi.
>
> App ki baari OS deta hai. Toh OS bas uski baari dena band kar deta hai aur uski jagah wapas le leta hai.
>
> App yeh rok nahi sakta. Woh chip ke us mode mein chal raha hai jahan usse yeh kar hi nahi sakta.
>
> Isiliye purane systems mein ek app poori machine baitha deta tha, aur ab nahi. Farak taakat ka hai, speed ka nahi.

**2. (samajh check)** Aapka phone kehta hai "yeh app aapka location dekhna chahta hai." Kaun pooch raha hai, aur agar aap na kaho toh kya hota hai?

> **Jawab:** OS pooch raha hai, app nahi.
>
> App ne OS se location maanga. OS ne aapse poocha. Aap mana karo toh OS app ko keh deta hai ki nahi mila.
>
> App iske aas-paas se nikal nahi sakta, kyunki uske paas location tak jaane ka koi seedha raasta hai hi nahi. Har raasta OS se hokar jaata hai.
>
> Yeh soch aage phir milegi. Book 2 mein aap dekhoge ki AI agent ke paas bhi apna koi haath nahi hota. Har cheez kisi ke through jaati hai, aur wahi jagah hai jahan rok lagti hai.

**3. (jodne wala)** Chapter 0.3 mein Kabir ne kaha tha ki ek group ajnabiyon ko scale pe serve karta hai. OS us baat ka kaunsa roop hai?

> **Jawab:** OS ek manager hai jo un programs ke beech baantta hai jo ek doosre ko jaante hi nahi.
>
> Jaise sheher mein log ek doosre ko jaane bina ek hi sadak istemaal karte hain, aur koi niyam tay karta hai ki kaun kab chalega.
>
> Aur wahi wajah bhi ek hai: gaon mein sau log the toh aapas mein tay ho jaata tha. Programs bhi jab do teen the tab tay ho jaata tha. Jab tees-chalees ho gaye, tab manager zaroori ho gaya.
>
> **Scale hi manager ko paida karta hai.** Yeh baat Part 7 mein poore zor se wapas aayegi.
