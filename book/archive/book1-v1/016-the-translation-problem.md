# Chapter 3.1  [SPINE]
## Translation problem

---

### Samvaad

**Madhav:** Machine sirf numbers samajhti hai. Aur nirdesh bhi numbers hain. Toh program likhne ka matlab kya hua?

**Kabir:** Sahi numbers sahi jagah likhna.

**Madhav:** Chalo likho. Do numbers jodne ka nirdesh likho.

**Kabir:** Mujhe kaise pata hoga ki kaunsa number "jodo" hai?

**Madhav:** Kisi kitaab mein likha hoga. Har chip ki apni list hoti hai. Maan lo "jodo" ka number 137 hai.

**Kabir:** Toh main 137 likh dunga.

**Madhav:** Aur kis cheez mein kya jodna hai?

**Kabir:** Woh bhi likhna padega. Kaunse khaane se, kaunse khaane mein.

**Madhav:** Toh ek chhote se kaam ke liye teen-chaar numbers. Ab ek poora app socho. Kitne nirdesh?

**Kabir:** Lakhon.

**Madhav:** Lakhon numbers, haath se, sahi order mein, aur ek bhi galat hua toh?

**Kabir:** Toh sab kuch galat.

**Madhav:** Aur agar tumhe beech mein ek nirdesh jodna ho?

**Kabir:** Uske aage ke saare... aage khisak jaayenge. Poora dobara likhna padega.

**Madhav:** Ab batao, tum kya chahoge?

**Kabir:** Main chahunga ki main aam bhasha mein likhun. "Ise usme jodo." Aur koi use numbers mein badal de.

**Madhav:** Kaun badlega?

**Kabir:** Koi aadmi.

**Madhav:** Aadmi thak jaayega aur galti karega.

**Kabir:** Toh koi machine.

**Madhav:** Machine ko kaise pata chalega ki kya karna hai?

**Kabir:** Uske andar bhi ek program hoga.

**Madhav:** Aur woh program kis shakal mein hoga?

**Kabir:** Numbers mein. Kyunki har program numbers mein hi hota hai.

**Madhav:** Toh tum ek aisa program chahte ho, jo numbers mein likha ho, aur jiska kaam ho doosre programs ko numbers mein badalna.

**Kabir:** Haan. Yeh ajeeb lag raha hai.

**Madhav:** Ajeeb hai, lekin ek baar bana lo toh phir kabhi nahi banana padta. Kisi ne ek baar woh takleef uthayi, aur uske baad kisi ko nahi uthani padi.

**Kabir:** Yeh toh Anil ki naali hai.

**Madhav:** Bilkul wahi hai. Do saal ki takleef, phir hamesha ke liye paani.

**Kabir:** Lekin sabse pehla wala? Jab koi translator tha hi nahi?

**Madhav:** Woh haath se likha gaya, numbers mein, ek-ek karke. Aur uske baad kisi ko dobara nahi likhna pada.

---

### Naam

Woh problem jo Kabir ne mehsoos ki, uska naam nahi hai, lekin uske hal ka hai.

Woh aam-bhasha jaisi shakal jismein insaan likhta hai, use **programming language** kehte hain.

Woh program jo use numbers mein badalta hai, use **compiler** ya **interpreter** kehte hain. Farak agle chapter mein.

Aur woh seedhe numbers wali shakal, jismein pehla aadmi likhta tha, use **machine code** kehte hain.

Beech mein ek aur shakal hoti hai, jahan har nirdesh ko ek chhota naam de diya jaata hai, jaise `ADD` ya `MOV`. Use **assembly** kehte hain. Woh insaan ke liye machine code se behtar hai, lekin sirf thoda.

```
insaan likhta hai        →   total = price + tax
                                    ↓  compiler
assembly                 →   MOV R1, price
                             ADD R1, tax
                             MOV total, R1
                                    ↓
machine code             →   10110001 00000101
                             00000001 00000110
                             10001001 00000111
                                    ↓
switch                   →   bijli aayi ya nahi
```

Chaar parat. Har parat neeche wali ko chhupa rahi hai. Yeh wahi cheez hai jo Chapter 0.4 mein Kabir ne khud nikaali thi, ab kaam karti hui dikh rahi hai.

Aur ek baat jo pehli baar ajeeb lagti hai: **compiler khud ek program hai, aur use bhi kisi ne likha tha.** Aaj ke compiler aksar usi language mein likhe hote hain jise woh translate karte hain. Yeh mumkin hai kyunki pehla wala haath se likha gaya tha, aur uske baad har naye compiler ko purane wale ne bana diya.

