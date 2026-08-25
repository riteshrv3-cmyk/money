# Chapter 3.2  [SPINE]
## Translator ke do tareeke

---

### Samvaad

**Madhav:** Tumhe ek angrezi kitaab hindi mein chahiye. Do tareeke hain. Batao.

**Kabir:** Ek toh poori kitaab pehle translate karwa lo. Phir padho.

**Madhav:** Doosra?

**Kabir:** Ek aadmi paas baith jaaye aur padhte padhte bolta jaaye.

**Madhav:** Ab dono ke faayde nuksaan batao. Pehla tareeka.

**Kabir:** Shuru mein waqt lagega, poori kitaab karni padegi. Lekin uske baad padhna tez hoga. Aur baar baar padho toh har baar tez.

**Madhav:** Aur agar kitaab mein ek galti hai, page 300 pe?

**Kabir:** Woh translate karte waqt hi pakdi jaayegi. Padhna shuru karne se pehle.

**Madhav:** Achha. Ab doosra tareeka.

**Kabir:** Turant shuru ho jaata hai. Lekin padhna dheema hoga, kyunki har line par tarjuma ho raha hai.

**Madhav:** Aur page 300 wali galti?

**Kabir:** Woh tab pata chalegi jab hum page 300 pe pahunchenge.

**Madhav:** Aur agar hum kabhi page 300 tak pahunche hi nahi?

**Kabir:** Toh kabhi pata nahi chalegi.

**Madhav:** Ab ek aur baat. Doosre tareeke mein, agar main beech mein kahun "yeh line badal do, dobara padho"?

**Kabir:** Woh ho sakta hai. Aadmi wahin baitha hai.

**Madhav:** Aur pehle tareeke mein?

**Kabir:** Poori kitaab dobara translate karwani padegi.

**Madhav:** Toh ab batao, kaunsa tareeka behtar hai?

**Kabir:** Depends. Agar kitaab baar baar padhni hai toh pehla. Agar experiment karna hai toh doosra.

**Madhav:** Bas. Aur programming mein bilkul yahi do tareeke hain, unhi faaydon aur nuksaan ke saath.

---

### Naam

```
COMPILER    poora program pehle numbers mein badal do,
            phir chalao

INTERPRETER chalate chalate translate karo, line by line
```

Aur seedha nateeja:

```
                     COMPILER              INTERPRETER
shuru hone mein      der lagti hai         turant
chalne mein          tez                   dheema
galti kab pakdi      chalane se pehle      wahan pahunchne pe
badalna              dobara compile        turant
dena kis shakal mein numbers               asli code + translator
```

Aur isse ek baat nikalti hai jo log aksar nahi jodte:

**Compiled program dene ke liye aapko apna code nahi dena padta.** Aap numbers de dete ho. Interpreted program dene ke liye aapko asli code dena padta hai, ya kam se kam kuch aisa jo uske bahut kareeb hai.

Isiliye bikne wale software aksar compiled hote hain, aur khule software aksar interpreted.

Aaj ki asli duniya beech mein hai. Java aur C# pehle ek beech ki shakal mein compile hote hain, aur woh shakal chalte waqt translate hoti hai. JavaScript aur Python interpreted hain, lekin unke andar ek hissa chalte-chalte compile bhi karta hai, un jagahon ke liye jo baar baar chalti hain.

Yeh khud ek kaam ka soch hai: **jo cheez baar baar chalti hai use pehle se taiyaar kar lo, jo ek baar chalti hai use waqt pe hi kar lo.** Yeh soch aage cache mein, database mein, aur AI mein phir milegi.

---

### Asli duniya se ek example

C, jo 1972 mein bani, compiled hai. Operating system, database aur game engine aaj bhi usmein ya usi jaisi languages mein likhe jaate hain, kyunki wahan har kadam ki speed mayne rakhti hai.

