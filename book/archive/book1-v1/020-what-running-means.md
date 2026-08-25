# Chapter 3.5  [DEPTH]
## "Running" ka matlab kya hai

---

*DEPTH chapter. Iske baad "app khula hai," "app band hai," aur "app crash ho gaya" ka asli matlab pata chalega.*

---

### Samvaad

**Madhav:** Ek app tumhare phone mein hai lekin khula nahi hai. Woh kahan hai?

**Kabir:** Storage mein. Disk pe.

**Madhav:** Aur kis shakal mein?

**Kabir:** Numbers ki ek file.

**Madhav:** Woh file kuch kar rahi hai?

**Kabir:** Nahi. Bas padi hai.

**Madhav:** Ab tum icon dabate ho. Kya hota hai?

**Kabir:** App khul jaata hai.

**Madhav:** Kadam ke hisaab se batao. Pehla kadam kya?

**Kabir:** Woh file... RAM mein aani padegi. Kyunki CPU disk se seedha nahi chala sakti.

**Madhav:** Achha. Ab woh RAM mein hai. Aur?

**Kabir:** CPU ko batana padega ki shuru kahan se karna hai.

**Madhav:** Woh program counter, Chapter 2.3 wala. Usmein pehla pata daal do. Aur?

**Kabir:** Bas, chalna shuru?

**Madhav:** Ek cheez aur chahiye. App ko apne kaam ke numbers rakhne ke liye jagah chahiye. Woh jagah kaun degi?

**Kabir:** OS.

**Madhav:** Toh ab ginti karo. App chalne ke liye kya kya chahiye?

**Kabir:** RAM mein nirdesh. Ek jagah apne data ke liye. Aur ek nishaan ki abhi kahan hoon.

**Madhav:** Aur ek cheez aur, jo tum bhool rahe ho. Agar OS beech mein iski baari le le, aur baad mein wapas de, toh use kaise pata chalega ki yeh kahan tha?

**Kabir:** Uske sab khaane sambhal kar rakhne padenge. Registers.

**Madhav:** Bas. Ab in sab ka ek dher bana lo. Yeh dher hi "chal raha app" hai.

**Kabir:** Toh file aur chalta hua app do alag cheezein hain.

**Madhav:** Bilkul alag. File ek hai. Ab batao, kya ek hi file se do app ek saath chal sakte hain?

**Kabir:** Do browser window? Haan, chal sakte hain.

**Madhav:** Toh file ek hai aur chalte hue kitne?

**Kabir:** Do. Alag alag data ke saath.

**Madhav:** Toh file ek nuskha hai, aur chalta hua app us nuskhe se banaya gaya khaana. Ek nuskhe se kitne bhi khaane ban sakte hain, aur har khaana alag hota hai.

**Kabir:** Aur jab main app band karta hoon?

**Madhav:** Kya hota hai, socho.

**Kabir:** RAM wapas le li jaati hai. Jo usmein tha, gaya.

**Madhav:** Aur file?

**Kabir:** File wahi ki wahi hai. Disk pe.

**Madhav:** Isiliye band karke dobara kholne se app naye jaisa ho jaata hai. Tumne app ko theek nahi kiya. Tumne purana khaana phenk kar naya bana liya.

**Kabir:** Toh "restart karo" ka matlab yehi hai.

**Madhav:** Har baar yehi. Aur isiliye woh itni baar kaam kar jaata hai.

---

### Naam

Woh file jo disk pe padi hai, use **program** ya executable kehte hain.

Woh chalta hua dher, use **process** kehte hain.

Ek process mein kya kya hota hai:

```
┌─────────────────────────────────────────────┐
│  PROCESS                                    │
│                                             │
│  nirdesh          (file se copy kiye hue)   │
│  data ki jagah    (OS ne di hui)            │
│  program counter  (abhi kahan hoon)         │
│  registers        (abhi kya haath mein hai) │
│  khuli hui files, network ke raaste         │
│  kis user ka hai, kya kar sakta hai         │
└─────────────────────────────────────────────┘
```

Ek program se kai process ban sakte hain. Har process ka apna dabba hota hai, aur woh ek doosre ko dekh nahi sakte. Yeh Chapter 3.4 wala "alag rakhna" hai, ab shakal ke saath.

**Chalne ki haalatein**

Ek process hamesha chal nahi rahi hoti. Uski teen haalatein hoti hain:

```
CHAL RAHI      CPU abhi isi ke nirdesh chala rahi hai
TAIYAAR        chal sakti hai, bas baari ka intezaar hai
RUKI HUI       kisi cheez ka intezaar hai: disk, network, ya user
```

