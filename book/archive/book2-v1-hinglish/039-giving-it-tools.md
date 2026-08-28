# Chapter 6.3  [SPINE]
## Tools dena

### Samvaad

**Madhav:** RAG mein aap use jaankari dete ho. Ab use kaam karne dena hai. Farak kya hai?

**Kabir:** Jaankari padhne ki cheez hai. Kaam ka asar hota hai.

**Madhav:** Toh ek program ko batana hai ki kaunse kaam mumkin hain. Kaise batayenge?

**Kabir:** Ek list. Har kaam ka naam, aur woh kya karta hai.

**Madhav:** Aur kaam ko kuch chahiye hoga. Jaise "email bhejo" ko kiska naam chahiye.

**Kabir:** Toh yeh bhi likhna padega ki kya kya dena hai.

**Madhav:** Woh list model ko kaise pahunchegi?

**Kabir:** Context mein, sawal ke saath.

**Madhav:** Toh woh list bhi tokens hai. Aur uska daam bhi hai.

**Kabir:** Toh bahut saare tools dene se har sawal mehnga ho jaayega.

**Madhav:** Aur usse bura kya hoga?

**Kabir:** Model ko chunna mushkil hoga. Pachaas tools mein se sahi chunna.

**Madhav:** Bas. Ab ek aur baat. Aapne tool ka varnan likha: "yeh email bhejta hai." Yeh varnan kiske liye hai?

**Kabir:** Model ke liye.

**Madhav:** Toh use kaise likhna chahiye?

**Kabir:** Saaf. Jaise kisi naye insaan ko samjha rahe hon.

**Madhav:** Aur agar varnan dhundhla ho?

**Kabir:** Toh woh galat tool chunega, ya sahi tool galat tareeke se istemaal karega.

**Madhav:** Yeh sabse aam wajah hai jab agent kaam nahi karte. Ab aage. Model ne likha ki email bhejo. Program ne bhej diya. Ab?

**Kabir:** Nateeja model ko wapas dena hoga.

**Madhav:** Aur agar kaam fail ho jaaye?

**Kabir:** Woh bhi batana hoga. Warna woh maan lega ki ho gaya.

**Madhav:** Aur galti ka message kaisa hona chahiye?

**Kabir:** Aisa jisse woh samajh sake ki ab kya karna hai. "Error 500" se kuch nahi hoga.

**Madhav:** Bas. Ab aakhri, aur yeh sabse zaroori hai. Kaunse tools dene chahiye aur kaunse nahi?

**Kabir:** Jo zaroori hain.

**Madhav:** Ek sawal se tay karo. Ek tool jo padhta hai, aur ek jo badalta hai. Farak?

**Kabir:** Padhne wale se galti sasti hai. Badalne wale se mehngi.

**Madhav:** Aur mitane wale se?

**Kabir:** Woh wapas nahi aata.

**Madhav:** Toh ek niyam bana lo.

**Kabir:** Padhna aasani se do. Badalna soch kar. Mitana bina poochhe kabhi nahi.

### Naam

Us list ko **tool definitions** kehte hain, aur model ke us likhe ko jo tool maangta hai, **tool call**.

Ek poora chakkar:

```
1.  program bhejta hai: sawal + tools ki list
2.  model likhta hai: "yeh tool chalao, in cheezon ke saath"
3.  program us tool ko SACH MEIN chalata hai
4.  nateeja wapas context mein jaata hai
5.  model us nateeje ko dekh kar aage badhta hai
```

Aur teen baatein jo har asli system mein mayne rakhti hain.

**Ek: tool ka varnan hi asli prompt hai.**

Model us varnan ke aadhaar pe chunta hai. Dhundhla varnan matlab galat chunav. Yeh sabse aam wajah hai ki agent kaam nahi karte, aur log aksar model ko doshi maante hain.

**Do: har tool context mein jagah aur paisa leta hai.**

Pachaas tools ka matlab hai har sawal pe pachaas varnan bheje jaa rahe hain, chahe kisi ki zaroorat na ho. Aur chunav bhi mushkil ho jaata hai.

Isliye achhe systems mein tools chhaante jaate hain: iss kaam ke liye yeh paanch, us kaam ke liye woh teen.

**Teen: khatra tool se aata hai, model se nahi.**

Model ek text banane wali cheez hai. Woh kuch nahi kar sakta. Jo kuch bhi ho sakta hai, woh un tools se hoga jo aapne diye.