Python, jo 1991 mein aayi, interpreted hai. Woh C se lagbhag 10 se 100 guna dheemi hai.

Ab dhyaan dene wali baat: **aaj lagbhag saara AI ka kaam Python mein likha jaata hai**, jo dheemi language hai.

Yeh ulta lagta hai. Lekin wajah saaf hai: Python khud kaam nahi karti. Woh sirf order deti hai. Asli hisaab C ya usse bhi neeche likhe hisson mein hota hai. Python bas yeh tay karti hai ki kaunsa bada kaam kab shuru ho.

Yaani insaan wahan baitha hai jahan sochna hai, aur tez cheez wahan hai jahan mehnat hai.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki dheemi language matlab dheema program.**

Log yeh sun kar ghabra jaate hain ki Python C se sau guna dheemi hai, aur maan lete hain ki unka program bhi sau guna dheema hoga.

Lekin agar program ka 99 pratishat waqt kisi tez hisse mein ja raha hai, aur Python sirf order de rahi hai, toh farak lagbhag nahi padta.

Yeh Chapter 2.3 wali baat hai, doosri shakal mein: **speed wahan mayne rakhti hai jahan waqt lagta hai, har jagah nahi.**

Yeh galti tempting isliye hai ki speed ka ek hi number bata diya jaata hai, aur woh number kabhi nahi batata ki program apna waqt kahan bitata hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  DO TAREEKE   pehle poora, ya chalte    │  ← naya
    │               chalte                    │
    ├────────────────────────────────────────┤
    │  LANGUAGE, TRANSLATOR                   │
    ├────────────────────────────────────────┤
    │  CPU, DOORI, RAM/DISK                   │
    ├────────────────────────────────────────┤
    │  PROGRAM, BINARY, SWITCH                │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek game bana rahe ho jo har second saath baar screen banata hai. Compiler ya interpreter?

> **Jawab:** Compiler, aur bina soche.
>
> Kyunki wahan har kadam ki speed sach mein mayne rakhti hai. Har frame ke liye lakhon hisaab hain, aur woh hisaab aapka apna code kar raha hai, kisi aur ka nahi.
>
> Yeh tab badalta hai jab aapka code sirf order de raha ho. Tab language ki speed lagbhag bemaani ho jaati hai.

**2. (samajh check)** Ek program compile hone ke baad chalta hai lekin ek khaas haalat mein crash ho jaata hai. Compiler ne use kyun nahi pakda?

> **Jawab:** Kyunki compiler sirf **shakal** dekh sakta hai, **nateeja** nahi.
>
> Woh pakad sakta hai ki aapne galat likha, ya do cheezein jodne ki koshish ki jo jud hi nahi sakti.
>
> Woh yeh nahi pakad sakta ki chalte waqt koi number zero ho jaayega, ya user kuch aisa likhega jiska aapne socha hi nahi tha.
>
> Yeh ek gehri seema hai: **kuch galtiyan sirf chalne pe hi dikhti hain, kyunki woh code mein nahi, data mein hoti hain.** Isiliye testing ek alag cheez hai, aur woh Part 4 hai.

**3. (jodne wala)** Chapter 1.6 kehta tha ki program aur data dono numbers hain. Interpreter uss baat ka kaunsa udaharan hai?

> **Jawab:** Ek saaf udaharan.
>
> Interpreter ke liye, aapka program **data** hai. Woh use padhta hai, jaise koi program kisi photo ko padhta hai.
>
> Aur us data ko padhkar woh tay karta hai ki kya karna hai.
>
> Toh ek hi cheez, aapka code, do nazariyon se do alag cheezein hai: aapke liye woh nirdesh hai, interpreter ke liye woh data hai.
>
> Yeh baat Book 2 mein bahut kaam aayegi. Wahan aap dekhoge ki AI ke liye bhi aapke shabd data hain, nirdesh nahi, aur usse bahut kuch samajh mein aata hai.
