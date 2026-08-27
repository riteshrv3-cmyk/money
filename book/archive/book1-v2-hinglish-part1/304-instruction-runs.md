# Chapter 2.4 [DEPTH]: Ek instruction chalti kaise hai

(DEPTH chapter. Skip kar sakte ho, lekin yeh chhota hai aur iske baad
"processor" shabd hamesha ke liye khul jaata hai.)

Chapter 1.6 se: recipe numbers ban kar memory mein rakhi hai. Machine
use chalati kaise hai? Poora raaz ek ginne wale khaane mein hai.

CPU ke andar ek chhota sa khaana hai jisme bas ek number rehta hai:
**"abhi main recipe ke kadam number ___ pe hoon."** Aur CPU din raat
bas yeh teen kaam gol gol karta hai:

**1. UTHAO (fetch):** khaane mein jo number hai, memory ki us jagah
se kadam utha lo. Maan lo wahan likha hai: "3" (matlab: jodo).

**2. SAMJHO (decode):** number 3 ka matlab kya hai? Chapter 1.5 wali
gates ki chain number ko padh kar sahi purza chuun leti hai: jodne
wala dibba on.

**3. KARO (execute):** jod do. Jawab kisi khaane mein rakho. Aur
ginne wale khaane mein 1 badha do, taaki agla phera agla kadam uthaye.

Bas. Yeh teen kadam ka chakkar hi "computer chal raha hai" ka poora
matlab hai. Aapke phone mein yeh chakkar ek second mein ~3 arab baar
ghoomta hai.

Ek sawal khud se poochho: "agar aisa toh wahan jao" wala kadam kaise
chalega? Aasaan: woh kadam bas ginne wale khaane mein NAYA number
likh deta hai. Ab agla fetch wahin se uthega. Recipe ne chhalaang
maar li. Loop bhi yahi hai: peechhe wale number pe chhalaang, baar
baar. Programming ka poora control isi ek khaane se hota hai.

Ab "3 GHz processor" ka matlab bhi le lo: GHz = giga hertz = arab
phere prati second. 3 GHz matlab yeh chakkar 3 arab baar prati
second. Yeh hi woh "arab kadam" hai jo kitaab mein baar baar aaya.

## NAAM

Ginne wale khaane ka naam **program counter** hai. Teen kadam ke
chakkar ka naam **fetch-decode-execute cycle**. Chakkar ki raftaar ka
naam **clock speed** (GHz mein). Kadmon ke numbers wali poori bhasha
ka naam **machine code**: yehi ek bhasha hai jo CPU sach mein samajhta
hai. (Insaan iski jagah aaraam wali bhaashaein likhta hai; unka
tarjuma Part 2 ka mukhya kissa hai.)

## ASLI DUNIYA SE EK EXAMPLE

Phone kabhi "hang" hota hai. Ab aap bata sakte ho andar kya hua:
program counter kisi aisi jagah phas gaya jahan recipe gol gol ghoom
rahi hai aur bahar aane ki shart kabhi sach nahi ho rahi (infinite
loop), ya kisi aise number pe chala gaya jahan recipe thi hi nahi.
Machine kharab nahi hui, recipe ne use gadhe mein ghuma diya. Restart
kya karta hai? Program counter samet sab kuch shuruaati jagah pe wapas.
Isliye restart itni beemariyan theek karta hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Zyada GHz = tez computer," bas itna. Adhoora hai. GHz sirf chakkar
ki raftaar hai; kaam kitna hua yeh is pe bhi hai ki har phere mein
kitna hota hai, kadam kitne samajhdaar hain, aur memory kitni tez
kadam pakda rahi hai (agla chapter). Do processor same GHz pe do guna
alag kaam kar sakte hain. Dukaandaar aapko ek number bech raha hai,
machine kai numbers ka khel hai.

## MAP PE

Rupaye ka rasta: Apple apne chips khud design karta hai (M-series)
taaki har phere mein zyada kaam ho. Behtar cycle = kam battery mein
zyada kaam = mehngi machine bikti hai. Ek chakkar jo aapne abhi 10
minute mein samjha, uski bareeki pe duniya ki sabse keemti company ka
margin tika hai. Level 3 ke andar bhi levels hain, aur neeche wala
jitna behtar, upar sab utna behtar.

## KHUD DEKHO (5 minute)

Yeh recipe kaagaz pe chalao, aap khud CPU bano. Khaana K mein 5 hai.
Recipe: kadam 1: K mein 3 jodo. kadam 2: agar K < 15, kadam 1 pe
jao. kadam 3: ruko. Ungli se program counter banao aur chalao. Kitne
phere lage? (K: 5, 8, 11, 14, 17 -> 4 jod, phir shart fail, ruk
gaye.) Aapne abhi fetch-decode-execute aur loop dono chala liye.

## SOCHNE KE LIYE

1. (derivation) Program counter mein galat number aa jaaye, aisi
jagah ka jahan recipe nahi, kachra numbers hain. CPU kya karega?
Usko kaise pata chalega ki yeh "recipe nahi" hai?

> **Jawab:** Nahi pata chalega, yahi darr ki baat hai. CPU ke liye
> har number kadam jaisa hi dikhta hai, woh kachre ko bhi decode
> karke chalane ki koshish karega. Kabhi bekaar kaam hoga, kabhi
> crash. Isliye aas paas ke intezaam (operating system, Part 2)
> deewarein banate hain: kaunsi recipe kahan chal sakti hai, kaunsi
> memory chhoo sakti hai. Aur hackers ka aadha khel hi yeh hai:
> kisi tarah apne numbers program counter tak pahunchana. Ek
> chhota khaana, poori security ki jang ka maidan.
