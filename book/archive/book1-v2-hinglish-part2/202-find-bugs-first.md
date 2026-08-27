# Chapter 4.2 [DEPTH]: Galti pehle dhoondhna

(DEPTH chapter. Iske bina bhi kahani aage badhegi, lekin jo
founder "testing" ka matlab jaanta hai, woh kabhi kachcha maal
nahi khareedta.)

Pichhle chapter ka sach maan lo: bugs aayenge hi. Toh ab
engineer ki kursi pe baitho aur socho: user tak pahunchne se
PEHLE unhe kaise pakdein?

Pehla jawab sab ka wahi hota hai: "chala ke dekh lo." Theek
hai, chalaya, form bhara, kaam kiya. Ship?

Ruko. Aapne EK raasta chala. Pichhle chapter ke hazaar jodon
mein se ek. Aur agle hafte jab code badlega (code roz badalta
hai), kya aap phir se sab haath se chalaoge? Har badlav ke
baad, har raasta, hamesha? Insaan se yeh hota nahi, aur jahan
insaan se nahi hota, wahan kya aata hai? (Part 1 se jawab:
recipe.)

Toh chaal yeh hai: **jaanchne ka kaam bhi code bana do.** Ek
aur recipe likho jo pehli recipe ko chalaye aur jawab jaanche:

```
maan_lo: jod(2, 2) == 4
maan_lo: jod(-5, 5) == 0
maan_lo: bill_nikaalo(khaali_list) == 0
```

Aisi sau-do-sau jaanchein likh do (har edge case jo dimaag
mein aaye: khaali, zero, minus, bahut bada). Ab har badlav ke
baad machine SAARI jaanchein seconds mein chala deti hai. Kal
wala code aaj bhi sahi hai ya kisi ne tod diya, iska jawab
har din, muft, turant.

Yeh hi testing ka asli matlab hai: ek baar likho, hamesha
jaancho. (Leverage, phir wahi. Achhe engineer ka har auzaar
aakhir mein leverage hi nikalta hai.)

Lekin ek imaandaar baat: tests likhna waqt khaata hai, aaj ki
raftaar girati hai, kal bachaata hai. Toh kitne tests likhein?
Yeh engineering ka nahi, BUSINESS ka sawal hai: galti ki
keemat kya hai? Bank ka paisa-ginanne wala code: galti crores
ki, tests pe kanjoosi paagalpan. Naye idea ka pehla version
jise 50 log dekhenge: kam tests, raftaar zyaada, theek hai.
Jaan boojh ke chuna gaya sauda samajhdaari hai; bina soche
chhoda gaya testing laaparwahi hai. Farq wahi "jaan boojh ke"
hai.

## NAAM

Chhoti jaanchein: **unit tests**. Har badlav pe sab tests
apne aap chalna: **CI (continuous integration)**. Naya badlav
purani cheez tod de: **regression** (yeh shabd engineers ki
zubaan pe roz hota hai: "regression aa gaya").

## ASLI DUNIYA SE EK EXAMPLE

Jab UPI ya bank ka naya version aata hai, woh seedha aap tak
nahi aata. Pehle machine pe lakhon nakli transactions chalti
hain (har edge case: zero rupaye, ulta time, dohri entry),
phir thode asli users pe, phir sab pe. Isliye aapke paise
wale apps itne kam girte hain: unke peeche jaanchon ki fauj
har raat daudti hai. Bharosa jo aap feel karte ho, woh
asal mein tests ki ginti hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Testing = launch se pehle ek baar sab check kar lena." Nahi.
Woh toh sirf ek raat ka pehra hai. Asli testing STHAAYI hai:
code ke saath saath jaanchon ki fauj bhi badhti rehti hai,
aur har badlav unse guzar ke hi bahar jaata hai. Isliye jab
aap kisi se software banwao, toh poochhna: "tests kitne
hain, aur kya woh har badlav pe apne aap chalte hain?" Is ek
sawal se aap aadhe kachche vendors chhaant doge.

## MAP PE

Kaun kamata hai: QA/test engineers ka poora pesha (India
mein lakhs log), aur test-automation ke tools ka apna bazaar.
Lekin naya mod dekho: AI ab tests LIKHNE mein sabse achha
hai, kyunki edge cases sochna pattern ka kaam hai. Toh
"haath se test chalaane wala" pesha sikud raha hai, aur
"jaanchon ka intezaam design karne wala" mehnga ho raha hai.
Wahi seedhi, phir se: kaam machine ko, soch insaan ko, paisa
soch wale ko.

## KHUD DEKHO (5 minute)

Login form ke liye 5 aisi jaanchein kaagaz pe likho jo use
tod sakti hain (khaali password? emoji wala email? 1000
akshar? do baar submit? net beech mein gaya?). Aapne abhi
test plan likha, bina ek line code ke. Banwaate waqt yehi
list vendor ko doge toh woh samajh jaayega ki saamne kachcha
grahak nahi baitha.

## SOCHNE KE LIYE

1. (derivation) Maan lo tests likhna bilkul muft ho jaaye
(AI likh de). Kya tab bugs zero ho jaayenge?

> **Jawab:** Nahi. Tests sirf woh jaanchte hain jo kisi ke
> DIMAAG mein aaya. Bug wahan hota hai jahan kisi ka dimaag
> gaya hi nahi (Chapter 4.1 ka gap). Muft tests us gap ko
> chhota karenge, khatam nahi: jo jod socha nahi, uski jaanch
> bhi nahi likhi jaayegi, AI se bhi tabhi likhegi jab use
> sochne ka rasta mile. Isliye zero-bug ka waada physics
> nahi, marketing hai. Ho sakta hai wala best: gap chhota
> karo, pakadne ki raftaar badhao, nuksan ki had bandho.
