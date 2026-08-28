# Chapter 2.5  [DEPTH]
## Sahi direction mein badalna

*DEPTH chapter. Yeh training ka aakhri mechanism hai. Iske baad Part 2 ka baaki hissa data ke baare mein hai, machine ke nahi.*

### Samvaad

**Madhav:** Loss ek number hai aur use girana hai. Ab batao ki 70 arab numbers mein se kaunsa hilaana hai.

**Kabir:** Pata nahi. Sabko thoda thoda?

**Madhav:** Kis disha mein? Har number ya toh badhaya ja sakta hai ya ghataya.

**Kabir:** Try karke dekh lo? Ek badhao, loss dekho.

**Madhav:** Achha. Ek number badhaya, loss nikala. Kitna kaam laga?

**Kabir:** Poora model ek baar chalana pada.

**Madhav:** Ab 70 arab numbers ke liye?

**Kabir:** 70 arab baar model chalana padega. Har ek badlav ke liye.

**Madhav:** Aur yeh ek example ke liye. Kharabon examples hain.

**Kabir:** Yeh kabhi khatam hi nahi hoga.

**Madhav:** Toh yeh raasta band hai. Ab dooosra socho. Aap ek pahaadi pe khade ho, andhera hai, aur aapko neeche jaana hai. Kya karoge?

**Kabir:** Paaon se dekhunga ki dhalaan kis taraf hai. Us taraf ek kadam.

**Madhav:** Aapko poori pahaadi ka naksha chahiye?

**Kabir:** Nahi. Sirf yahan ka dhalaan.

**Madhav:** Aur phir?

**Kabir:** Phir wahan se dobara. Aur dobara.

**Madhav:** Ab isse model pe lagao. "Dhalaan" ka matlab kya hoga?

**Kabir:** Ki agar main iss number ko thoda badhaun, toh loss badhega ya ghatega, aur kitna.

**Madhav:** Aur woh kaise pata chalega bina 70 arab baar chalaye?

**Kabir:** Wahi toh problem hai.

**Madhav:** Ab main aapko woh cheez batata hoon jisne yeh sab mumkin banaya. Ek chhota udaharan lo. Aapke paas teen numbers hain, ek ke baad ek lage hue. Pehla doosre pe asar daalta hai, doosra teesre pe, aur teesre se jawab nikalta hai.

**Kabir:** Theek.

**Madhav:** Ab jawab galat aaya. Kya aap bata sakte ho ki teesre number ne kitni galti ki?

**Kabir:** Haan, woh toh ekdum jawab ke paas hai.

**Madhav:** Aur doosre ne?

**Kabir:** Woh teesre ke through gaya. Toh agar mujhe pata hai ki teesre ne kitni galti ki, aur yeh bhi ki doosra teesre pe kitna asar daalta hai, toh main nikaal sakta hoon.

**Madhav:** Aur pehla?

**Kabir:** Usi tarah, doosre se peeche jaakar.

**Madhav:** Toh aapne kya kiya? Kitni baar hisaab lagana pada?

**Kabir:** Ek baar aage, ek baar peeche. Bas.

**Madhav:** 70 arab baar nahi?

**Kabir:** Nahi. Ek baar peeche chalne mein sabka dhalaan mil gaya.

**Madhav:** **Yehi woh cheez hai jisne yeh poora field mumkin banaya.** Ek baar aage jaakar jawab nikalo, ek baar peeche aakar sabki zimmedari nikalo.

### Naam

Us "dhalaan pe ek kadam" ka naam hai **gradient descent**.

Aur us "ek baar peeche jaakar sabki zimmedari nikalna" ka naam hai **backpropagation**.

Poora chakkar:

```
1.  aage:    ek example daalo, jawab nikalo
2.  naapo:   loss nikalo (Chapter 2.4)
3.  peeche:  ek baar peeche chal kar har number ka dhalaan nikalo
4.  hilao:   har number ko dhalaan ke ulti taraf ek chhota kadam
5.  dohrao:  kharabon baar
```

Aur do cheezein jo iss mein tay karni padti hain:

**Kadam ka size.** Bahut bada kadam toh aap manzil ke upar se kood jaoge aur cheez bikhar jaayegi. Bahut chhota toh saal lag jaayenge. Iska naam **learning rate** hai, aur woh training ka sabse tedha faisla hai.

**Kitne examples ek saath.** Ek example ka dhalaan shor bhara hota hai. Isliye kuch sau ya hazaar ek saath liye jaate hain aur unka average dhalaan istemaal hota hai. Iska naam **batch** hai.

