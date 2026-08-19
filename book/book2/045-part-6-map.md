# Part 6 ka naksha aur gate

## Naksha, ab tak

```
┌──────────────────────────────────────────────────────────┐
│  PART 6   ISE HAATH DENA                                 │
│                                                          │
│   MODEL KE PAAS KOI TAAKAT NAHI HAI                      │
│   woh sirf text banata hai                                │
│            ↓                                              │
│   RAG        pehle dhoondho, phir jawab do                │
│              yaaddasht se nahi, saamne rakhi cheez se     │
│            ↓                                              │
│   TOOLS      ek list jo program ne di                     │
│              model maangta hai, program karta hai         │
│              padhna aasani se, badalna soch kar,          │
│              mitana kabhi bina poochhe nahi               │
│            ↓                                              │
│   LOOP       karo, dekho, phir tay karo, dohrao           │
│              context bharta hai, galtiyan judti hain      │
│              seema hamesha honi chahiye                   │
│            ↓                                              │
│   KHATRA     model nirdesh aur data mein farak nahi karta │
│              bahar ka text ek hukum ban sakta hai         │
│              asli bachaav: tools kam, daayra chhota       │
├──────────────────────────────────────────────────────────┤
│  PART 5   hallucination, seemayein, jaanch                │
├──────────────────────────────────────────────────────────┤
│  PART 4   prefill, decode, temperature, context           │
├──────────────────────────────────────────────────────────┤
│  PART 3   embedding, attention, transformer               │
├──────────────────────────────────────────────────────────┤
│  PART 2   data, training, weights, dhalai                 │
├──────────────────────────────────────────────────────────┤
│  PART 1   token, sambhavna, ek-ek karke jawab             │
├──────────────────────────────────────────────────────────┤
│  BOOK 1   server, RAM, GPU, kharcha, git, protocol        │
└──────────────────────────────────────────────────────────┘
```

## Paanch baatein jo Part 6 se nikli

**1. Agent koi nayi cheez nahi hai.** Ek model, kuch tools, aur ek dohrav. Model ke andar kuch nahi badla.

**2. Model ke paas apna koi haath nahi hota, aur wahi ek bachaav hai.** Har kaam ek program se hokar jaata hai, aur woh program aapke haath mein hai.

**3. RAG model ko sikhaana nahi hai, use dikhana hai.** Isliye document badlo aur agla jawab turant naya. Aur jab jawab kharaab aaye, toh problem aksar dhoondhne mein hoti hai, model mein nahi.

**4. Model nirdesh aur data mein farak nahi kar sakta.** Isliye koi bhi webpage, email ya file ek hukum ban sakti hai. Iska koi poora hal abhi nahi hai.

**5. Bharosa tools kam karne se aata hai, model behtar hone se nahi.**

## Gate

**1.** Aapka AI assistant email padh bhi sakta hai aur bhej bhi sakta hai. Kya khatra hai aur kya karoge?

> **Jawab:** Koi bhi aapko email bhej sakta hai jismein nirdesh chhupe hon. Agent use padhega aur uske paas bhejne ka tool hai.
>
> Padhna aur bhejna, dono ek saath, yahi asli khatra hai.
>
> Ilaaj: draft banane do, bhejne ka button apne paas rakho. *(6.7, 6.3)*

**2.** RAG wala system galat jawab de raha hai. Model badal doge?

> **Jawab:** Pehle dekho ki kaunse tukde bheje gaye the.
>
> Agar sahi tukda bheja hi nahi gaya, toh naya model bhi wahi galat jawab dega. Problem dhoondhne mein hai.
>
> **RAG mein zyadatar nakaami dhoondhne ki hoti hai, model ki nahi.** *(6.2)*

**3.** Ek agent teen ghante chala aur nateeja galat hai. Sabse pehle kya dekhoge?

> **Jawab:** Har kadam ka record, shuru se.
>
> Galti aksar ek kadam pe hui aur baaki sab uske upar khade hain. Aakhri kadam dekhne se kuch nahi milega. *(6.4, 6.8)*

## Chat app pe

```
Ab hamara app poora ban gaya.

Aap poochte ho "pichhle mahine doctor ka kya zikr tha."

Woh aapke saare messages nahi bhejta. Woh pehle matlab se
dhoondhta hai aur das messages chunta hai. (6.2)

Woh un das ko sawal ke saath bhejta hai, aur nirdesh deta hai
ki sirf inhi se jawab do, aur source dikhao.

Model jawab likhta hai. Program us jawab ke saath woh asli
messages bhi dikhata hai. (5.4)

Agar aap kaho "us doctor ko email bhej do," toh woh draft
banata hai aur aapse poochta hai. Bhejta khud nahi. (6.3)

Aur jo message woh padhta hai, unmein koi bhi kuch bhi likh
sakta tha. Isliye uske paas bhejne ka tool hai hi nahi,
sirf draft banane ka. (6.7)
```

Yeh poora app hai, upar se neeche tak. Aur usmein ek bhi cheez aisi nahi hai jo aapne iss kitaab mein na banayi ho.

Ab aakhri Part. Ab tak humne dekha ki yeh cheez kaam kaise karti hai. Ab dekhenge ki **iska aap ke liye matlab kya hai**: paisa kahan hai, ek aadmi kya bana sakta hai, aur ise kaise chalaya jaaye.
