# Chapter 1.6  [DEPTH]
## Tokens bante kaise hain

*DEPTH chapter. Pehli baar mein chhod sakte ho. Lekin iske baad "kaunse shabd sasta hain" ka jawab andar se dikhta hai.*

### Samvaad

**Madhav:** Pichhle chapter mein tumne kaha ki tukde woh hon jo aksar aate hain. Ab batao ki yeh tay kaun karega.

**Kabir:** Koi insaan list bana de.

**Madhav:** Kitni bhashaon ke liye? Aur code, naam, emoji?

**Kabir:** Bahut kaam hai. Aur galtiyan hongi.

**Madhav:** Toh machine ko kaise batayenge? Uske paas sirf bahut saara text hai.

**Kabir:** Woh khud dekh le ki kya aksar aata hai.

**Madhav:** Kaise shuru karega? Uske paas toh koi shabd hi nahi hain.

**Kabir:** Sabse chhoti cheez se. Akshar.

**Madhav:** Theek. Toh shuruaat mein har akshar ek token hai. Ab aage?

**Kabir:** Ab dekhe ki kaunse do akshar sabse zyada baar ek saath aate hain.

**Madhav:** Angrezi mein woh kya hoga?

**Kabir:** Shayad "th". Ya "he".

**Madhav:** Maan lo "th". Ab kya karein?

**Kabir:** Use ek naya token bana do. Ab "th" ek cheez hai.

**Madhav:** Aur phir?

**Kabir:** Phir dobara dekho. Ab shayad "th" aur "e" sabse zyada saath aayenge.

**Madhav:** Toh "the" ban gaya. Aur phir?

**Kabir:** Dobara. Aur dobara. Jab tak kaafi tokens na ban jaayein.

**Madhav:** Kitne?

**Kabir:** Pata nahi. Kuch hazaar?

**Madhav:** Aam taur pe 50,000 se 2,00,000 ke beech. Ab batao ki agar aap 1,000 pe ruk jao toh kya hoga?

**Kabir:** Tokens chhote rahenge. Har shabd kai tokens lega. Sab dheema aur mehnga ho jaayega.

**Madhav:** Aur agar aap 10 lakh tak jao?

**Kabir:** Har shabd ek token mein aa jaayega. Tez hoga.

**Madhav:** Aur nuksaan?

**Kabir:** Model ko har token ke liye kuch rakhna padta hoga. Das lakh bahut zyada ho jaayega.

**Madhav:** Bilkul. Har token ke liye model ke andar ek poori line rakhi hoti hai. Das lakh tokens matlab das lakh lines. Toh yeh ek sauda hai.

**Kabir:** Kam tokens: chhota model, dheemi baat. Zyada tokens: bada model, tez baat.

**Madhav:** Ab aakhri, aur yeh sabse zaroori hai. Yeh ginti kis text pe ki gayi thi?

**Kabir:** Jo bhi text unhone liya tha.

**Madhav:** Aur agar us text mein 90 percent angrezi thi?

**Kabir:** Toh angrezi ke bade tukde banenge. Baaki bhashaon ke nahi.

**Madhav:** Toh hindi mehngi kyun hai?

**Kabir:** Kyunki jab yeh list banayi ja rahi thi, tab hindi kam thi. Uske tukde bade ban hi nahi paaye.

**Madhav:** Aur woh faisla ab tay ho chuka hai. Model bana, list uske andar hai, aur woh badal nahi sakti.

### Naam

Us tareeke ka naam hai **BPE**, yaani baar baar sabse aam jodi ko milaate jaana.

```
shuruaat   har akshar ek token
dohrao     sabse zyada saath aane wali jodi ko mila do
ruk jao    jab tay ki gayi ginti tak pahunch jao
```

Ek chhota udaharan, angrezi jaise text pe:

```
kadam 0   l o w   l o w e r   n e w e s t
kadam 1   "e"+"s" sabse aam  →  "es"
kadam 2   "es"+"t"           →  "est"
kadam 3   "l"+"o"            →  "lo"
kadam 4   "lo"+"w"           →  "low"

ab "low" ek token hai, "est" ek token hai
"lowest" do tokens mein likha jaayega
```

Aur teen nateeje, jo Kabir ne khud nikaale:

```
1.  LIST KA SIZE EK SAUDA HAI
    chhoti list  →  chhota model, zyada tokens, mehngi baat
    badi list    →  bada model, kam tokens, sasti baat

2.  JO TEXT ZYADA THA, USKI BHASHA SASTI HAI
    yeh nyaay nahi hai, yeh ginti hai

3.  YEH FAISLA MODEL BANNE SE PEHLE HOTA HAI
    aur uske baad kabhi badalta nahi
```

