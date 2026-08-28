# Chapter 2.4  [DEPTH]
## Error ko naapna

*DEPTH chapter. Pehli baar mein chhod sakte ho. Iske baad "training" ek jaadui shabd nahi rehta.*

### Samvaad

**Madhav:** Model ne "Mumbai" guess kiya, sahi tha "Dilli". Ab batao galti kitni thi.

**Kabir:** Woh galat tha. Galti poori.

**Madhav:** Aur agar usne "Mumbai" ko 90 percent sambhavna di hoti, "Dilli" ko 5?

**Kabir:** Toh woh bahut galat tha.

**Madhav:** Aur agar "Mumbai" ko 35 percent, "Dilli" ko 33?

**Kabir:** Toh woh galat tha lekin thoda hi.

**Madhav:** Toh galti sirf haan-na nahi hai. Woh ek maatra hai.

**Kabir:** Haan.

**Madhav:** Ab yeh zaroori kyun hai? Agar galti sirf haan-na hoti toh kya problem hoti?

**Kabir:** Toh mujhe pata nahi chalta ki main sudhar raha hoon ya nahi.

**Madhav:** Aur bhi. Socho: "Dilli" ko 5 se 20 percent le jaana ek sudhaar hai. Kya woh haan-na mein dikhega?

**Kabir:** Nahi. Dono baar jawab galat hi rahega.

**Madhav:** Toh haan-na wali galti ke saath aap seekh hi nahi sakte, kyunki aapko chhote sudhaar dikhte hi nahi.

**Kabir:** Toh maatra chahiye. Har chhote badlav pe woh thodi hilni chahiye.

**Madhav:** Bas. Ab ek maatra banate hain. Model har mumkin token ko ek sambhavna deta hai. Sahi jawab ek hai. Aap kya naapoge?

**Kabir:** Sahi jawab ko usne kitni sambhavna di.

**Madhav:** Aur woh zyada honi chahiye ya kam?

**Kabir:** Zyada.

**Madhav:** Toh galti kya hui?

**Kabir:** Ulta. Jitni kam sambhavna, utni zyada galti.

**Madhav:** Achha. Ab ek problem. Model ne sahi jawab ko 0.5 sambhavna di, aur ek doosre case mein 0.25. Kitna bura hai doosra?

**Kabir:** Do guna bura.

**Madhav:** Aur 0.5 se 0.001?

**Kabir:** Paanch sau guna bura.

**Madhav:** Ab sochiye: 0.5 se 0.25 mein girna, aur 0.002 se 0.001 mein girna. Dono aadhe hue. Kya dono barabar bure hain?

**Kabir:** Hmm. Doosra zyada bura lagta hai. Woh toh pehle se hi lagbhag zero tha.

**Madhav:** Ulta socho. Doosre case mein model pehle se hi bilkul galat tha. Uska aadha aur galat hona itna mayne rakhta hai?

**Kabir:** Shayad nahi. Pehla case zyada mayne rakhta hai, kyunki wahan woh lagbhag sahi tha.

**Madhav:** Toh humein ek aisi maatra chahiye jo aadhe hone ko hamesha ek jaisa maane, chahe kahin se aadha ho. Aisi maatra kaisi hogi?

**Kabir:** Woh sambhavna ke seedhe anupaat mein nahi ho sakti.

**Madhav:** Sahi. Isliye wahan ek aisa hisaab lagta hai jo har baar aadha hone pe utna hi jodta hai. Uska naam abhi zaroori nahi hai. Zaroori yeh hai ki woh kyun chahiye tha.

**Kabir:** Taaki har guna badlav barabar gina jaaye.

**Madhav:** Ab aakhri sawal. Ek example ki galti nikal aayi. Poore data ki galti kya hai?

**Kabir:** Sabka jod. Ya average.

**Madhav:** Aur training ka lakshya kya hai?

**Kabir:** Us average ko kam se kam karna.

**Madhav:** Bas. Poori training ek line mein: **ek number hai jo batata hai ki model kitna galat hai, aur saara kaam use neeche laana hai.**

### Naam

Us maatra ka naam hai **loss**. Woh ek number hai. Zyada matlab zyada galat.

Aur woh khaas hisaab jo har guna badlav ko barabar ginta hai, uska naam **cross-entropy** hai. Uska sirf ek kaam hai:

```
model ne sahi jawab ko          loss
0.9 sambhavna di                bahut kam
0.5                             thodi zyada
0.1                             kaafi zyada
0.001                           bahut zyada
0.0000001                       bahut hi zyada
```

Har baar sambhavna das guna girti hai, aur loss utna hi badhta hai, chahe woh kahin se gire.

Teen baatein jo iss se nikalti hain:

**Ek: loss training ki poori bhasha hai.** Aap kabhi model se nahi poochte "kya tum sahi ho?" Aap sirf loss dekhte ho, aur use girana hi sab kuch hai.

