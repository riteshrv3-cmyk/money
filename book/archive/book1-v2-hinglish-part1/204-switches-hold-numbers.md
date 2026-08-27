# Chapter 1.4 [SPINE]: Switches numbers kaise rakhte hain

Ek switch do baatein keh sakta hai: 0 ya 1. Lekin duniya ke numbers toh
0 se 9 tak ke ankon se bante hain, aur bade numbers, jaise 300 rupaye ya
15 arab, unka kya?

Khud nikaalte hain. Ek switch: do haalat (0, 1). Do switch: chaar haalat
(00, 01, 10, 11). Teen switch: aath haalat. Har naya switch haalat ki
ginti DUGNI kar deta hai, kyunki purani har haalat ab do roop mein ho
sakti hai: naya switch 0 ke saath, ya 1 ke saath.

Ab in haalaton ko naam de do, bas itna hi karna hai:

```
00 ko bolo "zero"      01 ko bolo "ek"
10 ko bolo "do"        11 ko bolo "teen"
```

Ruko, yeh toh wahi hai jo hum das ungliyon ke saath karte hain! Hum 9 ke
baad naya anka shuru karte hain (10), machine 1 ke baad naya switch
shuru karti hai (10). Hamara har anka das guna badhta hai, machine ka
har switch do guna. Bas itna hi farq hai. Ginti ka idea wahi hai, sirf
ungliyaan 10 ki jagah 2 hain.

Toh kitne switch chahiye kaam ke numbers ke liye?

```
 8 switch   =  256 haalat      (0 se 255)
16 switch   =  65,536
32 switch   =  429 crore
64 switch   =  itna bada ki duniya ke saare rupaye, saare
               phone, saari files gin lo, khatam nahi hota
```

Aapke phone ka processor ek saath 64 switchon ke jhund pe kaam karta
hai. Isliye "64-bit phone" likha hota hai dibbe pe. Ab aap jaante ho us
line ka matlab, duniya ke 99% log nahi jaante.

Ek aakhri sawal khud se poochho: machine 2 pe kyun ruki, 10 haalat wala
switch kyun nahi banaya? Ban sakta tha. Lekin bijli ka current kabhi
thoda upar neeche hota rehta hai (noise). Do haalat mein farq itna
bada hai (poora on, poora off) ki chhoti moti hilna-dulna se galti
nahi hoti. Das haalat paas paas hoti, aur har halki kampan galat anka
ban jaati. **2 chuna gaya kyunki 2 sabse bharosemand hai.** Machine
ki har design mein yeh sawal milega: tez chahiye, sasta chahiye, ya
bharosemand chahiye? Yahan bharosa jeeta.

## NAAM

Ek switch ki haalat ka naam **bit** hai (binary digit). Aath bit ke
jhund ka naam **byte**. Do-guna wali ginti ka naam **binary**. Yeh teen
shabd ab aapke hain, aur poori digital duniya inhi se napi jaati hai.

## ASLI DUNIYA SE EK EXAMPLE

Aapka bank balance kahin kisi machine mein 64 switchon ki ek qataar
hai. UPI se 50 rupaye bheje toh us qataar ke kuch switch palte, aur
kisi doosri machine mein doosri qataar ke switch palte. Poori Indian
economy, har khaata, har lena-dena, on/off ki qataaron mein rakhi hai.
Isliye us qataar ki hifaazat (Part 3 mein encryption) itna bada
business hai: switchon mein rakha paisa asli paisa hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

Log binary dekh ke sochte hain machine koi alag, ajnabi bhasha bolti
hai jo insaan ke bas ki nahi. Aapne abhi 5 minute mein poora idea
nikaal liya, kyunki naya kuch tha hi nahi: yeh wahi ginti hai jo aap
bachpan se karte ho, chhoti ungliyon pe. Technology mein "mushkil"
aksar "anjaan" ka doosra naam hota hai.

## MAP PE

Rupaye ka rasta: har cheez jo aap store karte ho, bits mein napti hai,
aur bits rakhne ki jagah ka kiraya lagta hai. Google aapko 15 GB muft
deta hai, aur uske upar mahina charge karta hai. Woh kiraya arabon ka
business hai (Google One, iCloud). Aage Chapter 2.1 mein hum yeh naap
poora seekhenge, kyunki jo cheez napti hai, wahi bikti hai.

## KHUD DEKHO (5 minute)

Ek haath ki paanch ungliyan lo. Band ungli 0, khuli 1. Angoothe se
shuru karo: sirf angootha khula = 1, sirf doosri ungli = 2, dono = 3.
Aise ginte jao. Paanch ungliyon pe aap 31 tak gin sakte ho. Jab yeh
kar loge, aapne binary ko haath se chala liya, ab woh kabhi nahi
bhoolegi.

## SOCHNE KE LIYE

1. (derivation) 8 switch 256 haalat dete hain. Ek purani game console
"8-bit" thi. Uske screen pe ek rang chunne ke liye 8 bit the. Us
console pe kitne rang possible the, aur is se yeh nikaalo ki purane
games waise kyun dikhte the?

> **Jawab:** 256 rang, bas. Isliye purane games ke rang saaf saaf
> tukdon mein dikhte hain, godhuli ka narm dhalta rang unme ban hi
> nahi sakta tha. Aaj ke screen har pixel ke liye 24+ bit rakhte
> hain, 1.6 crore rang, isliye photo asli lagti hai. Sabak: bits ki
> ginti seedha tay karti hai ki machine kitni bareeki dekh sakti
> hai. Yeh niyam AI tak jaayega: wahan bhi bareeki bits mein bikti
> hai.
