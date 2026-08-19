# Chapter 3.3  [SPINE]
## Kaunsa word kis pe depend karta hai

### Samvaad

**Madhav:** Pichhla sawal khula tha. Vaakya mein bees shabd hain. Ek shabd ki jagah badalni hai. Usse kaise pata chalega ki kin shabdon ki taraf khisakna hai?

**Kabir:** Aas-paas wale? Pichhle do-teen?

**Madhav:** Yeh vaakya lo. "Woh ladki jo kal school se aayi thi, apni kitaab bhool gayi."

**Kabir:** Theek.

**Madhav:** "Bhool gayi" mein "gayi" hai, "gaya" nahi. Woh kis shabd ki wajah se?

**Kabir:** "Ladki" ki wajah se.

**Madhav:** Aur "ladki" kitne shabd peeche hai?

**Kabir:** Aath-nau.

**Madhav:** Toh sirf paas wale dekhna kaam nahi karta.

**Kabir:** Nahi. Toh poora vaakya dekhna padega.

**Madhav:** Achha. Toh har shabd har doosre shabd ko dekhega?

**Kabir:** Haan.

**Madhav:** Barabar dekhega?

**Kabir:** Nahi. "Gayi" ko "ladki" zyada mayne rakhti hai, "kal" kam.

**Madhav:** Toh use ek maatra chahiye. "Yeh shabd mere liye kitna mayne rakhta hai."

**Kabir:** Haan. Ek number, har jodi ke liye.

**Madhav:** Aur woh number kahan se aayega?

**Kabir:** Dono shabdon ki jagah se? Agar woh ek doosre se jude hue hain toh number bada.

**Madhav:** Ab woh number mila. Ab usse karoge kya?

**Kabir:** Jinke number bade hain, unki taraf zyada khisakunga. Jinke chhote, kam.

**Madhav:** Toh nayi jagah kya hui?

**Kabir:** Saare shabdon ka mishran, unke numbers ke hisaab se.

**Madhav:** Bas. Aapne poora mechanism bana diya. Ab do baatein aur. Pehli: kya har shabd ko sirf ek hi tarah ke rishte dekhne chahiye?

**Kabir:** Matlab?

**Madhav:** "Gayi" ko "ladki" vyakaran ke liye chahiye. Aur "bhool gayi" ko "kitaab" chahiye kyunki wahi bhooli gayi. Do alag tarah ke rishte.

**Kabir:** Toh ek hi baar dekhne se dono nahi milenge.

**Madhav:** Toh?

**Kabir:** Kai baar dekho, alag alag tarah se. Ek baar vyakaran ke liye, ek baar kis-kis-ko ke liye.

**Madhav:** Aur kaun tay karega ki kaunsi baar kis cheez ke liye hai?

**Kabir:** Koi nahi. Woh bhi training se nikalna chahiye.

**Madhav:** Bilkul. Aur nikalta bhi hai. Doosri baat: yeh sab ek hi baar karna kaafi hai?

**Kabir:** Shayad nahi. Pehli baar mein "yeh" ko pata chalega ki woh "kitaab" ki baat kar raha hai. Aur uske baad hi doosre shabd us nayi jaankari ko istemaal kar sakte hain.

**Madhav:** Toh?

**Kabir:** Poora kaam dobara karo. Aur dobara.

**Madhav:** Kitni baar?

**Kabir:** Pata nahi. Kai baar.

**Madhav:** Bade models mein sau se zyada baar. Har baar tasveer thodi aur saaf hoti hai.

### Naam

Us poore mechanism ka naam hai **attention**.

Woh teen kadam mein chalta hai:

```
1.  har shabd har doosre shabd ko dekhta hai
2.  har jodi ke liye ek number nikalta hai:
    "yeh shabd mere liye kitna mayne rakhta hai"
3.  har shabd ki nayi jagah banti hai: baaki sab ka mishran,
    un numbers ke wazan ke hisaab se
```

Do cheezein jo Kabir ne khud nikaali, aur dono ke naam hain:

**Kai baar, alag tarah se dekhna.** Har baar ek alag kism ka rishta pakadti hai: kaun kiska kartaa hai, kaunsa vishesan kis pe lagta hai, "yeh" kis cheez ko ishaara kar raha hai. Iska naam **multi-head** hai, aur ek bade model mein aisi bees-tees "aankhein" ek saath chalti hain.

**Poora kaam baar baar dohrana.** Har dohrav ke baad har shabd ki jagah thodi behtar hoti hai, aur agle dohrav mein woh behtar jagah istemaal hoti hai. Har dohrav ko **layer** kehte hain, aur bade models mein sau se zyada layers hoti hain.

Ab do baatein jo iss se seedhi nikalti hain.

**Ek: doori se koi farak nahi padta.**

Yeh sabse bada faayda hai. Ek shabd jo sau shabd peeche hai, woh utna hi paas hai jitna woh jo ek shabd peeche hai. Attention doori nahi dekhti, sirf rishta dekhti hai.

Purane tareeke ek-ek karke aage badhte the, isliye door ki cheezein dheere dheere dhundhli ho jaati thin. Yahan woh problem hai hi nahi.

