# Chapter 2.2  [SPINE]
## Galat hokar seekhna

### Samvaad

**Madhav:** Examples se seekhna, theek. Lekin "seekhna" ka matlab kya hai, jab andar sirf numbers hain?

**Kabir:** Numbers badalte honge.

**Madhav:** Kis disha mein?

**Kabir:** Us disha mein jo sahi ho.

**Madhav:** Machine ko kaise pata ki kaunsi disha sahi hai?

**Kabir:** Hmm.

**Madhav:** Ek chhoti cheez se shuru karte hain. Aap ek nishaana lagate ho aur teer daayein chala jaata hai. Ab kya karoge?

**Kabir:** Thoda baayein karke phir maarunga.

**Madhav:** Kitna baayein?

**Kabir:** Jitna daayein gaya tha, uske hisaab se. Bahut door gaya toh zyada, thoda gaya toh thoda.

**Madhav:** Ab dhyaan do ki aapko kya kya chahiye tha. Ginao.

**Kabir:** Mujhe pata hona chahiye ki nishaana kahan tha. Mujhe pata hona chahiye ki teer kahan gaya. Aur donon ke beech ka farak.

**Madhav:** Aur teesri cheez?

**Kabir:** Ki farak kam karne ke liye mujhe kya badalna hai.

**Madhav:** Bas. Yeh chaar cheezein hi poora seekhna hain. Ab isse machine pe lagao. Ek model hai jo agla token guess karta hai. Use ek vaakya dikhaya jaata hai: "Bharat ki rajdhani hai ___". Woh kya karega?

**Kabir:** Woh guess karega.

**Madhav:** Maan lo woh "Mumbai" guess karta hai. Ab sahi jawab kahan se aayega?

**Kabir:** Text mein pehle se hai. Asli vaakya mein "Dilli" likha tha.

**Madhav:** Toh kisi insaan ko batana pada?

**Kabir:** Nahi! Jawab text mein hi tha. Bas woh chhupa diya gaya tha.

**Madhav:** Ab yeh baat dhyaan se dekho, kyunki yeh sabse chalak hissa hai. Aapko kitne examples chahiye honge?

**Kabir:** Bahut.

**Madhav:** Aur unhe kisi ko banana padega?

**Kabir:** Nahi. Har likha hua vaakya apne aap ek example hai. Aap uska aakhri hissa chhupa do, aur jawab pehle se maujood hai.

**Madhav:** Toh duniya mein kitne examples hain?

**Kabir:** Jitna kuch bhi kabhi likha gaya. Sab.

**Madhav:** Aur unke liye kisi ne mehnat ki?

**Kabir:** Nahi. Woh pehle se pade hain.

**Madhav:** **Isi ek chaalaki ne yeh sab mumkin banaya.** Agar har example ke liye kisi insaan ko jawab likhna padta, toh yeh kabhi nahi hota. Ab aage. Model ne "Mumbai" kaha, sahi tha "Dilli". Ab kya?

**Kabir:** Numbers thoda badlo, us disha mein jismein agli baar "Dilli" ki sambhavna zyada ho.

**Madhav:** Kitne numbers hain?

**Kabir:** Arbon.

**Madhav:** Kaunsa badalna hai?

**Kabir:** Sab? Thoda thoda?

**Madhav:** Aur kitna thoda?

**Kabir:** Uske hisaab se ki woh number galti ke liye kitna zimmedar tha.

**Madhav:** Aur woh kaise pata chalega?

**Kabir:** Yeh mushkil hai.

**Madhav:** Woh mushkil hai aur uska hal hai, aur woh do DEPTH chapters hain. Abhi bas yeh pakdo: **galti naapo, sabko thoda thoda us disha mein hilao jismein galti kam ho, aur yeh arbon baar dohrao.**

### Naam

Poora tareeka, paanch kadam mein:

```
1.  ek asli text ka tukda lo
2.  uska agla token chhupa do
3.  model se guess karwao
4.  guess aur asli jawab ka farak naapo
5.  saare numbers thoda hilao taaki woh farak kam ho
    ── aur yeh arbon baar dohrao
```

Iska naam hai **training**.

Do baatein jo iski jaan hain:

**Ek: jawab data mein pehle se hota hai.** Kisi insaan ko har example ka jawab nahi likhna padta. Aap text ka ek hissa chhupate ho aur jawab baaki text mein pada hai. Isliye internet ka har page ek training example hai, bina kisi mehnat ke.

Isi wajah se yeh cheez itni badi ho payi. Jo cheezein insaan ko haath se label karni padti hain, unka paimana hamesha chhota rehta hai.

**Do: seekhna aur istemaal karna do alag waqt hain.**

