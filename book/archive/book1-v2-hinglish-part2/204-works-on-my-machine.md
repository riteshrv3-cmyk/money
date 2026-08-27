# Chapter 4.4 [DEPTH]: "Mere machine pe toh chal raha tha"

(DEPTH chapter. Yeh line software ki duniya ka sabse purana
mazaak hai. Iske peeche ka sach samajh loge toh "deploy" aur
"DevOps" jaise bhaari shabd halke ho jaayenge.)

Scene: engineer ne feature banaya, apne laptop pe sau baar
chalaya, sab perfect. Server pe daala: crash. User ke phone
pe: khali screen. Engineer ki pehli line: "mere machine pe
toh chal raha tha..."

Woh jhooth nahi bol raha. Toh galti kahan hai?

Chapter 3.5 se socho. Recipe kabhi akeli nahi chalti: woh OS
se maangti hai, doosri recipes (libraries) ko bulaati hai,
settings padhti hai, files dhoondhti hai. Matlab recipe ke
aas paas ek poora MAAHAUL hai jis pe woh tiki hai:

```
code khud            (yeh toh dono jagah same tha)
+ OS aur uska version     (laptop: Windows 11; server: Linux)
+ libraries ke versions   (laptop pe nayi, server pe purani)
+ settings, passwords     (laptop pe test wale, server pe asli)
+ doosri services         (laptop pe nakli bank; server pe asli)
```

Code same, maahaul alag = alag natija. "Chal raha tha" ka
poora sach hai: "MERE maahaul mein chal raha tha."

Toh ilaaj khud soch lo: maahaul ko bhi code jaisa bana do.
Likh do ki is recipe ko kya kya chahiye (OS, libraries ke
EXACT versions, settings), aur aisa intezaam karo ki har
jagah, laptop se server tak, WAHI maahaul ban jaaye. Recipe
ke saath poora kitchen hi pack kar do.

Yeh intezaam bana: pehle list-waali files (requirements),
phir poora packed-kitchen: container. Ek dibba jisme code +
uska maahaul saath band hai; dibba jahan bhi khulega, andar
ki duniya same hogi. Ship ke container se hi naam liya gaya:
saamaan koi bhi ho, dibba ek jaisa, isliye har port ka crane
use utha leta hai.

## NAAM

Recipe ke aas paas ki poori duniya: **environment**. Packed
kitchen wala dibba: **container**, sabse mashhoor auzaar:
**Docker**. Code ko laptop se asli server tak pahunchana:
**deploy**. Aur yeh sab intezaam sambhaalne ka pesha:
**DevOps**.

## ASLI DUNIYA SE EK EXAMPLE

Aapke ghar ki dal har baar perfect banti hai. Wahi recipe
mausi ke ghar banao: cooker alag, aanch alag, namak ka
dabba alag. Swad badla. Recipe jhooth nahi boli, kitchen
badla tha. Ab restaurant chains ka raaz dekho: McDonald's
har jagah ek jaisa isliye hai kyunki unhone KITCHEN ko
standard kiya, sirf recipe ko nahi. Docker software ka
McDonald's-kitchen hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Software = code ki file. File bhej di, kaam khatam." Ab aap
jaante ho: software = code + maahaul. Isliye "app bana di,
ab live karna toh bas ek button hoga na" founder ka sabse
mehnga bhram hai. Deploy apna poora kaam hai: maahaul
banana, jaanchna, purane version se naye pe bina rukawat
jaana, galti pe wapas aana. Estimate mein iska waqt alag se
poochho, warna "ho gaya" aur "chal raha hai" ke beech ke
hafte aapko surprise karenge.

## MAP PE

Rupaye ka rasta: yeh dard itna asli hai ki iske ilaaj ki
companies arabon ki hain. Docker ne dibba diya; phir sawal
aaya "hazaar dibbon ko kaun sambhaale" toh Google ne
Kubernetes khola (open source: Chapter 3.7 ki chaal, taaki
sab uske cloud ke tareeke pe aa jaayein); aur cloud
companies (Part 5) ka aadha business hi yeh hai: "maahaul
ka jhanjhat humein do, kiraya do." Jahan har team ka dard
ek jaisa ho, wahan platform banta hai, aur platform lagaan
wasoolta hai. Dard dhoondho, dukan wahin kholo.

## KHUD DEKHO (5 minute)

Play Store/App Store mein kisi app ka page kholo, neeche
"Requires Android 12+" ya "Requires iOS 16+" dhoondho. Yeh
environment ki sabse seedhi shakal hai: app keh rahi hai
"mera kitchen kam se kam itna naya ho." Ab samajh aayega
purane phone pe nayi app kyun nahi chalti: code nahi,
maahaul chhota pad gaya.

## SOCHNE KE LIYE

1. (derivation) Do dost, bilkul same phone model, same app
version. Ek ke phone pe app roz crash, doosre pe kabhi
nahi. Code same, phone same. Ab kya alag ho sakta hai?
Kam se kam teen cheezein ginno.

> **Jawab:** Maahaul ab bhi alag hai: (1) OS ka chhota
> version/update alag ho sakta hai, (2) ek ka storage
> lagbhag full hai (likhne ki jagah nahi = ajeeb crashes),
> (3) permissions alag (ek ne location mana kiya, app ka
> woh raasta kabhi test nahi hua tha), (4) bhasha/region
> setting alag (date ka format alag = parse error), (5)
> background apps aur battery-saver alag. Sabak: "same
> phone" kabhi same nahi hota. Isliye bade apps hazaaron
> asli devices pe test hote hain, aur phir bhi Chapter
> 4.1 ka niyam lagta hai: koi na koi jod chhoot hi jaata
> hai.
