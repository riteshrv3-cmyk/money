# Chapter 3.3 [DEPTH]: Translator ke do tareeke

(DEPTH chapter. Skip kar sakte ho; lautoge toh "compiled vs
interpreted" wali har tech baat khul jaayegi.)

Ek kitaab Hindi mein hai, aapko English walon tak pahunchani hai.
Do raaste hain, dono aap khud soch sakte ho:

**Pehla: poori kitaab ka tarjuma pehle karwa lo.** Waqt lagega,
lekin uske baad har English reader seedha padhega, poori raftaar
se. Aur translator poori kitaab dekhta hai, toh galtiyan pehle hi
pakdi jaayengi, chhapne se pehle.

**Doosra: reader ke saath ek dubhashiya baitha do.** Shuru turant
ho jaayega, ek line suno, ek line bolo. Lekin har baar padhne pe
tarjuma phir se hoga, toh raftaar kam. Aur galti tabhi pakdegi
jab woh line aayegi, beech kitaab mein bhi atak sakte ho.

Code ke bhi yahi do raaste hain:

**Compiler** = poora tarjuma pehle. Code ek baar machine code mein
badla, ab woh file seedha CPU pe bhaagti hai. Tez. Games, browsers,
operating systems aise bante hain (bhaashaein: C, C++, Rust).

**Interpreter** = saath baitha dubhashiya. Likho aur turant chalao,
badlo aur phir chalao. Aaraam hai, lekin chalte waqt har line ka
tarjuma hota hai, toh dheema (10-100 guna tak). Python aisa hai.

Toh sauda saaf hai: **compiler = mehnat pehle, raftaar baad mein.
Interpreter = aaraam pehle, raftaar ki keemat baad mein.** Kaunsa
sahi? Galat sawal. KIS KAAM ke liye, yeh poochho. Game ko raftaar
chahiye: compiler. Roz badalne wala chhota kaam: interpreter.
(Duniya mein beech ke raaste bhi hain, Java aur JavaScript aadha
pehle aadha chalte-waqt tarjuma karte hain, lekin idea yehi do
hain.)

## NAAM

**Compiler** (poora pehle), **interpreter** (line-by-line).
Compiled code ki tayyar file ko log **binary** ya **executable**
kehte hain: .exe wali file wahi hai, tarjuma ho chuki recipe.

## ASLI DUNIYA SE EK EXAMPLE

Android phone pe kabhi update ke baad likha aata hai "Optimising
apps 1 of 132..." Woh yahi hai: phone apps ka tarjuma apne CPU ke
liye pehle se kar raha hai, taaki baad mein har app tez khule.
Aapne compiler ko kaam karte hue dekha hai, bas naam nahi pata
tha.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Python dheemi hai toh AI jaise bhaari kaam Python mein kyun hote
hain?" Chaal yeh hai: Python sirf STEERING hai. AI ka asli bhaari
hisaab (numbers ka guna, arabon baar) compiled code mein likha
hai (C/C++ ki libraries), Python bas use bulaata hai. Dheemi
bhasha se tez engine chalaya ja raha hai. Abstraction phir se:
aaraam upar, raftaar neeche, dono ek saath.

## MAP PE

Rupaye ka rasta: server pe har second ka CPU kiraya lagta hai
(Part 5 mein poora hisaab). Dheema code = zyada seconds = bada
bill. Isliye companies jab badi hoti hain, toh apne sabse zyada
chalne wale hisse compiled bhaashaon mein DOBARA likhti hain,
sirf bill ghatane ko. Founder ke liye sabak: shuru mein aaraam
wali bhasha (raftaar se pehle zinda rehna zaroori hai), scale pe
raftaar wali. Galat waqt pe galat chunaav, dono taraf mehnga hai.

## KHUD DEKHO (5 minute)

Apne phone/laptop mein files mein jhaanko: .exe ya .apk file
(compiled, tarjuma ho chuki, kholo toh ajeeb aksharon ka kachra
dikhega kyunki woh machine code hai) vs koi .txt ya website ka
source (insaan ke padhne laayak). Do duniyaon ka farq apni aankh
se dekh lo: ek insaan ke liye likhi gayi, ek CPU ke liye.

## SOCHNE KE LIYE

1. (derivation) Compiler galtiyan pehle pakadta hai, interpreter
chalte waqt. Bank ka core system kis se banna chahiye, aur ek
naya idea jo har hafte badal raha hai woh kis se? Wajah bhi do.

> **Jawab:** Bank: compiler wali bhasha. Wahan galti chalne ke
> BAAD milna crores ka ho sakta hai; pehle pakadna hi bachav hai,
> aur raftaar bhi chahiye. Naya idea: interpreter wali. Wahan
> sabse bada khatra dheema code nahi, DHEEMA SEEKHNA hai: har
> hafte badlav karna hai, turant chala ke dekhna hai. Sauda
> hamesha wahi hai: galti ki keemat vs badlav ki raftaar. Yeh
> ek line kisi bhi tech decision pe lagao, aadha jawab mil
> jaayega.
