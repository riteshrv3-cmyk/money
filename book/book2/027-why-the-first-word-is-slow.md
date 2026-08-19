# Chapter 4.2  [DEPTH]
## Pehla word slow kyun hota hai

*DEPTH chapter. Chhod sakte ho. Iske baad AI ki har keemat ki list samajh mein aati hai.*

### Samvaad

**Madhav:** Aap Enter dabate ho. Pehla shabd aane mein kitna waqt lagta hai?

**Kabir:** Ek do second.

**Madhav:** Aur uske baad shabd kis raftaar se aate hain?

**Kabir:** Tez. Lagbhag lagatar.

**Madhav:** Toh pehla shabd baaki sab se dheema hai. Kyun? Dono baar toh wahi model chal raha hai.

**Kabir:** Shayad shuru mein kuch taiyaari hoti hai.

**Madhav:** Sochte hain. Aapne do hazaar shabd ka sawal bheja. Pehla token banane se pehle model ko kya karna hai?

**Kabir:** Poore do hazaar shabd padhne hain. Sab layers se guzarna hai.

**Madhav:** Aur doosra token banane ke liye?

**Kabir:** Sirf ek naya shabd. Baaki ka kaam bacha hua hai. Pichhla chapter.

**Madhav:** Toh kitna farak hai?

**Kabir:** Pehli baar do hazaar shabd ka kaam. Uske baad ek shabd ka.

**Madhav:** Do hazaar guna.

**Kabir:** Toh isiliye pehla shabd dheema hai.

**Madhav:** Ab ek aur cheez. Pehle wale kaam mein, do hazaar shabd ek saath sambhale ja sakte hain ya ek ke baad ek?

**Kabir:** Ek saath. Attention mein kram ka intezaar nahi hai. Chapter 3.3.

**Madhav:** Aur uske baad wale kaam mein? Har naya token?

**Kabir:** Woh ek ke baad ek hi hoga. Kyunki agla token banane ke liye pichhla chahiye.

**Madhav:** Toh do bilkul alag kism ke kaam ho gaye.

**Kabir:** Pehla bada hai lekin ek saath ho sakta hai. Doosra chhota hai lekin ek-ek karke karna padta hai.

**Madhav:** Aur GPU kis mein achha hai?

**Kabir:** Ek saath wale mein.

**Madhav:** Toh doosre wale mein chip kaisa lagta hai?

**Kabir:** Khaali. Woh ek chhote se kaam ke liye poori file mangwa raha hai.

**Madhav:** Bas. Ab poori tasveer bolo.

**Kabir:** Pehla hissa: bada kaam, ek saath, chip poora bhara. Doosra hissa: chhota kaam, ek-ek karke, chip zyadatar khaali aur numbers ka intezaar.

**Madhav:** Aur inka daam bhi alag hoga?

**Kabir:** Hona chahiye. Ek mein hisaab bhara hua hai, doosre mein sirf laana-le jaana.

**Madhav:** Aur wahi hota hai. Isiliye har jagah do alag daam likhe hote hain.

### Naam

Do hisse, do naam:

```
PREFILL  (aapka sawal padhna)
├── poora sawal ek saath sambhala jaata hai
├── chip poori tarah bhara, hisaab bharpoor
├── waqt sawal ki lambai ke saath badhta hai
└── isi mein "pehla shabd aane tak ka waqt" jaata hai

DECODE  (jawab banana)
├── ek token, phir agla, ek-ek karke
├── har token pe poori file memory se aani padti hai
├── chip zyadatar khaali, sirf intezaar
└── isi se "shabd kitni tezi se aa rahe hain" tay hota hai
```

Aur isse teen cheezein seedhi nikalti hain, jo aap roz dekhte ho.

**Ek: input aur output ka daam alag hai.**

Har jagah do alag rate likhe hote hain, aur output aksar input se kai guna mehnga hota hai. Ab wajah saaf hai: input ek saath sambhala jaata hai, output ek-ek karke.

**Do: lamba sawal pehle shabd ko dheema karta hai. Lamba jawab poore waqt ko dheema karta hai.**

Do alag seemayein, do alag ilaaj:

```
pehla shabb der se aata hai   →  sawal chhota karo, kam sandarbh bhejo
poora jawab dheera hai        →  chhota jawab maango
```

