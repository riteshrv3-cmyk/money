# Part 2 ka naksha aur gate

## Naksha, ab tak

```
┌──────────────────────────────────────────────────────────┐
│  PART 2   MODEL BANTA KAISE HAI                          │
│                                                          │
│   DATA      web, kitaabein, code                         │
│             chhaana gaya, saaf kiya gaya, kaata gaya      │
│                     ↓                                     │
│   TRAINING  agla token chhupao, guess karwao,             │
│             galti naapo (loss), dhalaan nikalo,           │
│             numbers hilao, kharabon baar                  │
│                     ↓                                     │
│   WEIGHTS   kuch sau GB, ek nichod, ek copy nahi          │
│                     ↓                                     │
│   DHALAI    insaan ke examples, phir insaan ki pasand     │
│             yahin se "sahayak" wali shakal aati hai       │
│                     ↓                                     │
│   MODEL     ek sthir file + use chalane wala code         │
├──────────────────────────────────────────────────────────┤
│  PART 1     token, sambhavna, ek-ek karke jawab           │
├──────────────────────────────────────────────────────────┤
│  BOOK 1     server, RAM, kharcha, cache                   │
└──────────────────────────────────────────────────────────┘

    Aur ek sawal abhi khula hai:
    sambhavna nikalti kaise hai?  ── PART 3
```

## Paanch baatein jo Part 2 se nikli

**1. Do hi tareeke hain.** Niyam likho, ya examples dikhao. Doosra isliye bana ki kuch kaam pehle se ho hi nahi sakte. Jahan niyam likhe ja sakte hain, wahan niyam behtar hain.

**2. Jawab data mein pehle se tha.** Kisi insaan ko har example ka jawab nahi likhna pada. Isi ek chaalaki ne paimana mumkin banaya.

**3. Model ek nichod hai, copy nahi.** Jo baar baar aaya woh bacha. Jo ek baar aaya woh lagbhag gaya. Aur model ko khud pata nahi ki kya bacha.

**4. Jo aap naapte ho wahi milta hai.** Loss ne sirf agla token naapa. Sach naapa hi nahi gaya. Uske baad insaan ki pasand naapi gayi, sach phir bhi nahi.

**5. Model ki kamzori ke teen alag kaaran hain**, aur teeno bahar se ek jaise dikhte hain:

```
duniya mein woh cheez kam likhi gayi     (2.6)
nichodne mein woh gayab ho gayi          (2.3)
safai ne use jaan-boojh ke kaat diya     (2.7)
```

## Gate

**1.** Model aapko aatmvishwas se galat jawab deta hai. Part 2 se do alag wajahein batao.

> **Jawab:**
>
> **Ek:** woh baat data mein kam thi, isliye nichodne mein gayab ho gayi. Aur woh chup nahi reh sakta, kyunki uska kaam agla token chunna hai. Toh woh woh likhta hai jo aisi jagah pe aksar likha hota hai. *(2.3, 2.6)*
>
> **Do:** use aatmvishwas ke liye dhaala gaya hai. Insaanon ne bhare andaz wale jawab chune, isliye woh us taraf jhukta hai. *(2.8)*
>
> Pehli wajah gyaan ki hai. Doosri swabhav ki. Dono milkar sabse khatarnak jodi banti hain.

**2.** Ek dost kehta hai "main isse baat karke ise train kar raha hoon." Kya yeh sahi hai?

> **Jawab:** Nahi. Uski file badal hi nahi rahi. Training ek alag waqt pe, alag jagah, mahinon mein hui thi.
>
> Do cheezein jo aisa lagne deti hain: usi chat mein purani baat dobara bheji jaati hai (1.2), aur company aapki baat rakh kar **agle** model ki training mein daal sakti hai (2.2).
>
> Doosri baat ka matlab hai ki aapki baat kahin rakhi ja rahi hai. Chapter 6.6.

**3.** Ek company apna model muft mein public kar deti hai. Kyun?

> **Jawab:** Book 1 Ch 3.6 ke wahi kaaran: neeche wali parat pe kabza, taaki log unke upar cheezein banayein. Naam aur saabiti. Aur yeh ki na dene se koi aur de dega.
>
> Aur uski keemat bhi wahi hai: sabse mehngi cheez de di, ab paisa kahin aur se banana padega.
>
> Jo bacha hai woh file se bada hai: data, paimana, product, aur agli file banane ki kaabiliyat.

## Chat app pe

Hamara app aapke messages ke baare mein sawal ka jawab dega. Part 2 ke baad:

```
Jo model woh istemaal karega, use kisi aur ne banaya, mahinon mein,
karodon dollar mein, us data pe jo aapke messages se koi rishta
nahi rakhta.

Woh aapke messages ke baare mein kuch nahi jaanta. Woh ek nichod
hai duniya ki likhawat ka, ek tarikh tak.

Toh aapke messages use sawal ke saath bhejne padenge, har baar.
Woh unhe seekh nahi sakta.

Aur uska jawab dene ka andaz, uski vinamrata, uska sehmat hona,
sab ek aakhri parat se aaya hai jo kisi ne jaan-boojh ke dhaali.
```

Ab woh sawal jo Part 1 se khula pada hai:

**Woh yeh kaise tay karta hai ki agla token kya hoga? Sambhavna aati kahan se hai?** Yeh Part 3 hai.
