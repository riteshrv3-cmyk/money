# Chapter 1.4  [SPINE]
## Switches numbers kaise rakhte hain

---

### Samvaad

**Madhav:** Ek switch se kitne numbers dikha sakte ho?

**Kabir:** Do. 0 aur 1.

**Madhav:** Do switch se?

**Kabir:** Chaar haalatein hain. Toh 0, 1, 2, 3.

**Madhav:** Likh ke dikhao. Kaunsi haalat kaunsa number hai?

**Kabir:** Dono band ko 0 kehta hoon. Phir 01 ko 1. Phir 10 ko 2. Phir 11 ko 3.

**Madhav:** Tumne yeh order kyun chuna?

**Kabir:** Bas... ginti jaisi lagi.

**Madhav:** Woh ginti jaisi hai. Ab teen switch se ginti karo, 0 se shuru.

**Kabir:** 000, 001, 010, 011, 100, 101, 110, 111. Aath haalatein. 0 se 7.

**Madhav:** Aur tumne ginti kaise ki? Kya niyam laga rahe the?

**Kabir:** Dayen se badhata gaya. Jab 1 ke aage badhna tha toh use 0 kar ke agle ko 1 kar diya.

**Madhav:** Bilkul wahi jo tum aam ginti mein karte ho. 9 ke baad 0 likh kar aage 1 badhate ho. Sirf yahan 9 ki jagah 1 pe hi bharav ho jaata hai, kyunki sirf do nishaan hain.

**Kabir:** Toh yeh koi nayi ginti nahi hai. Bas kam nishaan hain.

**Madhav:** Bas itna hi. Aam ginti mein das nishaan hain, 0 se 9. Yahan do hain. Aur kuch nahi badla.

**Kabir:** Lekin fayda kya hua? 7 likhne ke liye teen switch lag gaye. 7 toh ek nishaan hai.

**Madhav:** Sahi sawal. Ab dhyaan se dekho. Teen switch se 8 haalatein. Chaar se?

**Kabir:** Solah.

**Madhav:** Aath switch se?

**Kabir:** 2 ko aath baar guna... 256.

**Madhav:** Solah switch se?

**Kabir:** 65,000 ke aas-paas.

**Madhav:** Tees switch se?

**Kabir:** Bahut zyada. Karodon.

**Madhav:** Ek arab se upar. Ab yeh dekho: switch tees hain, lekin numbers ek arab. Har naya switch **dugna** karta hai. Isiliye tumhara sawal ulta ho gaya. Sawal yeh nahi hai ki 7 ke liye teen switch kyun lage. Sawal yeh hai ki tees switch se ek arab kaise aa gaye.

**Kabir:** Theek hai. Toh numbers ban gaye. Lekin mujhe toh naam bhi likhne hain, gaane bhi.

**Madhav:** Ek kaam karo. Ek kaagaz pe likho: A ke liye 1, B ke liye 2, C ke liye 3. Aage bhi.

**Kabir:** Kar liya.

**Madhav:** Ab "CAB" likho, sirf numbers mein.

**Kabir:** 3, 1, 2.

**Madhav:** Aur maine tumhe woh kaagaz diya hota, toh main 3-1-2 padh kar kya samajhta?

**Kabir:** CAB.

**Madhav:** Toh akshar kya hain?

**Kabir:** Numbers. Bas hum unhe alag dikhate hain.

**Madhav:** Rang?

**Kabir:** Rang bhi number ho sakta hai. Laal ka ek number, neela ka doosra.

**Madhav:** Ek photo?

**Kabir:** Photo... bahut saare chhote dabbe, har dabbe ka ek rang, har rang ek number.

**Madhav:** Aur awaaz?

**Kabir:** Awaaz toh lehar hai. Uski unchai bhi number ho sakti hai. Har pal ka ek number.

**Madhav:** Toh ek switch se 0 aur 1 mile. Kaafi switch se koi bhi number mila. Aur ek tay-shuda list se, koi bhi number kisi bhi cheez ka matlab ban gaya. Ab batao, aisa kya hai jo computer mein nahi daala ja sakta?

**Kabir:** Aisi cheez jise number mein badalne ka koi tareeka hi na ho.

**Madhav:** Bilkul sahi. Aur yeh yaad rakhna, kyunki agla pura hissa isi pe khada hai.

---

### Naam

Ek switch ki haalat ko **bit** kehte hain. Bit ka matlab hai: ek haan-na, 0 ya 1.

Sirf do nishaanon wali ginti ko **binary** kehte hain.

Aur woh tay-shuda list jismein likha ho ki kaunsa number kaunsi cheez ka matlab hai, use **encoding** kehte hain.

Yeh teesri cheez sabse zaroori hai aur sabse kam samjhi jaati hai. Number khud kuch nahi kehta.

```
number 3  →  agar akshar ki list dekhein     →  C
number 3  →  agar rang ki list dekhein       →  koi rang
number 3  →  agar seedha number ho           →  teen
number 3  →  agar niyam ki list dekhein      →  "jodo"
```

Ek hi 3, chaar alag matlab. Farak sirf iss baat ka hai ki aap kaunsi list dekh rahe ho.

**Computer ke andar sirf numbers hain. Matlab kabhi bhi andar nahi hota.** Matlab is baat mein hai ki unhe padha kis tarah jaa raha hai.

