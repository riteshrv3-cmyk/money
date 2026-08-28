# Chapter 2.6  [SPINE]
## Data kahan se aaya

### Samvaad

**Madhav:** Training ke liye kharabon examples chahiye. Woh kahan se aaye?

**Kabir:** Internet se.

**Madhav:** "Internet" ek jagah nahi hai. Kaun sa hissa?

**Kabir:** Websites. Wikipedia.

**Madhav:** Wikipedia kitna bada hai, likhawat mein?

**Kabir:** Bahut. Kai GB?

**Madhav:** Angrezi Wikipedia lagbhag 20 GB hai. Aur training ke liye lakhon GB chahiye.

**Kabir:** Toh Wikipedia ek hazaarva hissa bhi nahi hai.

**Madhav:** Toh baaki kahan se aaya?

**Kabir:** Har website se. Blog, forum, khabar, dukaan, sab.

**Madhav:** Aur uske alaawa?

**Kabir:** Kitaabein? Code?

**Madhav:** Dono, aur bahut saara. Code khaas taur pe, aur uski ek dilchasp wajah hai. Kya lagta hai?

**Kabir:** Kyunki log code likhwana chahte hain?

**Madhav:** Woh ek wajah hai. Doosri gehri hai: code mein tark saaf likha hota hai. Har cheez ka kaaran wahin hota hai. Us se model ka tark har jagah behtar ho jaata hai, sirf code mein nahi.

**Kabir:** Toh code padhne se woh soch ne mein behtar hua?

**Madhav:** Aisa dikha hai. Ab aage. Yeh saara text kiska hai?

**Kabir:** Jinhone likha.

**Madhav:** Kya unse poocha gaya?

**Kabir:** Nahi.

**Madhav:** Kya unhe paisa mila?

**Kabir:** Nahi.

**Madhav:** Kya woh jaante bhi hain?

**Kabir:** Zyadatar nahi.

**Madhav:** Ab ek sawal jiska jawab abhi kisi ke paas nahi hai. Kya yeh chori hai, ya padhna hai?

**Kabir:** Padhna toh sabko allowed hai.

**Madhav:** Aap ek kitaab padh kar uski shaili mein likh sakte ho?

**Kabir:** Haan.

**Madhav:** Toh machine kyun nahi?

**Kabir:** Kyunki... woh lakhon kitaabein ek saath padh leti hai aur turant kar deti hai?

**Madhav:** Toh farak paimane ka hai, kism ka nahi?

**Kabir:** Shayad. Lekin jab paimana itna badalta hai toh cheez alag ho jaati hai.

**Madhav:** Yeh ek asli tark hai aur ispe adaalaton mein bahas chal rahi hai, abhi. Main aapko jawab nahi de sakta kyunki kisi ke paas nahi hai. Lekin ek baat pakki hai. Ab batao: agar kal kanoon keh de ki bina ijaazat ka data nahi chalega, toh kya hoga?

**Kabir:** Purane models pe kya asar padega? Woh toh ban chuke hain.

**Madhav:** Aur Chapter 2.3 se aap jaante ho ki unmein se kuch nikaala nahi ja sakta.

**Kabir:** Toh unhe dobara banana padega. Poora.

**Madhav:** Karodon dollar. Aur yehi wajah hai ki yeh sawal itna bada hai. **Yeh sirf naitikta ka sawal nahi hai. Yeh iss poore udyog ki neev pe khada hai.**

### Naam

Training data aam taur pe teen jagah se aata hai:

```
WEB
├── karodon pages, apne aap ikattha kiye gaye
├── sabse bada hissa, aur sabse kharaab quality
└── ismein sab kuch hai: achha, bura, jhooth, nafrat

KITAABEIN AUR LEKH
├── bahut behtar quality, lambi soch, poore tark
├── sabse zyada kanooni jhagda yahin hai
└── paimane mein chhota, asar mein bada

CODE
├── public repositories se
├── saaf tark, jaanchi ja sakne wali sahi-galat
└── isse model ka tark har jagah behtar hota hai
```

Aur teen sawal jo har dataset pe uthte hain:

**Kiska tha?** Zyadatar logon se poocha nahi gaya aur unhe paisa nahi mila. Kanoon abhi tay nahi hua hai, aur alag deshon mein alag disha mein ja raha hai.

**Kis samay ka hai?** Har model ki ek **cutoff** hoti hai: us tarikh ke baad ki duniya use pata nahi hai. Yeh ek pakki, sakht seema hai.

**Kis duniya ka hai?** Internet pe likhawat barabar nahi bant ti. Kuch bhashaayein bahut hain, kuch lagbhag nahi. Kuch nazariye bahut hain, kuch nahi.