Ab ek baat jo dhyaan dene laayak hai. Yeh tareeka yeh guarantee nahi karta ki aap sabse neeche pahunchoge. Andhere mein dhalaan pe chalte hue aap ek chhote gaddhe mein bhi ruk sakte ho.

Aur phir bhi yeh kaam karta hai, bahut bade models pe. **Kyun kaam karta hai, iska poora jawab kisi ke paas nahi hai.** Yeh un jagahon mein se ek hai jahan practice theory se aage nikal gayi hai.

### Asli duniya se

Backpropagation ka idea 1970 aur 1980 ke dashak mein aa chuka tha. Woh naya nahi hai.

Uske baad lagbhag tees saal tak yeh field lagbhag thanda pada raha. Log ise "AI winter" kehte hain.

Kya badla? Teen cheezein, aur teeno idea ke bahar thin:

```
DATA        internet ne kharabon examples muft mein de diye (Ch 2.2)
MACHINE     GPU aa gaye, jo ek saath hazaaron hisaab karte hain
            (Book 1 ne bataya tha ki AI ko alag chip kyun chahiye)
PAISA       kisi ne itna kharch karne ka faisla kiya
```

Yeh Book 1 ka sabse bada dohrav hai: **idea pehle se tha. Paimana baad mein aaya.**

Aur yeh aage ke liye ek kaam ka sabak hai. Jab koi kahe ki "yeh nayi khoj hai," toh aksar khoj purani hoti hai aur naya yeh hota hai ki woh ab sasti ho gayi.

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki training mein koi samajhdaari hai.**

Kahin koi cheez yeh nahi soch rahi ki "yeh number badhana chahiye kyunki Dilli rajdhani hai."

Sirf yeh ho raha hai: ek number hai (loss), har weight ka uspe ek dhalaan hai, aur har weight ko dhalaan ke ulte thoda hilaya jaata hai. Kharabon baar.

Yeh poori tarah yaantrik hai. Usmein koi soch nahi hai, koi lakshya nahi hai siwaay ek number ko girane ke.

Doosri galti: **yeh sochna ki training ke baad model "jaanta" hai.**

Jo bacha hai woh 70 arab numbers hain jo aise sthir hue ki loss kam ho. Bas.

Ki us se "jaanna" jaisa vyavhaar nikal aata hai, yeh sach hai aur woh ajeeb hai, aur woh iss kitaab ka sabse imaandaar khula sawal hai.

### Sochne ke liye

**1. (samajh check)** Learning rate bahut bada rakh diya jaaye toh kya hoga?

> **Jawab:** Loss girne ki jagah upar-neeche uchhalne lagega, aur aksar poori cheez bikhar jaayegi.
>
> Pahaadi wale udaharan mein: aap dhalaan dekh kar itna bada kadam maar rahe ho ki aap ghaati ke paar wali pahaadi pe pahunch jaate ho, phir wapas, har baar pehle se upar.
>
> Aur bahut chhota rakh do toh training itni dheemi ho jaayegi ki woh kabhi khatam nahi hogi.
>
> **Yeh sirf ek number hai aur woh karodon dollar ki training bana ya bigaad sakta hai.**

**2. (samajh check)** Backpropagation ke bina kitna kaam lagta? Uske saath kitna?

> **Jawab:** Bina: har weight ke liye poora model dobara chalana. 70 arab weights matlab 70 arab baar, har example pe.
>
> Saath: ek baar aage, ek baar peeche. Yaani lagbhag do baar, har example pe.
>
> Farak lagbhag 35 arab guna hai.
>
> Isiliye yeh sirf ek "optimisation" nahi hai. **Uske bina yeh cheez mumkin hi nahi hai**, kisi bhi paimane pe.

**3. (jodne wala)** Book 1 Ch 5.2 mein index tha, jo das crore mein se ek cheez sattaais kadam mein dhoondh leta tha. Kya yahan wahi shakal hai?

> **Jawab:** Haan, aur woh shakal poori kitaab mein sabse zyada dikhti hai.
>
> Dono jagah: ek aisa kaam jo seedha karne pe data ke saath badhta hai, aur ek chalaki jo use lagbhag sthir kar deti hai.
>
> ```
> dhoondhna    seedha: 5 crore kadam    index se: 27 kadam
> dhalaan      seedha: 70 arab baar     backprop se: 2 baar
> ```
>
> Aur dono mein woh chalaki dhaanche se aati hai, taakat se nahi. Koi badi machine yeh farak nahi de sakti.
>
> **Jab bhi kuch namumkin lage, sawal yeh nahi hai ki machine kitni badi ho. Sawal yeh hai ki kaam ka dhaancha badla ja sakta hai ya nahi.**
