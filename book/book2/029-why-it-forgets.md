# Chapter 4.4  [SPINE]
## Yeh bhool kyun jaata hai

### Samvaad

**Madhav:** Ek lambi baat-cheet mein woh shuruaat bhool jaata hai. Ab aap wajah bata sakte ho?

**Kabir:** Usmein yaaddasht hai hi nahi. Har baar poori baat dobara bheji jaati hai. Chapter 1.2.

**Madhav:** Toh bhoolna kya hai?

**Kabir:** Woh dobara bheji hi nahi ja rahi.

**Madhav:** Kyun nahi?

**Kabir:** Kyunki woh bahut lambi ho gayi.

**Madhav:** Ek seema hai. Kyun hai?

**Kabir:** Attention ka kaam varg mein badhta hai. Chapter 3.3.

**Madhav:** Aur?

**Kabir:** Aur bacha hua kaam memory mein rehta hai. Chapter 4.1. Woh bhi badhta jaata hai.

**Madhav:** Toh do alag seemayein hain. Ek hisaab ki, ek memory ki. Ab batao ki jab seema aa jaaye toh kya kiya jaaye.

**Kabir:** Shuruaat kaat do.

**Madhav:** Aur us mein kya tha?

**Kabir:** Shayad woh sab jo maine shuru mein bataya tha. Mera kaam, meri shartein.

**Madhav:** Toh sabse zaroori cheez sabse pehle kati.

**Kabir:** Haan. Yeh bura hai.

**Madhav:** Doosra tareeka socho.

**Kabir:** Purani baat ka saaransh bana lo. Poori mat bhejo, nichod bhejo.

**Madhav:** Aur uska nuksaan?

**Kabir:** Saaransh mein kuch chala jaayega. Aur pata nahi chalega ki kya gaya.

**Madhav:** Aur teesra?

**Kabir:** Sirf woh hissa bhejo jo iss sawal ke liye kaam ka hai.

**Madhav:** Kaise pata chalega ki kaunsa kaam ka hai?

**Kabir:** Sawal se milta-julta dhoondho. Embedding se. Chapter 3.1.

**Madhav:** Aapne abhi woh cheez bana di jo Chapter 6.2 hai. Abhi ek aakhri baat. Bade context ka daawa aajkal khoob hota hai: das lakh tokens, aur zyada. Kya usse yeh problem khatam ho gayi?

**Kabir:** Lagta toh hai.

**Madhav:** Do wajahon se nahi. Pehli aap bata sakte ho.

**Kabir:** Daam. Aur waqt. Das lakh tokens bhejne ka matlab hai bada prefill, har baar.

**Madhav:** Aur doosri: agar aap das lakh tokens bhejte ho, toh kya model un sabko barabar dekhta hai?

**Kabir:** Attention toh sabko dekhti hai.

**Madhav:** Dekhti hai. Aur asli mein, bade context mein beech ka hissa aksar dab jaata hai. Shuruaat aur aakhir zyada asar daalte hain.

**Kabir:** Toh cheez andar hai lekin istemaal nahi ho rahi.

**Madhav:** Aur woh sabse khatarnak haalat hai, kyunki aapko lagta hai ki aapne bhej diya, toh kaam ho gaya.

### Naam

Woh kul seema, jitna text ek baar mein diya ja sakta hai, use **context window** kehte hain. Usmein aapka sawal, purani baat, aur jawab, sab ginate hain.

Do wajahein jinse seema aati hai:

```
HISAAB    attention ka kaam tokens ke VARG mein badhta hai  (3.3)
MEMORY    bacha hua kaam (KV cache) memory mein rehta hai   (4.1)
```

Aur seema aane pe teen tareeke, teeno mein kuch khota hai:

```
KAAT DO         purana hissa hata do
                sasta, aur sabse zaroori cheez aksar sabse pehle jaati hai

SAARANSH BANAO  purani baat ka nichod rakho
                behtar, lekin nichodne mein kya gaya woh pata nahi

CHUN KE BHEJO   sirf woh hissa jo iss sawal ke kaam ka hai
                sabse achha, aur sabse mushkil (Chapter 6.2)
```

Ab do baatein jo log lagbhag hamesha nazarandaaz karte hain.

**Ek: bada context muft nahi hai.**

Woh do tarah se mehnga hai: prefill ka waqt (Chapter 4.2) aur input tokens ka daam. Ek das lakh token ka sawal har baar poora padha jaata hai.