Teesri baat sabse kam dikhti hai aur sabse zyada asar daalti hai. **Model us duniya ka aaina hai jo likhi gayi thi, us duniya ka nahi jo hai.**

Aur do cheezein jinmein farak zaroori hai:

```
DUNIYA MEIN JO KAM HAI       →  data mein bhi kam hai
DUNIYA MEIN JO ZYADA HAI     →  lekin likha kam gaya
                                 (yeh doosri wali zyada khatarnak hai)
```

Bahut se log, kaam, aur jagahein asli duniya mein bade hain aur internet pe chhote. Model ke liye woh chhote hi rahenge.

### Asli duniya se

Zyadatar bade models ki ek **knowledge cutoff** hoti hai, aur woh saaf batayi jaati hai. Us tarikh ke baad jo hua, model use nahi jaanta.

Isliye woh aatmvishwas se purani baat bata dega. Woh jhooth nahi bol raha. Uske liye woh abhi bhi sach hai.

Aur isiliye aaj ke zyadatar AI products model ko search se jodte hain: taazi jaankari sawal ke saath bhej di jaati hai, model ke andar se nahi aati. Yeh Chapter 6.2 ka vishay hai.

Do baatein isse nikalti hain jo aap roz istemaal kar sakte ho:

```
purani, sthir baat        →  model se poochna theek hai
nayi ya badalne wali baat →  model pe bharosa mat karo
```

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki model ne "internet padh liya" isliye woh sab jaanta hai.**

Usne internet ka ek chuna hua hissa dekha, ek tarikh tak, aur usmein se bhi sirf patterns bache (Chapter 2.3).

Aur woh hissa random nahi tha. Kisi ne tay kiya ki kya lena hai, kya chhodna hai, aur kis cheez ko zyada wazan dena hai. Woh faisle dikhte nahi aur unka asar poore model pe rehta hai.

Doosri galti: **yeh maan lena ki data ki problem sirf naitik hai.**

Woh technical bhi hai, aur seedha aap pe asar daalti hai. Jo kaam, bhasha, ya ilaaka internet pe kam likha gaya, uspe model kamzor hoga, aur woh kamzori aatmvishwas ke saath aayegi.

**Model ki kamzori wahan hoti hai jahan likhawat kam thi, na ki wahan jahan kaam mushkil hai.** Yeh do bilkul alag baatein hain, aur log inhe hamesha mila dete hain.

### Sochne ke liye

**1. (samajh check)** Aap apne sheher ke kisi chhote kanoon ke baare mein poochte ho aur model aatmvishwas se galat jawab deta hai. Kya hua?

> **Jawab:** Woh baat likhawat mein bahut kam thi, isliye nichodne mein lagbhag gayab ho gayi (Chapter 2.3).
>
> Aur woh chup nahi reh sakta, kyunki uska kaam hi agla token chunna hai. Toh woh woh likhta hai jo aisi jagah pe aksar likha hota hai, jo aksar kisi bade sheher ka kanoon hoga.
>
> Ilaaj: use woh kanoon saath bhejo. Tab woh andar se nahi, saamne se padhega.
>
> **Jahan data kam tha, wahan model se poochna nahi chahiye. Wahan use jaankari deni chahiye.**

**2. (samajh check)** Do models hain. Ek 2024 tak ka data jaanta hai, doosra 2026 tak. Kya doosra hamesha behtar hai?

> **Jawab:** Nayi jaankari ke liye haan, baaki ke liye zaroori nahi.
>
> Cutoff sirf yeh batati hai ki uske paas kis samay tak ki duniya hai. Woh yeh nahi batati ki woh soch ne mein, likhne mein, ya tark mein behtar hai.
>
> Ek purana lekin behtar train kiya gaya model ek naye lekin kamzor model se behtar ho sakta hai.
>
> Aur agar aap taazi jaankari saath bhej rahe ho, toh cutoff ka mayne hi bahut kam ho jaata hai.

**3. (jodne wala)** Book 1 Ch 6.9 mein tha ki paisa neeche se aata hai aur scarcity pe rukta hai. Data uss tasveer mein kahan hai?

> **Jawab:** Woh un cheezon mein se ek hai jo abhi scarce ban rahi hai.
>
> Shuruaat mein data lagbhag muft tha: web utha lo. Ab teen cheezein badal rahi hain: aasan data khatam ho raha hai, log apne data ko band kar rahe hain, aur kanoon aa raha hai.
>
> Isliye ab bade paise us data ke liye die ja rahe hain jo kisi ek jagah ikattha hai: khabar, kitaabein, forum, aur woh baat-cheet jo log AI products ke saath karte hain.
>
> **Jab koi cheez muft se scarce banti hai, tab uske maalik ki taakat achanak badh jaati hai.** Yeh Chapter 7.1 mein poora khulega.
