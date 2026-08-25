# Chapter 4.3 [SPINE]: Har badlav ka record

Aapne kabhi aisi files dekhi hain? `project_final.docx`,
`project_final_v2.docx`, `project_FINAL_really.docx`. Hasi aati
hai, lekin yeh ek asli problem ka kachcha ilaaj hai: cheez
badalti rehti hai, aur hume purane roop chahiye hote hain.

Ab software ki duniya mein yeh problem raakshas ban jaati hai.
Code roz badalta hai. Das (ya das hazaar) log EK HI code pe
kaam kar rahe hain. Kal wala version chalta tha, aaj toota hai:
KISNE, KYA, KYUN badla? Aur do logon ne ek hi file ek saath
badal di toh kiska badlav rahe?

Khud intezaam design karo. Kya kya chahiye?

1. Har badlav ki photo: kya badla, kisne, kab, aur KYUN (ek
line ka note).
2. Kisi bhi purani photo pe wapas jaane ka button.
3. Ek saath kaam: main apni alag copy pe naya feature banaun,
tum apni pe bug theek karo, aur baad mein dono ka jod ban
jaaye.

Yeh intezaam bana hua hai, naam hai Git (2005, wahi aadmi jisne
Linux banaya, apne hi kaam ke liye banaya tha). Uski bhasha
teen shabdon mein:

**Commit** = badlav ki photo + note. "Payment ka bug theek
kiya" likh ke photo le li. History mein hamesha ke liye.

**Branch** = apni alag copy jahan aap bina kisi ko chhede
prayog karo. Main branch (asli) safe rehti hai.

**Merge** = branch ka kaam wapas asli mein jodna. Do logon ne
ek hi line badli ho toh Git rok ke poochhta hai: kaunsi rakhein?

Aur GitHub? Woh in sab ka adda hai: internet pe rakhi hui
saanjhi history, jahan duniya bhar ki teams (aur open source
ka poora sansaar) apna code rakhti hain.

Ek baat dhyaan se: yeh sirf "backup" nahi hai. Yeh HIMMAT ka
intezaam hai. Jab har badlav wapas ho sakta hai, toh prayog
karne ka darr khatam ho jaata hai. Bina Git ke engineer
chhoone se darta hai ("kahin tod na dun"); Git ke saath woh
todta hai, seekhta hai, wapas laata hai. Raftaar ka asli
raaz safety net hai.

## NAAM

Is poore intezaam ka naam **version control** hai, auzaar ka
naam **Git**, adde ka naam **GitHub** (ya GitLab). Do badlaavon
ka takraav: **merge conflict**.

## ASLI DUNIYA SE EK EXAMPLE

Sabse nazdeeki example aap khud ho: YEH KITAAB ek Git repo
mein ban rahi hai. Har chapter ka har badlav commit hai, note
ke saath. Purana version 1 poora ka poora archive mein zinda
hai, ek command pe wapas aa sakta hai. Jo intezaam Microsoft
aur Google ke das hazaar engineers ko sambhaalta hai, wahi
aapki kitaab ko sambhaal raha hai, muft. (Chapter 3.7:
auzaar sab ke liye ek jaisa muft hai. Farq istemaal mein hai.)

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Yeh engineers ka andaruni auzaar hai, founder ko kya." Galat.
GitHub kisi engineer ya team ka X-ray hai. Wahan dikhta hai:
kaam kitna regular hai (commits), notes kitne saaf hain, kitne
log sach mein kaam kar rahe hain. Aur jab aap AI se code
banwaoge (aaj ke tools seedha Git ke saath chalte hain), toh
commit history hi aapka hisaab-kitaab hai: kya banwaya, kab,
kis note ke saath. Register padhna aana chahiye, chahe likhe
koi aur.

## MAP PE

Company case: Microsoft ne 2018 mein GitHub ko 7.5 arab
dollar mein khareeda. Kyun itna, ek "code rakhne ki jagah" ke
liye? Kyunki wahan duniya ke engineers ka kaam, aadatein aur
aane wale projects dikhte hain: yeh developers ka darwaza hai
(Chapter 3.5 ki bhasha mein: platform). Aur ab dekho: usi
GitHub ke upar Microsoft ne AI coding tools bechne shuru kiye.
Darwaza pehle, dukan baad mein. Pattern har baar wahi hai.

## KHUD DEKHO (5 minute)

github.com kholo (bina account ke chalega). Search mein
"linux" likho, pehla result kholo. Aap duniya ke sabse
zaroori software ka asli code dekh rahe ho. "Commits" pe
click karo: lakhon badlaavon ki history, har ek pe naam,
taareekh, note. Sabse naya commit shayad kal ka hoga. Yeh
30 saal se roz badal raha hai aur kabhi toota nahi: yehi
version control ki taakat hai.

## SOCHNE KE LIYE

1. (derivation) Akela aadmi kaam kar raha hai, koi team
nahi. Use branch/merge ki kya zaroorat? (Socho: himmat wali
baat yahan kaise lagti hai.)

> **Jawab:** Zaroorat wahi hai, roop chhota hai. Branch uska
> prayogshaala hai: "naya design try karta hoon" wali copy,
> jisme fail hona muft hai, asli cheez surakshit hai. Aur
> history uska doosra dimaag hai: chhe mahine baad "yeh
> ajeeb line kyun likhi thi" ka jawab commit note mein
> milta hai. Akele aadmi ke paas toh poochhne ko koi doosra
> hai hi nahi, isliye use record ki zaroorat team se ZYADA
> hai. (Aapka second-brain repo bhi yahi hai: badalti soch
> ka version control.)