**Do: iski keemat bhari hai, aur woh doori nahi, ginti se aati hai.**

Har shabd har doosre shabd ko dekhta hai. Toh das shabd mein sau jodiyan. Sau shabd mein das hazaar. Hazaar shabd mein das lakh.

```
shabd      jodiyan
10         100
100        10,000
1,000      10,00,000
10,000     10,00,00,000
```

**Kaam shabdon ke saath seedha nahi, unke varg ke saath badhta hai.** Ise yaad rakhna. Yeh Chapter 4.5 mein context window ki poori wajah hai, aur Chapter 7.1 mein daam ki.

### Asli duniya se

2017 mein ek paper aaya jiska naam tha "Attention Is All You Need."

Us waqt bhasha ke models ek-ek shabd karke aage badhte the. Woh dheema tha, kyunki har shabd ko pichhle ka intezaar karna padta tha, aur door ki cheezein bhooli jaati thin.

Us paper ne kaha: woh ek-ek karke aage badhna hata do. Sirf attention rakho.

Do cheezein ek saath mili:

**Ek:** door ki cheezein utni hi saaf rahin jitni paas ki.

**Do,** aur yeh shayad zyada bada tha: **ab poora vaakya ek saath sambhala ja sakta tha.** Jab har shabd ko pichhle ka intezaar nahi karna, toh saara kaam ek saath ho sakta hai. Aur GPU wahi cheez karte hain: hazaaron hisaab ek saath. *(Book 1, Ch 2.4 wali baat: AI ko alag chip kyun chahiye)*

Toh yeh design GPU ke liye bilkul fit tha, aur usi ne training ko itna bada hone diya.

**Idea ke saath saath, us idea ka machine ke saath fit hona bhi utna hi mayne rakhta tha.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **"attention" ko insaani dhyaan samajhna.**

Naam bhraamak hai. Isme koi chun nahi raha ki kis pe dhyaan dena hai. Har shabd har doosre shabd ko dekhta hai, hamesha, poori tarah yaantrik roop se. Bas kuch ko zyada wazan milta hai.

Woh wazan bhi kisi ne tay nahi kiye. Woh us hisaab se nikalte hain jo training ne banaya.

Doosri galti: **yeh sochna ki har layer mein koi alag "kaam" hota hai.**

Log kehte hain ki pehli layers vyakaran dekhti hain aur upar wali matlab. Isme kuch sachai hai aur woh utna saaf nahi hai jitna kaha jaata hai. Kisi ne yeh baanta nahi. Log baad mein andar jhaank kar patterns dhoondhte hain, aur woh patterns kabhi kabhi milte hain aur kabhi nahi.

**Yeh un jagahon mein se ek hai jahan hum yeh jaante hain ki cheez kaam kaise karti hai, aur yeh nahi jaante ki woh kya kar rahi hai.**

### Sochne ke liye

**1. (samajh check)** Aap ek chhoti si baat ko poochte ho aur woh sasta hai. Phir aap ek poora document daal kar wahi baat poochte ho aur woh bahut mehnga ho jaata hai. Kyun?

> **Jawab:** Kyunki attention ka kaam shabdon ke varg ke saath badhta hai, seedhe anupaat mein nahi.
>
> Das guna zyada text daalne se kaam das guna nahi, lagbhag sau guna badhta hai.
>
> Isliye "poora document daal do, model dekh lega" ek mehnga vaakya hai. Aur isliye Chapter 6.2 ka poora tareeka maujood hai: **poora document mat bhejo, sirf zaroori tukda bhejo.**

**2. (samajh check)** Purane models door ki baat bhool jaate the, naye nahi. Kya badla?

> **Jawab:** Purane ek-ek shabd karke aage badhte the, isliye jaankari ko poore raaste se guzarna padta tha aur woh raaste mein ghis jaati thi.
>
> Attention mein har shabd seedha har doosre shabd ko dekhta hai. Sau shabd peeche wali cheez utni hi paas hai jitni ek shabd peeche wali.
>
> Toh doori ki problem khatam hui, aur uski jagah ek nayi problem aayi: ginti ki. Ab seema yeh nahi hai ki cheez kitni door hai, seema yeh hai ki kul kitni hai.
>
> **Purani seema hati, nayi bani.** Book 1 Ch 6.2 wali baat: har hal apne saath ek nayi kamzori laata hai.

**3. (jodne wala)** Book 1 Ch 6.7 mein N+1 problem thi: sau chhote sawal ek bade sawal ki jagah. Kya attention mein wahi shakal hai?

> **Jawab:** Ulti shakal hai, aur woh dilchasp hai.
>
> N+1 mein problem yeh thi ki sau alag chakkar lagte the, ek ke baad ek, aur har chakkar mein intezaar tha.
>
> Attention mein saari jodiyan **ek saath** nikalti hain. Koi kisi ka intezaar nahi karta.
>
> Isiliye woh GPU pe itni achhi chalti hai, aur isiliye woh ek-ek karke chalne wale purane tareekon se jeet gayi.
>
> **Kaam zyada hai, aur woh ek saath ho sakta hai. Yeh aksar kam kaam se behtar sauda hota hai jo ek ke baad ek karna pade.**
