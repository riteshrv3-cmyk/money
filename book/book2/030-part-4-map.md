# Part 4 ka naksha aur gate

## Naksha, ab tak

```
┌──────────────────────────────────────────────────────────┐
│  PART 4   FILE SE JAWAB TAK                              │
│                                                          │
│   PREFILL     poora sawal ek saath padha jaata hai        │
│               chip bhara hua, hisaab bharpoor             │
│               ── "pehla shabd" ka waqt yahi hai           │
│                          ↓                                │
│   DECODE      ek token, phir agla, ek-ek karke            │
│               har token pe poori file memory se aati hai  │
│               chip khaali, sirf intezaar                  │
│               ── isliye output input se mehnga hai        │
│                          ↓                                │
│   CHUNAV      sambhavna ki list mein se ek token          │
│               temperature: kitna random                   │
│               ── yeh model ke BAHAR hai                   │
│                          ↓                                │
│   SEEMA       context window                              │
│               hisaab varg mein, memory seedhi             │
│               ── bhoolna = dobara bheja hi nahi gaya      │
├──────────────────────────────────────────────────────────┤
│  PART 3   embedding, attention, transformer               │
├──────────────────────────────────────────────────────────┤
│  PART 2   data, training, weights, dhalai                 │
├──────────────────────────────────────────────────────────┤
│  PART 1   token, sambhavna, ek-ek karke jawab             │
├──────────────────────────────────────────────────────────┤
│  BOOK 1   server, RAM, GPU, kharcha, cache, line          │
└──────────────────────────────────────────────────────────┘
```

## Chaar baatein jo Part 4 se nikli

**1. Do alag kism ke kaam hain.** Sawal padhna ek saath ho sakta hai. Jawab banana ek-ek karke hi hoga. Isliye do alag daam, do alag seemayein, do alag ilaaj.

**2. Asli kharcha numbers laane mein hai.** Isliye chip khaali baitha rehta hai, isliye kai sawal ek saath chalaye jaate hain, aur isliye bhari hui machine sasti aur khaali machine mehngi hai.

**3. Chunav model ke bahar hai.** Model sirf sambhavna deta hai. Ek token chunna product ka faisla hai, aur temperature 0 ka matlab "sahi" nahi, "dohraya ja sakne wala" hai.

**4. Context mein hona aur istemaal hona alag hain.** Bada context muft nahi hai, aur usmein beech ka hissa aksar dab jaata hai.

## Gate

**1.** Aapka pehla shabd der se aata hai lekin uske baad jawab tez aata hai. Kya theek karoge?

> **Jawab:** Prefill chhota karo, yaani kam sandarbh bhejo.
>
> Decode ki raftaar badalne se koi faayda nahi, kyunki woh hissa toh theek chal raha hai.
>
> **Do alag problem, do alag ilaaj. Unhe mila do toh aap galat cheez theek karoge.** *(4.2)*

**2.** Aap ek hi sawal paanch baar poochte ho aur paanch alag jawab aate hain. Achha ya bura?

> **Jawab:** Yeh ek naap hai, achha ya bura nahi.
>
> Ek jaise jawab matlab model us baat pe sthir hai. Alag alag jawab matlab woh andaza laga raha hai.
>
> Aur yeh uske aatmvishwas se kahin behtar naap hai, kyunki aatmvishwas ko dhaala gaya tha (Ch 2.8) aur yeh naap nahi. *(4.3)*

**3.** Ek lambi chat mein jawab dheere dheere kharaab ho rahe hain. Sabse aasan ilaaj?

> **Jawab:** Nayi chat, aur sirf zaroori cheez dobara likho.
>
> Kyunki teeno wajahein us ek kaam se hat jaati hain: kati hui shuruaat, bhara hua context, aur purani baat ka kheenchav. *(4.4, 3.2)*

## Chat app pe

```
Aapka sawal aur chune hue purane messages, sab ek saath padhe
jaate hain. Yeh prefill hai, aur isi mein pehla shabd ka waqt hai.

Phir jawab ek-ek token karke banta hai, aur har token pe poori
model file memory se aati hai. Isliye lamba jawab seedha mehnga hai.

Aapka sawal doosre sau logon ke saath ek batch mein chalta hai.
Isliye vyast waqt mein woh dheema lagta hai.

Aur aap poore paanch saal ke messages nahi bhej sakte. Toh kisi
ko pehle chunna padega ki kaunse das messages iss sawal ke kaam
ke hain.
```

Ab woh sawal jo abhi tak taala gaya hai. Aap sab kuch theek karte ho aur woh phir bhi ek cheez bana kar bata deta hai jo hai hi nahi.

**Woh cheezein bana kyun leta hai, aur uske saath kya kiya jaaye?** Yeh Part 5 hai, aur woh iss kitaab ka sabse practical part hai.
