# Chapter 1.5  [DEPTH]
## Switches jodte kaise hain

---

*Yeh DEPTH chapter hai. Ismein aap ek machine ko andar se banta hua dekhoge. Pehli baar mein chhod sakte ho, lekin agar ek baar bhi dekh liya ki shartein kaam kaise karti hain, toh "computer jaadu hai" wali soch hamesha ke liye khatam ho jaati hai.*

---

### Samvaad

**Madhav:** Ek switch faisla karta hai. Kaafi switch numbers rakhte hain. Ab dono ko jodo: kya switch **jod** sakte hain?

**Kabir:** Pata nahi.

**Madhav:** Chalo banate hain. Sabse chhota jod. Ek bit aur ek bit. Chaar mumkin case hain, batao.

**Kabir:** 0 aur 0. 0 aur 1. 1 aur 0. 1 aur 1.

**Madhav:** Jawab kya hain?

**Kabir:** 0, 1, 1, aur... 2.

**Madhav:** Ruko. Ek bit mein 2 aa sakta hai?

**Kabir:** Nahi. Ek bit mein sirf 0 ya 1.

**Madhav:** Toh kya karoge?

**Kabir:** Do jagah chahiye. Jaise 9 aur 9 jodte hain toh 18 hota hai, do ank.

**Madhav:** Bilkul. Toh jawab ke do hisse honge. Ek jo wahin dikhta hai, aur ek jo aage jaata hai. Chaaron case dobara likho, ab do hisson mein.

**Kabir:**
```
0 + 0  →  wahin 0,  aage 0
0 + 1  →  wahin 1,  aage 0
1 + 0  →  wahin 1,  aage 0
1 + 1  →  wahin 0,  aage 1
```

**Madhav:** Ab pehle "aage" wale khaane ko dekho. Woh kab 1 hota hai?

**Kabir:** Sirf jab dono 1 hon.

**Madhav:** Aur "dono 1 hon" ka gate?

**Kabir:** AND!

**Madhav:** Toh aage jaane wala hissa ek AND gate hai. Bas. Ab "wahin" wale khaane ko dekho. Woh kab 1 hota hai?

**Kabir:** Jab ek 1 ho aur doosra 0. Yaani jab dono alag hon.

**Madhav:** Aur "dono alag hain" ko humne pichhle chapter mein banaya tha. Yaad hai?

**Kabir:** Haan. "A aur B-nahi" ya "A-nahi aur B." AND, NOT aur OR se.

**Madhav:** Toh tumne abhi kya bana diya?

**Kabir:** Jodne wali machine? Sirf gates se?

**Madhav:** Ek bit ki. Ab badi karte hain. Aath bit ke do numbers jodne hain. Kya karoge?

**Kabir:** Wahi cheez aath baar lagaunga. Har jagah pe do bit jodunga.

**Madhav:** Aur jo "aage" wala hissa nikla tha?

**Kabir:** Woh agli jagah mein daal dunga. Jaise haath se jodte waqt hasiya aage le jaate hain.

**Madhav:** Toh ab tumhe har jagah pe teen cheezein jodni hain: do numbers ke bit, aur pichhli jagah se aaya hua.

**Kabir:** Toh do jodne wali machine ek ke baad ek laga dunga. Pehle do jodo, phir uss jawab mein teesra jodo.

**Madhav:** Bas. Aur ab aath jagah, ek line mein, har ek agli ko apna hasiya de rahi hai. Tumne abhi ek asli chip ka hissa bana diya, sirf AND, OR aur NOT se.

**Kabir:** Lekin sirf jodna hi toh hai.

**Madhav:** Ghatana kya hai?

**Kabir:** Ulta jodna.

**Madhav:** Guna?

**Kabir:** Baar baar jodna.

**Madhav:** Bhaag?

**Kabir:** Baar baar ghatana.

**Madhav:** Toh ek jodne wali machine se saara ganit nikal aaya. Aur woh machine sirf switch hai. Ab aakhri sawal: ek chip mein aisi kitni machinein hoti hain?

**Kabir:** Kai hazaar?

**Madhav:** Karodon. Aur woh ek second mein arbon baar chalti hain. Isiliye tumhara phone ek video chala pata hai, jo har second mein karodon numbers ka hisaab hai.

---

### Naam

Jo aapne abhi banaya, uska naam hai **adder**.

Ek bit wale hisse ko **full adder** kehte hain, kyunki woh teen cheezein jodta hai: do bit aur pichhla hasiya.

Aur jo teen hisse mile:

```
"wahin dikhne wala" hissa    →  XOR gate  ("dono alag hain")
"aage jaane wala" hissa      →  AND gate
inhe jodne wala              →  OR gate
```

Aath ya solah ya chausath aise hisse ek line mein lagao, aur aapke paas ek poora jodne wala circuit hai.

Aur ab ek baat jo pehli baar ajeeb lagti hai. **Chip ko yeh nahi pata ki woh jod rahi hai.**