Toh ek saada, mazboot niyam:

```
PADHNE WALE TOOLS      aasani se do
                       galti sasti hai, wapas ki ja sakti hai

BADALNE WALE TOOLS     soch kar do
                       aur wapas jaane ka rasta rakho (Book 1, Ch 7.3)

MITANE / BHEJNE WALE   insaan se poochhe bina kabhi nahi
                       (email bhejna, paisa bhejna, file mitana)
```

Aakhri wali ki wajah Chapter 5.2 se aati hai: **model apni galti khud nahi pehchan sakta.** Toh jahan galti wapas nahi ho sakti, wahan ek insaan ka haath hona chahiye.

### Asli duniya se

Shuruaat mein har company apne tools apne tareeke se banati thi, aur har AI product ke liye alag se kaam karna padta tha.

2024 ke aas-paas iske liye ek saanjha tareeka phailna shuru hua, taaki ek hi tool kai alag AI products ke saath chal sake.

Ab Book 1 Chapter 4.4 aur 6.4 pe lagao. Yeh ek protocol jaisa hai: ek tay shakal jispe log sehmat ho jaate hain.

Aur uska wahi faayda hai: ek baar tool banao, sab jagah chale. Aur wahi sawal bhi: **woh tay shakal kaun tay karta hai, aur agar woh kal badal de toh?**

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki tool dene se model zyada samajhdaar ho jaata hai.**

Uske andar kuch nahi badla. Uski aankh ki seemayein hat gayi hain (Ch 5.2), aur ab uski galtiyon ka asar hota hai.

Doosri galti: **model ko doshi maanna jab woh galat tool chune.**

Pehle apna varnan padho. Aksar wahin problem hoti hai. Do tools ke varnan lagbhag ek jaise hain, ya varnan mein yeh nahi likha ki kab istemaal na karein.

Teesri galti, aur yeh sabse mehngi hai: **model ko woh tools de dena jo aap khud kisi naye insaan ko pehle din nahi doge.**

Log ek agent ko poora database access, sab kuch mitane ka haq, aur paise bhejne ka rasta de dete hain, aur phir hairan hote hain.

**Ek saada test:** agar aap yeh taakat ek naye, tez, aatmvishwas se bhare hue intern ko nahi doge jo apni galti nahi pehchan sakta, toh model ko bhi mat do.

### Sochne ke liye

**1. (samajh check)** Aapka agent galat tool chunta rehta hai. Sabse pehle kya dekhoge?

> **Jawab:** Tool ke varnan.
>
> Kya do varnan lagbhag ek jaise hain? Kya usmein likha hai ki kab istemaal karna hai aur kab nahi? Kya uske andar ki cheezon ke naam saaf hain?
>
> Model us varnan ke alaawa kuch nahi jaanta. Uske liye woh varnan hi poori sachai hai.
>
> **Model ko badalna aakhri kadam hai, pehla nahi.**

**2. (samajh check)** Aap ek agent bana rahe ho jo aapke emails sambhale. Kaunse tools doge?

> **Jawab:** Padhna aur dhoondhna: aasani se.
>
> Draft banana: theek hai, kyunki draft ka koi asar nahi hota.
>
> **Bhejna: nahi, ya sirf aapki ijaazat ke saath.** Kyunki bheja hua email wapas nahi aata, aur model apni galti nahi pehchan sakta.
>
> Yeh ek saada niyam hai jo lagbhag har agent pe lagta hai: **cheez taiyaar karne do, bhejne ka button apne paas rakho.**

**3. (jodne wala)** Chapter 6.1 mein tha ki model ko sirf woh dikhta hai jo wapas likh kar bataya gaya. Tools ke saath uska khatra kya hai?

> **Jawab:** Ki tool ka nateeja bhi sirf text hai, aur model use maan lega.
>
> Agar ek tool galat nateeja lauta de, toh model us galat nateeje pe poora kaam khada kar dega.
>
> Aur usse gehri baat: **agar us nateeje mein koi nirdesh likha ho, toh model use padh lega.**
>
> Woh nateeja aur nirdesh mein farak nahi karta. Dono uske liye ek jaisi likhawat hain.
>
> Yeh Chapter 6.7 ka poora aadhaar hai, aur woh iss kitaab ka sabse zaroori suraksha wala chapter hai.