**Teen: decode mein chip khaali baitha hai, aur wahi batching ki asli wajah hai.**

Chapter 4.1 mein humne dekha ki kai sawal ek saath chalaye jaate hain. Ab wajah gehri ho gayi: decode mein chip ke paas karne ko kuch hai hi nahi, toh usmein sau logon ka kaam daala ja sakta hai lagbhag muft mein.

**Isliye AI ka daam iss baat pe bahut nirbhar karta hai ki us waqt kitne log hain.** Yeh ek aisa karobaar hai jismein bhari hui machine sasti aur khaali machine bahut mehngi hai.

### Asli duniya se

Har badi AI service apni keemat ki list mein do alag numbers deti hai: input tokens ka daam, aur output tokens ka daam. Output aksar teen se paanch guna mehnga hota hai.

Ab aap jaante ho ki woh do numbers kyun hain. Woh marketing nahi hai. Woh do bilkul alag kism ke kaam hain.

Aur ek aur cheez jo isse nikalti hai: kuch services "cached input" ke liye aur bhi kam daam leti hain. Yaani agar aap wahi lamba sandarbh baar baar bhejte ho, toh uska prefill ka kaam bacha kar rakha ja sakta hai aur aapse kam liya jaata hai.

Wahi cache, phir se. Book 1 Chapter 5.5, ab AI ke bill pe.

### Yahan log kya galat samajhte hain

Sabse aam galti: **jawab ke waqt ko ek hi cheez samajhna.**

Do alag cheezein hain, aur unke ilaaj alag hain:

```
"pehla shabb aane mein der lagti hai"
    →  aapka sawal ya sandarbh bada hai

"shabd dheere dheere aa rahe hain"
    →  bojh zyada hai, ya model bada hai
```

Agar aap in dono ko mila do, toh aap galat cheez theek karoge.

Doosri galti: **yeh sochna ki lamba prompt "muft" hai kyunki woh sirf padha ja raha hai.**

Woh padha nahi ja raha. Uske har shabd ko sau layers se guzarna padta hai, aur attention ka kaam varg mein badhta hai (Chapter 3.3). Ek bahut lamba prompt pehle shabd ko kai second door kar sakta hai.

**Sandarbh muft nahi hai. Woh sirf output se sasta hai.**

### Sochne ke liye

**1. (samajh check)** Aapko ek aisa product banana hai jismein jawab turant dikhna chahiye. Kya karoge?

> **Jawab:** Prefill chhota karo.
>
> Kam sandarbh bhejo. Poori purani baat-cheet mat bhejo, sirf zaroori hissa. Poora document mat bhejo, sirf woh tukda jo kaam ka hai (Chapter 6.2).
>
> Aur agar wahi lamba sandarbh baar baar ja raha hai, toh dekho ki uska prefill cache ho sakta hai ya nahi.
>
> **Pehla shabd ka waqt lagbhag poora prefill hai. Use chhota karna hi ek matra ilaaj hai.**

**2. (samajh check)** Do product hain. Ek chhota jawab deta hai, doosra lamba aur poora. Kharche mein kitna farak?

> **Jawab:** Seedha anupaat, aur output ka daam input se kai guna zyada hai.
>
> Toh do guna lamba jawab lagbhag do guna mehnga hai, aur woh mehnga hissa poore bill ka bada hissa ho sakta hai.
>
> Isliye "sirf jawab do, samjhao mat" ek asli bachat hai, na ki sirf padhne ki suvidha.
>
> **Aur zyadatar mamlon mein aapko lamba jawab chahiye hi nahi tha.**

**3. (jodne wala)** Book 1 Ch 6.7 mein waqt ke paanch hisse the. Yahan wahi tarika lagao.

> **Jawab:** AI ke jawab ka waqt aise banta hai:
>
> ```
> network ka safar          Book 1 Ch 4.3
> line mein intezaar        bojh pe nirbhar (Ch 4.1)
> prefill                   sawal ki lambai
> decode                    jawab ki lambai
> network ka wapas safar
> ```
>
> Aur log aksar sirf aakhri do ko dekhte hain.
>
> Book 1 ka wahi sabak: **jab kuch dheema ho, poore raaste ko todo, ek hisse ko mat kosiye.** Aur aksar sabse bada hissa woh hota hai jispe kisi ka dhyaan nahi jaata.