**Do: context mein hona aur istemaal hona alag baatein hain.**

Bade context mein beech ka hissa aksar kam asar daalta hai. Iska ek naam bhi pad gaya hai: **lost in the middle**.

Toh yeh maan lena ki "maine document bhej diya isliye usne padh liya" galat hai. Aur woh galti chup-chaap hoti hai: jawab theek dikhta hai, aur woh us hisse pe khada nahi hota jo aapko lagta tha.

**Isliye zaroori cheez shuruaat mein ya aakhir mein rakhna ek asli, kaam ka tareeka hai.**

### Asli duniya se

Context ki seema teen saal mein bahut tezi se badhi hai: kuch hazaar tokens se lakhon tak.

Aur uske saath log ki aadat badal gayi: pehle sab kuch chhota rakhna padta tha, ab log poori file, poori kitaab, poora codebase daal dete hain.

Woh kaam karta hai, aur uske teen chhupe hue daam hain:

```
paisa    har baar poora prefill
waqt     pehla shabd der se
dhyaan   beech ka hissa dab jaata hai
```

Aur isiliye bade systems aaj bhi chun kar bhejte hain, chahe unke paas bada context ho. Woh isliye nahi ki woh nahi bhej sakte. Woh isliye ki chun kar bhejna sasta, tez aur zyada bharosemand hai.

**Bada context ek suvidha hai, ek hal nahi.**

### Yahan log kya galat samajhte hain

Sabse aam galti: **context ko yaaddasht samajhna.**

Woh yaaddasht nahi hai. Woh har baar dobara bheja jaane wala text hai. Kuch bhi "yaad" nahi rehta.

Iska seedha nateeja: log samajh nahi paate ki wahi cheez ek chat mein kaam karti hai aur nayi chat mein nahi. Ya ki lambi chat mehngi kyun hoti jaati hai.

Doosri galti: **yeh sochna ki bada context ka matlab behtar jawab.**

Aksar ulta hota hai. Zyada text bhejne se model ka dhyaan bat jaata hai, aur kaam ki cheez shor mein doob jaati hai.

Ek chhota, chuna hua sandarbh aksar ek bade, sab kuch daal do wale sandarbh se behtar jawab deta hai.

**Yeh Book 1 ka wahi sabak hai: zyada data laana mehnga hai, aur sahi data laana asli kaam hai.**

### Sochne ke liye

**1. (samajh check)** Aap ek lambi chat mein kaam kar rahe ho aur jawab dheere dheere kharaab hote ja rahe hain. Teen wajahein batao.

> **Jawab:**
>
> **Ek:** shuruaat kat gayi. Aapke shuruaati nirdesh ab bheje hi nahi ja rahe.
>
> **Do:** context bhar gaya hai aur zaroori cheez beech mein dab gayi hai.
>
> **Teen:** purani baat naye shabdon ka matlab kheench rahi hai (Chapter 3.2). Aap code ki baat kar rahe the aur ab "model" ka matlab wahin se aa raha hai.
>
> Teeno ka ek hi ilaaj hai aur woh saada hai: **nayi chat shuru karo, aur sirf zaroori cheez dobara likho.**

**2. (samajh check)** Aap ek 500 page ki kitaab context mein daal kar ek sawal poochte ho. Kya problem ho sakti hai?

> **Jawab:** Teen.
>
> **Paisa:** poori kitaab har sawal pe padhi jaayegi.
>
> **Waqt:** pehla shabd bahut der se aayega.
>
> **Bharosa:** jawab jis panne pe hona chahiye tha, woh beech mein dab sakta hai.
>
> Behtar tareeka: pehle sahi panne dhoondho, phir woh das panne bhejo. Sasta, tez, aur zyada bharosemand. **Yeh Chapter 6.2 ka poora idea hai.**

**3. (jodne wala)** Book 1 Ch 5.5 mein cache ka sauda tha: tez, aur purana ho sakta hai. Context ka sauda kya hai?

> **Jawab:** Zyada sandarbh, aur kam dhyaan.
>
> Zyada bhejo toh model ke paas zyada jaankari hai, aur uska dhyaan utna hi bat gaya hai.
>
> Kam bhejo toh dhyaan tez hai, aur kuch zaroori chhoot sakta hai.
>
> Aur wahi shakal hai jo poori kitaab mein hai: **koi cheez muft nahi milti.** Yahan aap jaankari aur dhyaan ke beech chun rahe ho, aur zyadatar log sirf pehli taraf dekhte hain.
