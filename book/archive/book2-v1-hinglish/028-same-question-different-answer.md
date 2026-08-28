# Chapter 4.3  [SPINE]
## Same sawal, alag jawab kyun

### Samvaad

**Madhav:** Aap ek hi sawal do baar poochte ho aur do alag jawab aate hain. Model wahi hai, file wahi hai. Kaise?

**Kabir:** Kuch random hoga.

**Madhav:** Kahan? Hisaab toh pakka hai. Wahi numbers andar, wahi bahar.

**Kabir:** Toh phir alag kaise?

**Madhav:** Chapter 1.3 yaad karo. Model har mumkin token ke liye kya deta hai?

**Kabir:** Ek sambhavna. Har token ki.

**Madhav:** Toh ek jawab nahi, ek poori list. Ab usmein se ek chunna hai. Kaun chunta hai?

**Kabir:** Model?

**Madhav:** Model ne apna kaam kar diya. Usne list de di. Chunna uske baad ka kaam hai, aur woh model ke bahar hai.

**Kabir:** Toh chunne mein random daala jaata hai.

**Madhav:** Ab batao: hamesha sabse zyada sambhavna wala chuna jaaye toh kya hoga?

**Kabir:** Har baar wahi jawab. Kyunki hisaab pakka hai.

**Madhav:** Aur kya woh achha hoga?

**Kabir:** Pakka hoga. Lekin shayad bore hoga.

**Madhav:** Kyun bore?

**Kabir:** Kyunki woh hamesha sabse aam wala shabd chunega. Kabhi kuch naya nahi.

**Madhav:** Aur agar aap kabhi kabhi doosra, teesra wala chuno?

**Kabir:** Toh jawab alag alag aayenge. Zyada dilchasp.

**Madhav:** Aur nuksaan?

**Kabir:** Kabhi kabhi galat wala chun liya jaayega.

**Madhav:** Toh yeh ek sauda hai. Ab batao, kis kaam mein pakka jawab chahiye?

**Kabir:** Hisaab. Code. Tathya. Tarjuma.

**Madhav:** Aur kis mein alag alag chahiye?

**Kabir:** Kahani. Naam sochna. Ideas.

**Madhav:** Aur ab yeh dekho: kya "hamesha sabse sambhavit" hamesha sabse sahi hai?

**Kabir:** Lagta toh hai.

**Madhav:** Ek vaakya socho. Har kadam pe sabse aam shabd chuno. Kya nikelga?

**Kabir:** Kuch bahut aam. Ghisa pita.

**Madhav:** Aur kabhi kabhi woh ek gaddhe mein bhi phans sakta hai, jahan har agla sabse aam shabd use aur gehre le jaata hai.

**Kabir:** Toh thoda random hona kabhi kabhi behtar bhi hai.

**Madhav:** Aur wahi wajah hai ki zyadatar products thoda random rakhte hain, chahe kaam pakka ho.

### Naam

Us "kitna random" wale knob ka naam hai **temperature**.

```
temperature 0     hamesha sabse sambhavit token
                  pakka, dohraya ja sakta hai, kabhi kabhi ghisa pita

temperature ~0.7  aksar sabse sambhavit, kabhi doosra teesra
                  zyadatar products ka default

temperature 1.5+  bahut variety
                  bekaar cheezein aane lagti hain
```

Aur do aur knob jo saath chalte hain:

```
top-k     sirf sabse upar ke k tokens mein se chuno, baaki phenk do
top-p     utne tokens rakho jinki sambhavna milkar p tak pahunche
```

Dono ka kaam ek hi hai: **bilkul bekaar tokens ko chunav se hataana**, taaki randomness sirf theek-thaak vikalpon ke beech ho.

Aur ab do baatein jo iss chapter ki jaan hain.

**Ek: chunav model ke bahar hai.**

Model ek list deta hai. Chunna uske baad ka kaam hai, aur woh product ka faisla hai. Isliye ek hi model do jagah alag lag sakta hai (Chapter 2.9).

**Do: temperature 0 ka matlab "sahi" nahi hai.**

Yeh sabse aam galtfehmi hai. Temperature 0 ka matlab hai **dohraya ja sakne wala**, na ki sahi.

```
temperature 0    →  har baar wahi jawab
                    agar woh jawab galat hai, toh har baar galat
```

Woh galti ko hataata nahi. Woh use sthir kar deta hai.

