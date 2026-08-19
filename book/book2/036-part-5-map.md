# Part 5 ka naksha aur gate

## Naksha, ab tak

```
┌──────────────────────────────────────────────────────────┐
│  PART 5   JAB YEH GALAT HOTA HAI                         │
│                                                          │
│   HALLUCINATION   teen wajahein, teeno humne banayi:      │
│                   1. uska kaam hi agla token dena hai     │
│                   2. usmein khaali jagah nahi dikhti      │
│                   3. aatmvishwas ke liye dhaala gaya      │
│                   ── hataya nahi ja sakta, kam ho sakta   │
│                                                          │
│   SEEMAYEIN       AANKH KI: tools se hat ti hain          │
│                   ANDAR KI: insaan chahiye                │
│                   ── farak jaanna hi asli hunar hai       │
│                                                          │
│   NAAP            benchmark: teen kamzoriyan              │
│                   apna chhota test: bees sawal            │
│                                                          │
│   JAANCH          hamesha model ke BAHAR se               │
│                   sthirta naapo, aatmvishwas nahi         │
│                   sawal mein apna jawab mat daalo         │
├──────────────────────────────────────────────────────────┤
│  PART 4   prefill, decode, temperature, context           │
├──────────────────────────────────────────────────────────┤
│  PART 3   embedding, attention, transformer               │
├──────────────────────────────────────────────────────────┤
│  PART 2   data, training, weights, dhalai                 │
├──────────────────────────────────────────────────────────┤
│  PART 1   token, sambhavna, ek-ek karke jawab             │
├──────────────────────────────────────────────────────────┤
│  BOOK 1   server, RAM, GPU, kharcha, cache                │
└──────────────────────────────────────────────────────────┘
```

## Chaar baatein jo Part 5 se nikli

**1. Hallucination design ka nateeja hai, bug nahi.** Aur woh wahan sabse zyada hota hai jahan sawal sabse khaas aur chhota ho, na ki jahan woh sabse mushkil ho.

**2. Do kism ki seemayein hain.** Aankh ki seemayein tools se hat ti hain aur tezi se hat rahi hain. Andar ki seemayein lagbhag nahi hilee hain. Kis pe daanv lagana hai, yeh faisla wahin se aata hai.

**3. Benchmark aapke kaam ke baare mein kuch nahi kehta.** Bees sawal ka apna test us se kahin zyada kaam ka hai.

**4. Har asli jaanch model ke bahar se aati hai.** Ek cheez khud ko nahi jaanch sakti.

## Gate

**1.** Aap AI se ek chhota, khaas tathya poochte ho aur woh aatmvishwas se galat batata hai. Poori wajah batao.

> **Jawab:** Teen cheezein ek saath.
>
> Us baat ka data kam tha, isliye nichodne mein woh gayab ho gayi (2.3, 2.6). Us jagah pe khaali jagah nahi dikhti, sirf milta-julta nichod dikhta hai (2.3). Aur woh chup nahi reh sakta, kyunki uska kaam agla sambhavit token dena hai (1.4).
>
> Aur uske upar: use aatmvishwas ke liye dhaala gaya tha (2.8).
>
> **Sawal jitna khaas, khatra utna zyada.** Yeh ulta lagta hai aur yeh sabse kaam ki baat hai.

**2.** Aap ek system bana rahe ho jismein AI ke jawab aage kisi customer ko jaayenge. Kya karoge?

> **Jawab:** Kaam ko aise todo ki har hissa bahar se jaancha ja sake.
>
> Jaankari saath bhejo, yaaddasht pe mat chhodo (5.1). Jawab aisi shakal mein maango jo machine jaanch sake (5.4). Numbers, naam aur tarikhein hamesha jaancho. Aur apna bees sawal ka test rakho (5.3).
>
> Jo mat karo: model se hi uski jaanch karwaana, aur uske aatmvishwas pe bharosa karna.

**3.** Naya model aata hai jo har benchmark mein aage hai. Aap apne product mein badal doge?

> **Jawab:** Pehle apne bees sawal chalao, dono pe.
>
> Aur sirf sahi-galat mat dekho: daam, raftaar, aur jawab ki shakal bhi dekho.
>
> **Benchmark yeh batata hai ki dekhna chahiye. Woh yeh nahi batata ki badal do.**

## Chat app pe

```
Aapka app aapke messages ke baare mein jawab dega. Ab aap
jaante ho ki woh kahan galat hoga.

Ek khaas tarikh, ek chhota naam, ek aisa message jo sirf ek
baar aaya: yahin woh sabse zyada aatmvishwas se galat hoga.

Toh use yaad se jawab dene mat do. Har jawab ke saath woh asli
message dikhao jispe woh khada hai. Agar woh message nahi dikha
sakta, toh jawab bhi nahi dena chahiye.

Yeh "AI ko sahi banana" nahi hai. Yeh use dhoondhne wala banana
hai, jaanne wala nahi.
```

Aur wahi ek line poore agle Part ko khol deti hai. Agar model ko bahar ki cheez chahiye, aur woh khud kuch chhoo nahi sakta:

**Use haath kaise diye jaate hain?** Yeh Part 6 hai.
