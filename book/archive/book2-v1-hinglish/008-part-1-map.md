# Part 1 ka naksha aur gate

## Naksha, ab tak

```
┌──────────────────────────────────────────────────────────┐
│  MODEL                                                   │
│  ek badi file, kuch sau GB, sirf numbers                 │
│  aur woh numbers kisi ne likhe hi nahi                    │
│  ── woh kaise bane? PART 2                                │
├──────────────────────────────────────────────────────────┤
│  TOKEN                                                    │
│  text shabdon mein nahi, tukdon mein tootta hai           │
│  aam shabd ek token, ajeeb shabd kai                      │
│  akshar model ko dikhte hi nahi                           │
├──────────────────────────────────────────────────────────┤
│  TAREEKA                                                  │
│  ab tak ka saara text dekho                               │
│  har mumkin agle token ki sambhavna nikalo                │
│  ek chuno, jodo, dobara                                   │
│  ── sambhavna kaise nikalti hai? PART 3                   │
├──────────────────────────────────────────────────────────┤
│  BOOK 1                                                   │
│  server, RAM, network, kharcha, cache                     │
└──────────────────────────────────────────────────────────┘
```

## Char baatein jo Part 1 se nikli

**1. Teesri tarah ke numbers.** Photo ke numbers duniya se aaye, program ke numbers insaan se, aur model ke numbers ek process se. Kisi ne unhe likha nahi.

**2. Usmein yaaddasht nahi hai.** Har baar poori purani baat dobara bheji jaati hai. Woh dohrana hai, yaad rakhna nahi.

**3. Sabse achha jawab bhi aksar galat hoga.** Woh hamesha sabse sambhavit tukda chunta hai, aur woh tareeka hi kuch galtiyan pakki kar deta hai.

**4. Uski aankh ki ek shakal hai.** Woh tokens dekhta hai, akshar nahi. Kuch kaam isliye mushkil hain ki woh sach mein mushkil hain, aur kuch isliye ki woh dikhte hi nahi.

## Gate

**1.** Model se poochte ho ki ek shabd mein kitne 'r' hain aur woh galat batata hai. Do alag wajahein batao. *(1.4, 1.5)*

> **Jawab:**
>
> **Ek:** use akshar dikhte hi nahi. Woh shabd ko do-teen numbers ki tarah dekh raha hai, aur un numbers ke andar akshar nahi hote.
>
> **Do:** ginna ek kaam hai, likhawat nahi. Woh yeh chun raha hai ki aisi jagah pe kaunsa number aksar likha hota hai, gin nahi raha.
>
> Aur ilaaj pehli wajah ka hai: shabd ko akshar-akshar karke do, aur woh gin lega.

**2.** Aap ek lambi baat-cheet karte ho. Har naya sawal pehle se mehnga hota jaata hai. Kyun? *(1.2)*

> **Jawab:** Kyunki model ko yaad kuch nahi rehta. Har naye sawal ke saath poori purani baat-cheet dobara bheji jaati hai.
>
> Toh dasva sawal pehle se nau guna zyada text le kar jaata hai, aur daam tokens pe hai.
>
> Yeh Chapter 4.5 aur 7.1 mein wapas aayega.

**3.** Ek dost ek galat jawab dikha kar kehta hai "yeh cheez bekaar hai." Kya jawab doge? *(1.3)*

> **Jawab:** Ki ek ghatna se kuch saabit nahi hota.
>
> Sambhavna ek baar ke baare mein kuch nahi kehti. Ek galat jawab utna hi bemaani hai jitna ek sahi jawab.
>
> Kaam ka tareeka: wahi kaam bees baar karo jo aap sach mein karte ho, aur ginti karo. Kitni baar sahi, aur galat hone pe kitna nuksaan hua.

## Chat app pe

Hamara app ab aapke messages ke baare mein sawal ka jawab dega. Part 1 ke baad itna pata hai:

```
aapka sawal aur aapke messages, dono tokens mein badalte hain
woh sab ek server pe jaate hain, kisi aur ki machine pe
wahan ek badi file khuli padi hai jise kisi ne likha nahi
jawab ek-ek token karke banta hai, aur har token pichhle
    saare tokens ko dekh kar chuna jaata hai

aur uska daam tokens mein hai, isliye jitne zyada purane
    messages aap bhejoge, utna mehnga
```

Ek sawal jo ab khula hai, aur Part 2 usi pe hai:

**Un numbers ko kisi ne likha nahi. Toh woh bane kaise?**
