# Chapter 3.5 [SPINE]: Woh manager jo machine baantta hai

Abhi aapke phone pe kya kya chal raha hai? WhatsApp, gaana,
background mein email check, screen ka touch, network ki sunwai.
Lekin Part 1 se aap jaante ho: CPU ek waqt mein EK recipe ka EK
kadam chalata hai. Toh yeh sab EK SAATH kaise?

Aur ek gehri dikkat bhi hai. Chapter 2.4 ke sawal mein dikha tha:
agar ek recipe doosri recipe ki memory mein likh de toh? Sau
recipes, ek mez (RAM), koi rok-tok nahi: ek kharab app poore
phone ko gira degi.

Toh khud design karo. Aapke paas ek tez CPU hai aur sau recipes
hain jo chalna chahti hain. Kya karoge?

**Baari baantoh.** Har recipe ko thoda sa waqt do: 10 millisecond
WhatsApp, 10 gaane ko, 10 screen ko, phir wapas. CPU itna tez hai
(arab kadam/second) ki har recipe ko lagta hai machine sirf uski
hai. "Ek saath" ek bhram hai, asal mein bijli-tez baari-baari hai.

**Deewarein banao.** Har recipe ko mez ka apna hissa do, aur
niyam: apne hisse ke bahar haath dala toh wahin maar do (yehi
"app crash" hai). Ek app mare, baaki bache.

**Saajha cheezon ka darbaan bano.** Screen ek hai, speaker ek,
network ek, storage ek. Recipes ko seedha haath nahi lagane
denge; woh darkhaast karengi, darbaan karega. Files ka intezaam
bhi yahi darbaan rakhta hai.

Ab dekho aapne kya banaya: ek MALIK recipe, jo baaki sab recipes
ke upar baithti hai, waqt baantti hai, deewarein rakhti hai,
darbaani karti hai. Yeh operating system hai. Windows, Android,
iOS, Linux: yehi chaar naam duniya ki lagbhag har machine ke
malik hain.

Aur ab woh baat jo iski asli taakat hai: app likhne wala screen,
touch, network, file, KUCH bhi seedha nahi chhoota. Woh sirf OS
se maangta hai. Matlab app OS KE LIYE likhi jaati hai, machine ke
liye nahi. Isi liye iPhone wali app Android pe nahi chalti: machine
lagbhag same hai, MALIK alag hai, aur app malik ki bhasha mein
likhi thi.

## NAAM

Malik recipe: **operating system (OS)**. Chalti hui recipe ki
baari ka intezaam: **scheduling**. Har hardware se baat karne
wala OS ka tukda: **driver**. Files ka intezaam: **file system**.
Aur app jo OS se maangti hai, us maangne ke tay tareeke ka naam
agle chapters mein bada hoga: yehi "API" ka pehla roop hai.

## ASLI DUNIYA SE EK EXAMPLE

Ek dhaba socho jisme ek hi chulha hai aur das cooks. Bina
manager: jhagda, jala khaana, afra-tafri. Manager aake kya
karta hai: chulhe ki baari baantta hai, har cook ka apna
saamaan-shelf tay karta hai, aur bhandar ki chaabi apne paas
rakhta hai. Dhaba wahi, chulha wahi, lekin ab sau order nikalte
hain. OS bilkul yahi manager hai, aur "phone hang" us din hota
hai jab manager khud thak jaaye.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Android/iOS bas phone ka brand-type hai." Nahi, woh malik hai,
aur malik hona duniya ka sabse bada business-pad hai. Jo OS ka
malik hai, woh tay karta hai ki us machine pe kaun sa app aayega,
kaise aayega, aur (asli baat) PAISE ka kitna hissa raste mein
katega. Apple har app ki kamai ka 15-30% leta hai, sirf darwaze
ka malik hone ke naate. Is pad ka naam platform hai, aur platform
ka malik hamesha apne upar bane business se zyada sukoon se
kamata hai.

## MAP PE

Chain dekho: aap 100 rupaye ka in-app purchase karte ho (Level 1
se paisa ghusa). App wale ko ~70-85 mile, Apple/Google ne 15-30
raste mein liye (platform tax). App wala apne cloud aur tools
walon ko deta hai. OS ka malik har transaction mein baitha hai,
bina woh app banaye. Isliye companies OS/platform ki jang ladti
hain marte dum tak: Microsoft (Windows), Google (Android muft
baanta, taaki malik bane), Apple. Jo darwaza jeet gaya, woh
lagaan wasoolta hai.

## KHUD DEKHO (5 minute)

Phone ki Settings kholo, Battery dekho: kaunsi app ne kitna
khaya. Phir Apps mein jaake kisi app ki "Permissions" dekho:
camera, location, contacts. Yeh dono panne OS ke manager-register
hain: kisko kitni baari mili, kisko kaunsi chaabi. Malik ka
hisaab-kitaab aap khud padh sakte ho.

## SOCHNE KE LIYE

1. (derivation) Google Android ko muft kyun baantta hai, jabki
usko banane pe arabon lagte hain? (Chapter 0.1 ki soch lagao:
paisa kahan ghusta hai, kahan behta hai.)

> **Jawab:** Kyunki Android bech ke kamaana chhota khel tha,
> MALIK banna bada. Muft OS se duniya ke 70% phone Google ke
> darwaze ban gaye: unki search, unka Play Store (15-30% tax),
> unke ads, unka data. Ek baar banao, arabon phones pe chale,
> har phone kamaai ka rasta: leverage ka poora dial. Sabak
> founder ke liye: kabhi kabhi product muft dena hi sabse bada
> business hota hai, AGAR muft cheez aapko darwaze ka malik
> banati ho. (Muft ka poora khel Chapter 3.7 mein.)