```
TRAINING       mahinon chalti hai, hazaaron machinon pe
               numbers badalte hain
               bahut mehngi: karodon dollar

ISTEMAAL       har sawal pe, kuch second
               numbers bilkul nahi badalte
               sasti: paise ke chhote hisse
```

Aur isiliye Chapter 1.2 wali baat sach hai: aapse baat karke model behtar nahi hota. Woh us waqt seekh hi nahi raha. Seekhna khatam ho chuka hai, aur ab bas woh file istemaal ho rahi hai.

### Asli duniya se

Ek bade model ki training mein aaj mahine lagte hain, hazaaron khaas chips ek saath chalti hain, aur kharcha karodon dollar tak jaata hai. Bijli itni lagti hai ki jagah chunne mein bijli ka daam ek badi wajah hoti hai.

Uske baad wahi model karodon logon ke sawalon ka jawab deta hai, aur ek sawal ka kharcha ek rupaye ke chhote hisse jitna hota hai.

Ab Book 1 Chapter 0.2 ke dials lagao.

Training Anil ki naali hai: ek baar, bahut mehngi, aur uske baad woh chalti rehti hai. Har sawal ka jawab us ek baar ki mehnat se aata hai.

Aur yahi wajah hai ki yeh karobaar aise dikhta hai jaise dikhta hai: **bahut bada shuruaati kharcha, aur uske baad lagbhag zero.** Woh dhaancha kis tarah ka karobaar banata hai, yeh Chapter 7.1 ka vishay hai.

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki model aapse baat karke seekh raha hai.**

Woh nahi seekh raha. Uski file badal hi nahi rahi.

Do cheezein hain jo aisa lagne deti hain, aur dono alag hain:

```
usi chat mein woh yaad rakhta lagta hai
   →  purani baat har baar dobara bheji ja rahi hai (Ch 1.2)

aapki baat se AGLA model behtar ban sakta hai
   →  company aapki baat-cheet rakh kar use agli training
       mein daal sakti hai. Woh model badal jaata hai, yeh nahi.
```

Doosri galti: **yeh sochna ki training aur istemaal ka kharcha ek jaisa hai.**

Woh crore guna alag hain. Aur isse ek karobaari baat nikalti hai: bahut kam log model bana sakte hain, aur lagbhag koi bhi use istemaal kar sakta hai.

**Scarcity training mein hai, istemaal mein nahi.** Book 1 Chapter 6.9 ke hisaab se yeh batata hai ki paisa kahan rukega.

### Sochne ke liye

**1. (samajh check)** Training ke liye kisi insaan ko jawab nahi likhne padte. Iska sabse bada nateeja kya hai?

> **Jawab:** Ki examples ki ginti par koi seema nahi rahi.
>
> Agar har example ke liye ek insaan ko baithna padta, toh shayad lakhon examples milte. Bina uske, kharabon mil gaye.
>
> Aur ML mein data ki ginti seedha nateeje pe asar daalti hai.
>
> Isiliye jo kaam iss chaalaki se ho jaate hain, woh tez aage badhe hain, aur jinke liye insaan ko label karna padta hai, woh peeche reh gaye. **Jo cheez muft mein mil sakti hai, wahi paimane pe pahunchti hai.**

**2. (samajh check)** Ek company kehti hai "hamara model aapke istemaal se roz behtar hota hai." Kya yeh mumkin hai?

> **Jawab:** Do matlab ho sakte hain, aur farak zaroori hai.
>
> **Woh model jo abhi aapse baat kar raha hai:** nahi. Uski file sthir hai.
>
> **Woh cheez jo unka product hai:** haan. Woh aapki baat-cheet ikattha kar sakte hain, use jaanch sakte hain, aur agli training mein daal sakte hain. Kuch mahine baad naya model aata hai jo behtar hai.
>
> Toh vaakya galat nahi hai, lekin uska matlab yeh hai ki **aapki baat kahin rakhi ja rahi hai.** Yeh Chapter 6.6 ka vishay hai.

**3. (jodne wala)** Book 1 Ch 0.2 mein leverage tha: ek baar kaam karo, baar baar milta rahe. Training us baat ka kaunsa roop hai?

> **Jawab:** Woh uska sabse teekha roop hai jo iss kitaab mein aayega.
>
> Ek baar, mahinon, karodon dollar. Uske baad karodon log use roz istemaal karte hain, aur har istemaal ka kharcha lagbhag kuch nahi.
>
> Anil ki naali, lekin ek aisi naali jiske paani ki koi seema nahi hai.
>
> Aur isiliye yeh ek aise thode logon ka khel hai jo woh shuruaati kharcha utha sakein. Yeh Chapter 7.1 aur 7.3 mein poora khulega.
