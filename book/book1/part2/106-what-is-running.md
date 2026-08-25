# Chapter 3.6 [DEPTH]: "Running" ka matlab kya hai

(DEPTH chapter. Chhota hai. Iske baad "app band karo, process
maro, restart karo" wali har baat ka asli matlab dikhne lagega.)

Ek sawal jo seedha lagta hai lekin nahi hai: WhatsApp aapke phone
mein "hai" ka matlab kya hai? Do bilkul alag cheezein hain:

**Recipe ki file.** Storage (pakki almaari) mein padi hai, ~100
MB. Soyi hui. Bijli jaaye, kuch nahi bigadta. Yeh APP hai.

**Chalti hui copy.** Jab aapne icon dabaya, OS ne recipe ko RAM
ke mez pe utara, uska program counter set kiya, use baari dena
shuru kiya. Ab woh ZINDA hai: uski apni memory, uski abhi ki
haalat (kaunsi chat khuli hai, kahan tak scroll kiya). Yeh
PROCESS hai.

Ek recipe, kai copies bhi ho sakti hain: laptop pe do browser
windows = ek program, do process, har ek apni haalat ke saath.
Do alag tabs mein do alag email khaate khule hain: recipe
saajha, zindagi alag.

Ab roz ki bhasha is naye chashme se padho:

**"App kholna"** = process janamna (almaari se mez pe).
**"App not responding"** = process zinda hai lekin kisi kaam mein
atka hai, baari mil rahi hai par jawab nahi de raha.
**"Force stop"** = OS process ko maar deta hai. File salaamat.
**"Restart karo, theek ho jaayega"** = purani uljhi haalat wali
process mari, nayi saaf haalat se janmi. Isliye restart itni
beemariyan theek karta hai: beemari HAALAT mein thi, file mein
nahi.
**"Background apps"** = process zinda hai lekin screen pe nahi;
OS use kam baari deta hai, ya soola deta hai.

## NAAM

Chalti hui copy: **process**. Uski abhi ki poori haalat (memory
+ counter + khuli cheezein): **state**. Yeh shabd bahut bada
hai; aage database (Part 4) aur AI (Book 2) mein "state" baar
baar aayega. Aur ek process ke andar ki chhoti baari-lene wali
dhaaraon ka naam **thread** hai (itna hi kaafi hai abhi).

## ASLI DUNIYA SE EK EXAMPLE

Cyber cafe ya kisi saajha computer pe do log alag alag Gmail
khol lete hain, do browser windows mein. Recipe (browser) ek hi
thi. Lekin har process apna state rakhta hai, isliye do
zindagiyan ek machine pe bina mile chal jaati hain. Poora cloud
business (Part 5) isi baat pe khada hai: EK machine pe HAZAARON
alag processes, har ek apni deewar mein, har ek kisi aur ka
kaam karti hui.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Maine app band ki, matlab phone se hat gayi." Ulta bhi: "app
delete ki, matlab uska sab kuch gaya." Dono galat, kyunki log
FILE aur PROCESS ko ek samajhte hain. Band karna process ka ant
hai, file rahi. Delete karna file ka ant hai, lekin app ka data
(chats, settings) aksar alag jagah hai, aur cloud pe bhi. Do
naam alag rakho, aadhi confusion khatam.

## MAP PE

Rupaye ka rasta: cloud mein aap PROCESS ke waqt ka kiraya dete
ho. "Serverless" naam ki cheez mein toh hisaab hi yehi hai:
aapka code jitne millisecond process bana raha, utna paisa.
Process = meter chalu, process khatam = meter band. Jab Part 5
mein cloud ka bill padhoge, toh har line ke peeche yehi sawal
hoga: kitni processes, kitni der, kitne mez (RAM) ke saath.

## KHUD DEKHO (5 minute)

Phone pe recent apps ka button dabao (ya laptop pe Task Manager
kholo: Ctrl+Shift+Esc). Yeh zinda processes ki list hai. Kisi
app ko swipe karke maar do, phir dobara kholo: thoda dheere
khuli na, aur pichhli jagah pe nahi? Aapne ek process ka poora
janam-mrityu chakra khud chalaya: state gayi, file se naya
janam hua.

## SOCHNE KE LIYE

1. (derivation) Game beech mein band ho gaya (process mara).
Wapas khola toh score wahi ka wahi mila. State toh mar gayi
thi, score kaise bacha? Part 1 ke kis chapter ka intezaam hai
yeh?

> **Jawab:** Game ne marne se pehle score storage mein likh
> diya tha (save), yaani tez-bhulakkad RAM se dheemi-pakki
> almaari mein (Chapter 2.5). Process ki state hamesha maranshil
> hai; jo bachana ho use pakki jagah likhna hi ekmatra rasta
> hai. Isi ek kaam ka bada roop DATABASE hai, jo Part 4 ka
> mukhya kirdaar hai: state ko aisi jagah rakhna jahan process
> ke marne se, machine ke jalne se, kuch na bigde.