Yeh baat aage bahut kaam aayegi. Jab file kharaab ho jaati hai, jab akshar ki jagah ajeeb nishaan aate hain, jab ek program doosre ki file nahi khol paata, tab lagbhag hamesha wajah yehi hoti hai: numbers sahi hain, list galat lagayi gayi.

---

### Asli duniya se ek example

1963 mein America mein ek list tay ki gayi jiska naam ASCII tha. Usmein 128 nishaanon ke liye numbers tay kiye gaye: angrezi ke akshar, ginti ke ank, aur kuch chinh.

128 numbers ke liye saat bit kaafi hain. Us zamane mein har bit mehnga tha, isliye chhoti list rakhi gayi.

Problem yeh thi ki usmein duniya ki baaki bhaashaayein thi hi nahi. Hindi nahi, Chinese nahi, Arabic nahi. Har desh ne apni alag list banayi, aur ab ek desh ki file doosre desh mein kholo toh bakwaas dikhta tha. Numbers theek pahunchte the, list galat lagti thi.

Iska hal 1990 ke baad aaya, jab **Unicode** bani: ek hi list, duniya ki lagbhag har likhavat ke liye, aur usmein aaj lagbhag 1,50,000 se zyada nishaan hain.

Aaj aapke phone mein hindi, angrezi aur emoji ek hi message mein saath chalte hain. Woh isliye ki poori duniya ne ek list pe sehmati bana li. Naya hardware nahi laga. Sirf ek list.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki computer ke andar akshar, photo aur gaane rakhe hote hain.**

Log kehte hain "file mein meri photo hai." Photo file mein nahi hai. File mein numbers hain, aur ek tay-shuda tareeka hai unhe rang mein badalne ka.

Yeh sirf shabdon ka khel nahi hai. Iska seedha nateeja hai. Jab aapki file kharaab ho jaati hai aur ajeeb nishaan dikhte hain, tab log sochte hain ki file "toot gayi." Aksar file bilkul theek hoti hai. Sirf padhne wali list galat lag rahi hai.

Yeh galti tempting isliye hai ki aap photo ko photo ki tarah hi dekhte ho. Number kabhi dikhte hi nahi. Screen pe woh parat pehle hi hat chuki hoti hai.

Ek jumla yaad rakh lo, aage bees jagah kaam aayega:

> Andar sirf numbers hain. Matlab hamesha bahar se aata hai.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  ENCODING     number ka matlab kya hai │  ← naya
    ├────────────────────────────────────────┤
    │  BINARY       kaafi switch = koi number│  ← naya
    ├────────────────────────────────────────┤
    │  SHARTEIN     AND, OR, NOT             │
    ├────────────────────────────────────────┤
    │  SWITCH       1 ya 0                   │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

Har sawal pe ek minute socho, phir neeche jawab padho.

**1. (samajh check)** Aath bit se 256 alag haalatein banti hain. Agar aapko duniya ki har bhaasha ke akshar rakhne hain, toh 256 kaafi hai? Agar nahi, toh kya karoge?

> **Jawab:** Bilkul kaafi nahi hai. Akele Chinese mein hazaaron nishaan hain.
>
> Hal seedha hai: **zyada bit lo.** Solah bit se 65,000 se zyada. Ikkis bit se bees lakh se zyada, jo duniya ki har likhavat ke liye kaafi hai.
>
> Aur Unicode ne yehi kiya, ek hoshiyaari ke saath: aam angrezi akshar aaj bhi aath bit lete hain, aur jo nishaan kam aate hain woh zyada bit lete hain. Isse purani ASCII files bhi chalti rahin aur nayi bhaashaayein bhi aa gayin.
>
> Yeh soch aage bar bar dikhegi: **jo cheez zyada aati hai use sasta rakho, jo kam aati hai use mehnga hone do.**

**2. (samajh check)** Aapke paas ek file hai jismein numbers hain: 72, 101, 108, 108, 111. Aapko nahi pata ki yeh photo hai, gaana hai, ya likhawat. Kya aap sirf numbers dekh kar bata sakte ho?

> **Jawab:** Nahi. Aur yeh iss chapter ki sabse zaroori baat hai.
>
> Woh numbers ASCII list se "Hello" hain. Rang ki list se paanch alag halke rang hain. Awaaz ki list se ek chhoti si lehar.
>
> Numbers khud nahi batate ki woh kya hain.
>
> Isiliye file ke naam ke aage `.jpg` ya `.mp3` lagta hai. Woh file ka hissa nahi hai. Woh ek chit hai jo batati hai ki kaunsi list lagani hai. Chit badal do, aur wahi numbers kuch aur ban jaate hain.

**3. (jodne wala)** Chapter 0.4 kehta tha ki har parat neeche wali ko chhupa deti hai. Iss chapter mein kaunsi parat kis cheez ko chhupa rahi hai?

> **Jawab:** Encoding, binary ko chhupa rahi hai.
>
> Jab aap "A" likhte ho, toh aap 65 nahi soch rahe. Aur jab machine 65 rakhti hai, toh woh 01000001 nahi soch rahi. Aur jab woh 01000001 rakhti hai, toh woh aath switchon ke baare mein nahi soch rahi.
>
> Teen parat, ek hi cheez pe khadi.
>
> Yeh iss kitaab ki pehli jagah hai jahan aapne parat banti hui dekhi hai, bani hui nahi. Aage har part mein yeh dobara hoga.