Yeh dhyaan dene laayak hai: kuch kaamon mein sthir galti ek badalti hui galti se **behtar** hai, kyunki use pakda aur theek kiya ja sakta hai. Aur kuch mein badtar, kyunki woh har baar chup-chaap wahi galti dohrayegi.

### Asli duniya se

Zyadatar chat products aapko yeh knob nahi dikhate. Woh apne aap ek value chun lete hain, aksar 0.7 ke aas-paas.

Jab aap seedha model se baat karte ho, ek program ke through, toh yeh aapke haath mein hota hai.

Aur wahin ek asli, kaam ki practice hai:

```
code, hisaab, data nikalna   →  temperature 0 ya bahut kam
saaransh, tarjuma            →  kam
likhna, ideas, naam          →  zyada
```

Aur ek chalak istemaal jo bade systems mein hota hai: **ek hi sawal ko kai baar chalao, thodi randomness ke saath, aur dekho ki jawab ek jaise aate hain ya nahi.**

Agar paanchon jawab ek jaise hain, toh model us baat pe sthir hai. Agar paanchon alag hain, toh woh andaza laga raha hai.

Yeh ek asli tareeka hai yeh naapne ka ki model kitna "pakka" hai, aur woh uske aatmvishwas se kahin behtar hai. Chapter 5.4.

### Yahan log kya galat samajhte hain

Sabse aam galti: **temperature ko "creativity" ka knob samajhna.**

Woh creativity nahi badhata. Woh sirf kam sambhavit tokens ko chunav mein aane deta hai. Kabhi woh naya lagta hai, aur kabhi woh sirf galat hota hai.

Doosri galti: **temperature 0 ko "sach mode" samajhna.**

Woh sach nahi deta. Woh ek hi jawab deta hai, baar baar. Agar model galat hai, toh woh pakka galat rahega.

Teesri galti, jo bade systems mein mehngi padti hai: **yeh maan lena ki temperature 0 se sab kuch dohraya ja sakega.**

Aksar chhoti chhoti wajahon se, jaise batch mein aapke saath kaun hai, nateeja bilkul waisa ka waisa nahi aata. Toh "pakka jawab" bhi lagbhag pakka hota hai, poori tarah nahi.

Isliye agar aapke system ko sach mein ek hi jawab chahiye, toh use jaanchna padega, maan lena kaafi nahi hai.

### Sochne ke liye

**1. (samajh check)** Aap ek system bana rahe ho jo bill se number nikaalta hai. Temperature kya rakhoge?

> **Jawab:** Zero, ya jitna kam ho sake.
>
> Yahan koi variety nahi chahiye. Ek hi sahi jawab hai, aur alag alag jawab sirf nuksaan hain.
>
> Aur uske saath do cheezein aur karni chahiye: jawab ki shakal tay karo (sirf number, koi baat nahi), aur use jaancho (kya woh sach mein ek number hai, kya woh bill mein kahin hai).
>
> **Temperature 0 galtiyan nahi hataata. Woh sirf unhe dohraya ja sakne wala banata hai.**

**2. (samajh check)** Aap ek hi sawal paanch baar poochte ho aur paanch bilkul alag jawab aate hain. Kya nikalta hai?

> **Jawab:** Ki model us baat pe sthir nahi hai. Woh andaza laga raha hai.
>
> Agar woh sach mein jaanta hota, toh sabse sambhavit token itna aage hota ki thodi randomness usse hila nahi paati.
>
> **Yeh ek asli, kaam ka tareeka hai:** jahan bharosa zaroori ho, wahan wahi sawal kai baar poocho aur jawabon ko mila kar dekho.
>
> Ek jaise jawab ek sanket hain. Alag alag jawab ek chetavni hain. Aur yeh uske aatmvishwas se kahin behtar naap hai.

**3. (jodne wala)** Chapter 1.3 mein tha ki sabse achha jawab bhi aksar galat hoga. Temperature usmein kya jodta hai?

> **Jawab:** Woh us baat ko ek knob de deta hai.
>
> Temperature 0 pe aap hamesha sabse achha andaza le rahe ho. Woh aksar sahi hoga aur kabhi kabhi galat, aur woh galti pakki hogi.
>
> Temperature badhane pe aap jaan-boojh ke kabhi kabhi doosra sabse achha le rahe ho. Aap thodi zyada galtiyan mol le rahe ho, badle mein variety ke liye.
>
> **Kisi bhi setting pe galti khatam nahi hoti.** Woh us tareeke ke andar hai, jaise 90 laal gendon wale thaile mein thi.