Usmein bijli aati hai, shartein us bijli ko rokti aur jaane deti hain, aur doosri taraf se kuch nikal aata hai. Jodna sirf iss baat ka naam hai ki humne jo bahar aaya use kaise padha.

Chapter 1.4 ka jumla, wapas:

> Andar sirf numbers hain. Matlab hamesha bahar se aata hai.

---

### Asli duniya se ek example

1642 mein Blaise Pascal ne, 19 saal ki umar mein, ek jodne wali machine banayi. Usmein bijli nahi thi, sirf gear the. Har gear pe das dant, aur jab ek gear poora ghoom jaata tha toh woh agle gear ko ek dant aage kar deta tha.

Wahi hasiya. Sirf loha.

Uske teen sau saal baad wahi cheez switchon se bani, aur ek gear ki jagah ek transistor aaya. Idea nahi badla. Sirf hasiya le jaane wali cheez dhaatu se bijli ban gayi, aur uske saath speed lakhon guna ho gayi.

Yeh dekhna kaam ka hai: computer ka koi bhi idea naya nahi hai. Naya sirf yeh hai ki woh kitna chhota aur kitna tez ho gaya.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki chip ke andar ganit ke niyam likhe hain.**

Log sochte hain ki kahin ek jagah "2 + 2 = 4" jaisa kuch bhara hua hai, ya koi table hai jise dekh kar machine jawab batati hai.

Aisa kuch nahi hai. Koi jawab kahin rakha hua nahi hai. Bijli sharton mein se guzarti hai aur jawab **ban jaata hai**, har baar naye sire se.

Yeh galti tempting isliye hai ki jab hum jodte hain toh hum yaad se karte hain. Humne bachpan mein table ratay the. Toh lagta hai machine bhi yaad se karti hogi.

Machine yaad nahi karti. Woh har baar naye sire se banati hai, aur usse itni tezi se banati hai ki yaad karna dheema padta.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  GANIT        jod, ghatao, guna, bhaag │  ← naya
    ├────────────────────────────────────────┤
    │  ENCODING     number ka matlab kya hai │
    ├────────────────────────────────────────┤
    │  BINARY       kaafi switch = koi number│
    ├────────────────────────────────────────┤
    │  SHARTEIN     AND, OR, NOT             │
    ├────────────────────────────────────────┤
    │  SWITCH       1 ya 0                   │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

Har sawal pe ek minute socho, phir neeche jawab padho.

**1. (samajh check)** Aath bit se sabse bada number 255 hota hai. Ab 255 aur 1 jodo. Machine kya karegi?

> **Jawab:** Har jagah pe hasiya aage jaayega, aur aakhri hasiya ke paas jaane ki jagah hi nahi bachegi. Jawab 0 aa jaayega.
>
> Machine ise galti nahi maanegi. Uske paas aath jagah hain, usne aath jagah bhar di.
>
> Iska naam **overflow** hai, aur yeh asli duniya mein cheezein toda karta hai. Purane games mein score ek had ke baad zero ho jaata tha. Kuch systems mein tareekh ek din ke baad wapas peeche chali jaati hai.
>
> Seekhne wali baat: **machine ke paas jagah tay hoti hai, aur jagah khatam hone pe woh rukti nahi, woh chup-chaap galat jawab de deti hai.**

**2. (samajh check)** Adder mein har jagah apna hasiya agli jagah ko deti hai. Toh chausath bit ke numbers jodne mein, aakhri jagah ko kitna intezaar karna padega?

> **Jawab:** Use pichhli teiyasath jagahon ka intezaar karna padega, kyunki hasiya ek-ek karke aage aata hai.
>
> Isiliye zyada bit wala jod thoda dheema hota hai. Har jagah ka intezaar jud jaata hai.
>
> Asli chip mein iske liye alag design lagaye jaate hain jo hasiya pehle se andaz laga lete hain, taaki intezaar kam ho. Woh zyada transistor lete hain aur tez chalte hain.
>
> Yeh iss kitaab ka pehla **trade-off** hai: **zyada jagah kharch karo aur tez ho jao, ya kam jagah lo aur dheere chalo.** Yeh chunav aage har parat pe milega.

**3. (jodne wala)** Chapter 1.3 mein Kabir ne "dono alag hain" wali shart AND, OR aur NOT se banayi thi. Aaj wahi shart adder ka aadha hissa nikli. Isse aap kya seekhte ho?

> **Jawab:** Ki chhoti shartein bade tukdon ke purze ban jaati hain, aur wahi tukde aur bade tukdon ke.
>
> Aapne kabhi bhi teen se zyada cheezein istemaal nahi kin. AND, OR, NOT. Unse "alag hain" bana. Usse adder bana. Adder se ganit bana.
>
> Yehi poori kitaab ka dhaancha hai. Har parat neeche wali ke tukdon ko jodkar ek naya tukda banati hai, aur uske baad us naye tukde ko koi neeche ki taraf nahi dekhta.
>
> Isiliye jab aage koi badi cheez aaye, toh yeh mat poochna ki woh kaise mumkin hai. Poochna ki **woh kis cheez se bani hai.**