---

### Asli duniya se ek example

1950 ke dashak tak sab log seedhe machine ke numbers mein hi likhte the. Yeh maan liya gaya tha ki koi aur tareeka ho hi nahi sakta.

Grace Hopper naam ki ek naval officer aur mathematician ne kaha ki program aam angrezi jaise shabdon mein likha jaana chahiye, aur ek program use machine ke numbers mein badal dega.

Us waqt logon ne kaha ki yeh bewakoofi hai. Do wajahein deen: ki machine kabhi itni hoshiyaar nahi ho sakti, aur ki jo translator banayega woh insaan se ghatiya code banayega.

Doosri baat kai saal tak sach thi. Shuru ke compiler sach mein aise programs banate the jo haath se likhe programs se dheeme the.

Lekin pehli baat galat thi, aur woh zyada zaroori thi. Aaj lagbhag koi bhi machine code haath se nahi likhta. Aur compiler ab itne achhe ho chuke hain ki aksar woh insaan se behtar code banate hain, kyunki woh lakhon possibilities ek saath dekh sakte hain.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki programming language machine ki bhasha hai.**

Log kehte hain "computer Python samajhta hai." Computer Python nahi samajhta. Computer sirf apni chip ke numbers samajhta hai.

Python ek insaan ki suvidha hai. Machine ne usmein kabhi koi ruchi nahi li.

Iska seedha nateeja hai: yeh samajhna ki ek hi program alag machinon pe kyun nahi chalta, aur kyun use har jagah ke liye dobara translate karna padta hai. Aur yeh bhi ki "language" chunna asal mein machine ka nahi, insaan ka faisla hai.

Yeh galti templing isliye hai ki aap code likhte ho aur woh chal jaata hai. Beech ka translation dikhta hi nahi. Ek aur parat, pehle se chhupi hui.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  LANGUAGE     insaan ki shakal          │  ← naya
    │  TRANSLATOR   use numbers mein badalta  │  ← naya
    ├────────────────────────────────────────┤
    │  PROGRAM      nirdesh bhi numbers hain  │
    ├────────────────────────────────────────┤
    │  CPU, DOORI, RAM/DISK                   │
    ├────────────────────────────────────────┤
    │  BINARY, SHARTEIN, SWITCH               │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Compiler khud ek program hai. Toh sabse pehla compiler kisne banaya?

> **Jawab:** Kisi insaan ne, haath se, machine ke numbers mein. Ek baar.
>
> Uske baad us pehle compiler se ek behtar compiler banaya gaya. Aur us behtar wale se ek aur behtar.
>
> Aaj ke compiler lagbhag hamesha usi language mein likhe hote hain jise woh translate karte hain. Yeh ghoomta hua lagta hai lekin nahi hai, kyunki har naya wala kisi purane wale se bana tha, aur woh chain sabse pehle haath wale kaam pe jaakar rukti hai.
>
> Yeh technology ki ek aam shakal hai: **ek baar takleef uthao, phir us cheez se agli cheez banao.**

**2. (samajh check)** Ek aadmi kehta hai "main Python jaanta hoon, isliye main kisi bhi computer pe kaam kar sakta hoon." Kya yeh sahi hai?

> **Jawab:** Lagbhag sahi hai, aur wajah dilchasp hai.
>
> Woh isliye sahi nahi hai ki computer Python jaanta hai. Woh isliye sahi hai ki lagbhag har computer ke liye koi Python translator maujood hai.
>
> Yaani woh aadmi language pe nahi, un logon pe bharosa kar raha hai jinhone har machine ke liye translator likh diya.
>
> Yeh baat kaam ki hai: **jab kuch "har jagah chalta hai," toh iska matlab yeh nahi ki woh sarvavyapi hai. Iska matlab hai ki kisi ne har jagah ke liye alag se mehnat ki hai.**

**3. (jodne wala)** Chapter 0.2 ki teen dials yaad karo. Compiler banana kis dial ka udaharan hai?

> **Jawab:** Leverage ka, aur shayad kitaab ka sabse saaf udaharan hai.
>
> Ek baar likha gaya. Uske baad har programmer, har din, uska faayda uthata hai, bina us likhne wale ke kuch kiye.
>
> Scarcity bhi upar thi: bahut kam log compiler likh sakte hain.
>
> Aur size bhi bada tha: bina uske programming ek chhoti si duniya rehti.
>
> Teeno dials upar. Isiliye woh chand log jinhone yeh cheezein banayi, unka asar us paise se kahin zyada hai jo unhe mila.