Teesri baat dhyaan dene laayak hai. Tokenisation model ki training se **pehle** tay hoti hai. Woh uska sabse pehla faisla hai, aur uske baad poora model us list pe khada ho jaata hai. Use badalne ka matlab hai poora model dobara banana.

### Asli duniya se

Jab GPT ke shuruaati versions aaye, unki token list mein angrezi ka bhaari daabdaba tha. Ek angrezi shabd aksar ek token leta tha. Kuch bhashaon mein, jinki likhawat alag hai, wahi ek shabd chaar se dus token le leta tha.

Iska matlab teen alag nuksaan the, ek saath:

```
mehnga    wahi baat karne ka daam kai guna
chhota    utne hi context mein bahut kam baat aati thi
kamzor    us bhasha ka data bhi kam tha, toh jawab bhi kamzor
```

Naye models mein yeh farak kaafi kam hua hai, kyunki list banate waqt jaan-boojh ke zyada bhashaayein daali gayin.

Lekin farak khatam nahi hua, aur woh poori tarah kabhi hoga bhi nahi, kyunki internet pe likhawat khud barabar nahi bant ti. **Token list us duniya ka aaina hai jismein woh banayi gayi thi.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki tokenisation ek chhoti technical baat hai.**

Woh model ka pehla faisla hai aur uska asar har cheez pe padta hai: daam, speed, kaunsi bhasha sasti hai, aur kuch kaam mumkin hain ya nahi.

Ek udaharan jo dikhta hai: numbers. Agar "1234" ek token hai aur "1235" doosra, toh model ke liye woh do alag cheezein hain, jinka koi rishta nahi. Uske liye unke beech woh sambandh nahi hai jo aapke liye hai.

Isiliye bade numbers ka hisaab in models ke liye mushkil raha hai. Woh sirf "ganit mushkil hai" nahi tha. Woh aankh ki seema thi, phir se.

Naye models mein numbers ko ek-ek ank karke toda jaata hai, jaan-boojh ke, sirf isliye ki hisaab behtar ho.

**Ek chhota faisla, jo model banne se pehle liya gaya, aur uska asar uski poori zindagi rehta hai.**

### Sochne ke liye

**1. (samajh check)** Aap ek aisa model chahte ho jo sirf code likhe. Uski token list kaisi honi chahiye?

> **Jawab:** Usmein code ke aam tukde bade tokens hone chahiye: `function`, `return`, `<div>`, `==`, aur woh spaces jo indentation banate hain.
>
> Aur aam angrezi ke tukdon ki utni zaroorat nahi hai.
>
> Isse code sasta aur tez ho jaayega, aur utne hi context mein zyada code aayega.
>
> Isiliye kuch code wale models ki apni alag token list hoti hai. **List us kaam ke liye banayi jaati hai jo model karega.**

**2. (samajh check)** Ek naya shabd banta hai jo model banne ke baad aaya. Kya model use likh sakta hai?

> **Jawab:** Haan, hamesha. Woh chhote tukdon mein toot jaayega, aur zaroorat pade toh akshar-akshar.
>
> Yeh BPE ki sabse achhi baat hai: woh kabhi fail nahi hota. Koi bhi text likha ja sakta hai.
>
> Lekin woh mehnga hoga (zyada tokens), aur model use theek se samajhta nahi hoga, kyunki us shabd ko usne kabhi dekha hi nahi.
>
> **Likh paana aur samajh paana do alag baatein hain.** Yeh farak aage kai jagah kaam aayega.

**3. (jodne wala)** Book 1 Ch 2.1 mein compression thi, jo dohrav hatati thi. BPE usse kaise milta hai?

> **Jawab:** Woh lagbhag wahi soch hai.
>
> Compression kehti hai: jo cheez baar baar aati hai use ek chhote nishaan se badal do.
>
> BPE kehta hai: jo tukda baar baar aata hai use ek token bana do.
>
> Dono dohrav pe chalte hain, aur dono wahan bekaar ho jaate hain jahan dohrav nahi hai. Isiliye ek ajeeb, kabhi na dikha hua shabd bahut tokens leta hai, bilkul waise jaise ek bina pattern wali photo compress nahi hoti.
>
> Ek hi shakal, do jagah. Book 1 ki tarah, yeh kitaab bhi unhi das shakalon pe khadi hai.
