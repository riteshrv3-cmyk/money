# Chapter 2.3 [SPINE]: Bade numbers ka matlab

Is kitaab mein ab tak aaye: 15 arab transistor, 44,000 sample prati
second, arab kadam prati second. Aage aur bade aayenge. Problem yeh
hai ki insaan ka dimaag lakh ke aage sab numbers ko ek jaisa "bahut
bada" maan leta hai. Woh chalega nahi, kyunki in numbers ke beech ke
FARQ mein hi saari samajh aur saara paisa hai.

Pehle tarjuma ka table, kyunki India ginti apni bolta hai aur
technology angrezi:

```
10 lakh     = 1 million   (M)
1 crore     = 10 million
1 arab      = 1 billion   (B)  = 100 crore
1 kharab    = 100 billion
            = 0.1 trillion (T)
```

Ab farq ko mehsoos karo, ghadi se. Ek second mein ek ginti bolo:

```
1 million tak ginne mein    ~ 11 din lagenge
1 billion tak               ~ 31 SAAL
1 trillion tak              ~ 31,000 saal
```

Million aur billion "paas paas" nahi hain. Unke beech hazaar guna ka
samundar hai. Jab news kahe "company X billion dollar ki hui," toh
ab aapke paas paimana hai.

Ab ulti taraf, chhote waqt ki ginti, kyunki machine wahan jeeti hai:

```
1 second        aapka ek palak jhapakna
1 millisecond   (1/1000 sec)    achhe internet ka ek phera
1 microsecond   (1/10 lakh)     machine memory se ek cheez uthana
1 nanosecond    (1/1 arab)      CPU ka ek kadam
```

Ek moti baat nikaalo: **CPU ke ek kadam (nanosecond) aur internet ke
ek phere (millisecond) mein 10 lakh guna ka farq hai.** Matlab jab
tak ek message shehar paar jaa kar lautta hai, CPU 10 lakh kadam chal
chuka hota hai. Machine ke andar sab kuch muft jaisa tez hai; bahar
jaana mehnga hai. Yeh ek line aage Part 3, 4, 5 mein baar baar kaam
aayegi, aur engineers ke har design ke peeche yahi hai: **bahar mat
jao jab tak zaroori na ho.**

## NAAM

In chhote naapon ke naam upar table mein hain: milli (hazaarvan),
micro (10 lakhvan), nano (arabvan). Speed ke is khel ka naam
**latency** hai: ek kaam shuru hone se jawab aane tak ka waqt. Yeh
shabd Part 5 mein poora chapter layega.

## ASLI DUNIYA SE EK EXAMPLE

Google ne naapa ki search 400 millisecond dheemi hui toh log kam
search karne lage. Aadha palak jhapakne se kam waqt, aur karodon ka
farq. Amazon ki ginti: har 100 millisecond ki deri = ~1% kam bikri.
Isliye speed engineering ki shauk nahi, seedha paisa hai. Jo company
millisecond gin sakti hai, woh unhe rupaye mein badal sakti hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Computer tez hai, bas." Nahi: computer KAHAN tez hai, yeh jaanna hi
asli gyaan hai. Andar nanosecond, bahar millisecond, 10 lakh ka farq.
Jo yeh nahi jaanta, woh aisa product sochta hai jo har kadam pe
internet se poochhta hai, aur phir hairaan hota hai ki sab dheema
kyun hai. Tez machine pe bhi dheema design possible hai, aur aam hai.

## MAP PE

Kaun kamata hai is chapter se: jo scale ko padh sakta hai. Ek
investor ke liye "10 lakh users" aur "1 crore users" mein das guna ka
farq hai; jo founder dono ko "bahut saare users" bolta hai, usse
paisa door rehta hai. Aur jo engineer millisecond bacha sakta hai,
woh Google/Amazon jaise business mein seedha revenue dial ghuma raha
hai, isliye aisi skill ki tankhwah crore paar jaati hai. Numbers ko
mehsoos karna Level 2, 3, 4 teeno ki shared bhasha hai.

## KHUD DEKHO (5 minute)

Phone pe stopwatch chalao aur 100 tak zor se gino. (~100 second.) Ab
hisaab: 1 million tak aise ginne mein kitne din? (~11 din, bina soye.)
1 billion tak? (~31 saal.) Ek baar khud hisaab lagaoge toh billion
shabd hamesha ke liye bhaari ho jaayega, jaisa use hona chahiye.

## SOCHNE KE LIYE

1. (derivation) Aapke phone ki chip 15 arab transistor ki hai. Agar
har transistor chawal ka ek dana hota, toh kitna chawal banta? (Ek
kilo mein ~50,000 dane.) Aur is se kya samajh aata hai ki chip banane
wali factory duniya mein teen-chaar hi kyun hain?

> **Jawab:** 15 arab / 50,000 = 3 lakh kilo, yaani 300 tonne chawal,
> pachees trucks bhar ke. Itni cheezein nakhoon bhar jagah pe, bina
> ek bhi galat lage, chhaapni hain. Isliye yeh duniya ki sabse
> mushkil manufacturing hai: ek factory lagane ka kharcha ~2 lakh
> crore rupaye, aur hunar sirf TSMC (Taiwan), Samsung (Korea), Intel
> (US) ke paas. Scarcity itni oonchi ki desh iske liye jang ki
> taiyari karte hain. Ab aap samajhte ho ki "chip war" news mein
> kyun rehti hai.
