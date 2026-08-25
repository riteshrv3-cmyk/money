# Chapter 3.2 [SPINE]: Near-English mein likhna

Ab woh cheez saamne dekh lo jisse duniya itna darti hai: code. Yeh
raha ek poora, asli program (Python bhasha):

```
price = 300

if price > 500:
    print("mehnga hai")
else:
    print("theek hai")
```

Padho. Aap ise LAGBHAG waise hi padh sakte ho jaise English:
"price naam ke dibbe mein 300 rakho. Agar price 500 se bada hai,
toh 'mehnga hai' dikhao, warna 'theek hai' dikhao." Chalaoge toh
screen pe aayega: theek hai.

Bas. Yeh coding hai. Na maths ka pahad, na jaadu. Strict grammar
mein likhi recipe.

Ab ek baat jo coding ke bahar ke logon ko koi nahi batata: **har
program, WhatsApp se le kar ChatGPT tak, sirf TEEN cheezon se bana
hai:**

**1. Rakho:** naam wale dibbe mein value rakhna (`price = 300`).
Dibba wahi RAM ka mez hai (Chapter 2.5), naam insaan ki suvidha ke
liye hai.

**2. Poochho:** shart pe raasta chunna (`if ... else ...`). Yeh
wahi "agar" hai jo gates se bana tha (Chapter 1.5), bas ab insaan
ki shakal mein.

**3. Dohraao:** ek kaam baar baar karna (loop):

```
for customer in customer_list:
    bill = bill_nikaalo(customer)
    print(bill)
```

"Har customer ke liye: bill nikaalo, dikhao." Chahe list mein teen
hon ya teen crore, recipe wahi teen lines. YAHI woh jagah hai jahan
leverage code mein ghusta hai: insaan teen crore baar nahi kar
sakta, loop kar leta hai.

Rakho, poochho, dohraao. Agli baar koi bhi software dekho, khud se
poochho: ismein kya rakha ja raha hai, kya poochha ja raha hai,
kya dohraaya ja raha hai. Instagram feed: posts ki list pe loop,
har post pe "is user ko dikhana banta hai?" wala if, aur dekhe hue
posts ka hisaab dibbon mein. Poora app teen cheezon ka jaal.

## NAAM

Likhi hui recipe: **code**. Naam wala dibba: **variable**. Shart:
**condition** (if/else). Dohraana: **loop**. Strict grammar ka
naam: **syntax**. Grammar ki galti: **syntax error**, translator
usi waqt pakad leta hai.

## ASLI DUNIYA SE EK EXAMPLE

Aapka bank har mahine ki 1 taareekh ko lakhon khaaton pe interest
daalta hai. Andar kya hai? Ek loop ("har khaate ke liye"), ek
condition ("agar savings account hai"), aur kuch variables (rate,
balance, dinon ki ginti). Jo clerk 1960 mein mahina lagata tha
(Chapter 1.3), woh aaj 20 lines ka loop hai jo raat ko chalta hai.
Duniya ke sabse bade business-software ka pet aise hi seedhe
loops se bhara hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Coding ke liye maths genius chahiye." Aapne abhi ek program padha
aur ek ka andaza lagaya, bina kisi maths ke. Aam software mein
jod-ghata se zyada maths hota hi nahi. Asli skill maths nahi,
SAAF SOCHNA hai: kaam ko itne chhote, exact kadmon mein todna ki
ek bewakoof lekin bijli-tez naukar (machine) unhe kar sake. Jo
aadmi business process saaf soch sakta hai, woh coding ki soch
pehle se jaanta hai, use sirf grammar nahi aati.

## MAP PE

Rupaye ka rasta: duniya mein ~3 crore log code likh ke kamaate
hain. Lekin ab asli baat: AI ke baad grammar SASTI ho rahi hai
(Claude grammar jaanta hai), aur saaf sochna MEHNGA ho raha hai.
Jo aadmi jaanta hai KYA banwana hai aur use exact kadmon mein tod
sakta hai, woh ab bina grammar seekhe bhi banwa sakta hai. Aapki
is kitaab ki poori bet isi line pe hai.

## KHUD DEKHO (5 minute)

Upar wale pehle program mein 300 ko 800 kar do (dimaag mein).
Ab kya chhapega? Ab 500 ko 800 karo, price 800 hi rahe. Ab kya?
(Dhyaan: "bada hai" ka sawal hai, barabar ka nahi.) Agar dono ka
jawab aapne bina atke de diya (pehla: mehnga hai; doosra: theek
hai, kyunki 800 > 800 jhooth hai), toh aapne aaj code trace kiya,
yehi debugging ki pehli skill hai.

## SOCHNE KE LIYE

1. (derivation) Ek bracket ya comma chhootne se poora program kyun
ruk jaata hai? Insaan toh aadhi galat spelling waali chitthi bhi
padh leta hai.

> **Jawab:** Insaan matlab ka andaza laga leta hai kyunki uske
> paas duniya ki samajh hai. Translator ke paas sirf grammar ke
> niyam hain; bracket ke bina use pata hi nahi chalta ki "poochho"
> kahan khatam hua aur "karo" kahan shuru. Aur GUESS karna
> jaan-boojh ke nahi rakha gaya: bank ke code mein translator ka
> galat guess crores ka ho sakta hai. Behtar hai wahin rok do,
> insaan se poochho. Strict grammar sazaa nahi hai, woh EXACTNESS
> ki keemat hai, aur exactness hi woh cheez hai jiske liye
> machine pe bharosa kiya ja sakta hai.