**Do: loss aur upyogita ek cheez nahi hain.** Loss yeh naapta hai ki model agla token kitni achhi tarah guess karta hai. Woh yeh nahi naapta ki jawab sach hai, ya kaam ka hai, ya surakshit hai.

Yeh farak bahut mayne rakhta hai. **Model ko sach bolne ke liye train nahi kiya gaya. Use likhawat ka andaza lagane ke liye train kiya gaya.** Sach uska side effect hai, uska lakshya nahi.

Yeh Chapter 2.7 mein wapas aayega, jahan hum dekhenge ki insaan ne isko kaise sudhaara.

**Teen: loss girta rehta hai lekin nateeja ek jagah ruk jaata hai.** Ek waqt aata hai jab loss thoda thoda gir raha hota hai aur model sach mein behtar nahi ho raha hota. Isliye sirf loss dekhna kaafi nahi hai, aur asli jaanch alag hoti hai. Chapter 5.3.

### Asli duniya se

Training ke doraan log ek graph dekhte hain: loss, waqt ke saath.

Woh graph pehle tezi se girta hai, phir dheere, phir lagbhag seedha ho jaata hai.

Aur us graph ka aakar hi bahut kuch batata hai. Agar woh achanak upar chala jaaye, toh kuch toota hai. Agar woh girna hi band kar de, toh ya toh model chhota hai ya data khatam ho gaya.

Ek dilchasp cheez: kabhi kabhi loss dhare-dheere girta rehta hai aur model achanak koi naya kaam karne lagta hai jo woh pehle nahi kar pata tha. Bahar se woh ek chhalang lagti hai, aur andar loss mein koi chhalang nahi hoti.

Yeh abhi poori tarah samjha nahi gaya hai, aur ispe log bahas karte hain. Kuch kehte hain ki woh sach mein ek nayi kaabiliyat hai, kuch kehte hain ki hum use naapne ka tareeka hi aisa chun lete hain ki woh chhalang jaisi dikhe.

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki kam loss matlab achha model.**

Loss ek naap hai us kaam ka jo training mein diya gaya tha: agla token guess karo. Aap us kaam mein kamaal kar sakte ho aur phir bhi:

```
jhooth bolo (kyunki jhooth bhi likhawat mein aata hai)
nuksaan pahunchane wali baat likho
sawal ka jawab dene ki jagah use ghuma do
```

Kyunki inmein se koi bhi loss mein nahi naapa gaya.

Yeh ek gehri baat hai jo sirf AI ki nahi hai: **jo aap naapte ho, wahi aapko milta hai.** Aur jo aap nahi naapte, uske baare mein koi guarantee nahi hai.

Poora Chapter 2.7 issi ek problem ka hal hai.

### Sochne ke liye

**1. (samajh check)** Model ne sahi jawab ko 0.4 sambhavna di. Kya woh galat tha?

> **Jawab:** Yeh sawal hi adhoora hai.
>
> Agar usne wahi token chuna jise sabse zyada sambhavna thi, aur woh sahi tha, toh jawab sahi aaya.
>
> Lekin loss phir bhi zero nahi hai, kyunki usne sahi jawab ko poora bharosa nahi diya.
>
> **Sahi jawab dena aur pakka hona do alag baatein hain.** Training dono ko dekhti hai. Aur isiliye training aur istemaal mein farak hai: training mein har sambhavna mayne rakhti hai, istemaal mein sirf chuna hua token dikhta hai.

**2. (samajh check)** Loss girna band ho gaya. Do wajahein batao.

> **Jawab:**
>
> **Ek:** model ki apni seema aa gayi. Usmein itne hi numbers hain, aur woh usse zyada nichod nahi sakta.
>
> **Do:** data khatam ho gaya, ya woh dohraya jaane laga. Naya seekhne ko kuch bacha hi nahi.
>
> Do alag ilaaj: pehle ke liye bada model, doosre ke liye zyada ya behtar data.
>
> Yeh farak pehchanna training ka sabse mehnga faisla hai, kyunki dono ilaaj karodon dollar ke hain.

**3. (jodne wala)** Chapter 1.3 mein tha ki sabse achha jawab bhi aksar galat hoga. Loss usse kaise judta hai?

> **Jawab:** Loss lagbhag kabhi zero nahi ho sakta, aur woh honi bhi nahi chahiye.
>
> Agar model kisi text ko poori tarah, bina galti ke guess karne lage, toh usne us text ko yaad kar liya hai, seekha nahi.
>
> Aur uska nateeja bura hota hai: woh us text pe kamaal karega aur kisi naye text pe bekaar.
>
> Iska naam **overfitting** hai. Aur uska ilaaj ulta lagta hai: model ko itna achha mat hone do ki woh apne data ko ratt le.
>
> **Thodi galti rehna zaroori hai. Woh nishaani hai ki usne pattern seekha hai, jawab nahi.**