Aur ab ek baat jo bahut kuch samjha deti hai: **zyadatar process zyadatar waqt ruki hui hoti hain.**

Aapka chat app 99 pratishat waqt kuch nahi kar raha. Woh intezaar mein hai. Isiliye ek phone tees-chalees app "khule" rakh leta hai, jabki chip mein sirf aath hisse hain. Woh sab chal nahi rahe. Woh sab so rahe hain.

Chapter 2.3 ki baat, phir se: **CPU tez hai, intezaar lamba hai.** Poora system isi ek sachai ke aas-paas bana hua hai.

---

### Asli duniya se ek example

Jab aap phone pe ek app se doosre pe jaate ho, toh pehla app aksar band nahi hota. Woh "ruki hui" haalat mein chala jaata hai, aur uska data RAM mein pada rehta hai.

Agar RAM bhar jaaye, toh OS chup-chaap kisi purane app ka poora dher phenk deta hai.

Isiliye kabhi kabhi aap ek purane app pe wapas jaate ho aur woh shuru se khulta hai, jaise aapne use kabhi khola hi na ho. Woh crash nahi hua. OS ne use maar diya, kyunki jagah chahiye thi.

Aur isiliye zyada RAM wale phone "smooth" lagte hain. Woh tez nahi hain. Unmein app zinda rehte hain.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki "app band karne" se phone tez hota hai.**

Log baar baar saare app swipe karke band karte hain, yeh sochkar ki phone halka ho jaayega.

Zyadatar mamlon mein ulta hota hai. Ruki hui process CPU nahi le rahi thi. Woh sirf RAM mein padi thi, aur RAM ko khaali rakhne ka koi faayda nahi hai. Ab jab aap woh app dobara khologe, toh use disk se poora naye sire se load karna padega, jo mehnga hai.

OS pehle se hi jaanta hai ki kise phenkna hai aur kab. Woh aapse behtar jaanta hai.

Yeh galti tempting isliye hai ki "khula hua" ka matlab lagta hai "chal raha hai aur mehnat kar raha hai." Woh nahi hai. Zyadatar khule app sirf so rahe hain.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  PROCESS      file ≠ chalta hua app     │  ← naya
    │               chal rahi / taiyaar / ruki│
    ├────────────────────────────────────────┤
    │  OS           baari, jagah, alag rakhna │
    ├────────────────────────────────────────┤
    │  LANGUAGE, TRANSLATOR, CHUNAV           │
    ├────────────────────────────────────────┤
    │  CPU, RAM/DISK, PROGRAM, SWITCH         │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Aap ek document likh rahe ho, save nahi kiya, aur bijli chali jaati hai. Kya gaya aur kyun?

> **Jawab:** Jo aapne likha woh process ki RAM wali jagah mein tha. Bijli gayi toh RAM khaali ho gayi.
>
> File disk pe abhi bhi hai, us haalat mein jaisi aapne aakhri baar save ki thi.
>
> "Save" ka matlab hai process ki jagah se disk pe copy karna, jo Chapter 2.4 mein aaya tha.
>
> Aur isiliye aaj ke app har kuch second mein khud save karte rehte hain. Unhone problem hal nahi ki, unhone bas woh khidki chhoti kar di jismein nuksaan ho sakta hai.

**2. (samajh check)** Ek hi program se do process chal rahe hain. Ek crash ho jaata hai. Doosre pe kya asar?

> **Jawab:** Kuch nahi. Bilkul kuch nahi.
>
> Har process ka apna alag dher hai: apni jagah, apne registers, apna sab kuch. Woh ek hi file se bane hain, lekin ek doosre se jude nahi hain.
>
> Isiliye browser mein har tab aksar apna alag process hota hai. Ek page kharaab ho toh sirf woh tab marta hai, poora browser nahi.
>
> Yeh ek design ka faisla hai: alag rakhne mein zyada RAM lagti hai, lekin ek hissa toot ne pe baaki bach jaate hain. **Suraksha ki keemat jagah hai.**

**3. (jodne wala)** Chapter 1.6 mein "machine badalti nahi, sirf numbers badalte hain" tha. Process usi baat ka kaunsa hissa hai?

> **Jawab:** Process woh numbers hain, chalte hue.
>
> Machine wahi ek chip hai. Aap ek app kholte ho toh chip nahi badalti. RAM mein numbers ka ek naya dher aata hai, aur chip ab un numbers se guzarti hai.
>
> Band karo toh dher hat jaata hai. Chip phir bhi wahi hai.
>
> Isiliye ek chhoti si chip ek hi din mein hazaaron alag "machinein" ban jaati hai. Har process usi khaali machine ka ek naya roop hai.
