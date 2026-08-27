# Chapter 4.1 [SPINE]: Software mein bug hote hi kyun hain

Pul girte nahi (aksar). Ghadiyan chalti rehti hain. Phir software,
jo duniya ke sabse padhe-likhe log banate hain, roz kahin na kahin
toot ta kyun rehta hai? Kya yeh laaparwahi hai?

Nahi. Yeh GINTI hai. Khud dekho.

Chapter 1.3 yaad karo: machine wahi karti hai jo LIKHA hai, woh
nahi jo aapka MATLAB tha. Toh bug ki definition ek line mein:
**jo likha aur jo chaha tha, unke beech ka gap.** Ab sawal yeh
hai ki itne hoshiyaar log gap chhodte kyun hain?

Kyunki recipe likhne wale ko HAR situation ka pehle se jawab
likhna padta hai. Aur situations ginti mein bam ki tarah phat-ti
hain. Ek chhota sa form socho: naam, umar, pincode. Naam khaali
ho toh? 500 aksharon ka ho? Emoji ho? Umar 0 ho? Minus 5? 200?
Pincode mein akshar hon? User ne aadha bhara aur network gaya?
Do baar submit dabaya? Teen fields ke bhi dus-dus roop lo toh
hazaar jod ban gaye. Asli app mein aise LAKHON jod hote hain,
aur likhne wala insaan har jod apne dimaag mein khel nahi sakta.
Jo jod uske dimaag mein kabhi aaya hi nahi, wahi kisi din kisi
user ke haath lag jaata hai. Us din "bug mila."

Ab pul se tulna karo, toh farq dikh jaayega: pul ke paas
situations kam hain (gaadi bhaari ya halki, hawa tez ya dheemi,
sab ek hi physics ke andar). Software ke paas situations ka
visphot hai, aur har naya feature purane sab ke saath naye jod
banata hai. Isliye 10 guna bada software 10 guna nahi, 100 guna
zyada jodon wala hota hai.

Toh sach yeh hai: **bade software mein bugs ka hona pakka hai,
sawal sirf yeh hai ki kitni jaldi milte hain aur kitna nuksan
karne se pehle pakde jaate hain.** Achhi company woh nahi jiske
bug zero hain (aisi company hai hi nahi), achhi woh hai jiska
pakadne aur sudhaarne ka intezaam tez hai. Agla chapter wahi
intezaam hai.

## NAAM

Gap ka naam **bug** (kissa: 1947 mein ek asli patanga, moth,
machine mein phansa mila tha; naam chipak gaya). Anokha,
kinaare ka situation: **edge case**. Program ka achanak marna:
**crash**. Bug dhoondh ke theek karna: **debugging**.

## ASLI DUNIYA SE EK EXAMPLE

31 December ki raat ya cricket final ke waqt UPI/payment apps
kyun ladkhadaate hain? Kyunki "ek saath itne log" khud ek edge
case hai jo aam din kabhi nahi aata. Ya calendar wale bugs:
leap year ka 29 February har chaar saal mein aata hai aur har
chaar saal mein kahin na kahin koi system girta hai, kyunki
kisi likhne wale ke dimaag mein woh jod nahi aaya tha. Duniya
ke sabse bade systems ke bug bhi isi ek kahani ke roop hain:
jod jo socha nahi gaya tha.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Bug aaya matlab engineer ghatiya hai." Kabhi kabhi sach,
lekin aksar nahi. Naya founder pehle bug pe chillata hai;
samajhdaar founder poochhta hai: kitni DER mein pata chala,
kitne users tak pahuncha, dobara na ho iska kya intezaam bana?
Team ka level bug ki ginti se nahi, JAWAB ki raftaar se napta
hai. (Aur jo bechne wala kahe "hamare software mein bug nahi
hote," woh jhooth bol raha hai ya usne bada software banaya
hi nahi.)

## MAP PE

Bug ka apna bazaar hai. Companies apne system todne walon ko
INAAM deti hain: bug bounty. Google/Apple/Microsoft ek sangeen
bug ke lakhon-crores tak dete hain, kyunki chori se pehle
chowkidaar ko milna sasta hai. India ke ladke bug bounty se
ghar baithe dollar kamaate hain: scarcity (todne ki nazar sab
ke paas nahi) x size (system arabon logon ke) = inaam bada.
Level 3 ke andar yeh ek poora pesha hai jisme degree koi nahi
poochhta, sirf hunar.

## KHUD DEKHO (5 minute)

Kisi bhi app ke search box mein daalo: kuch nahi (khaali
search), sirf space, ek emoji, 200 akshar ka kachra. Dekho kya
hota hai. Aksar sab theek hoga (kisi ne yeh jod socha tha),
kabhi ajeeb jawab milega (nahi socha tha, aapne edge case pakda).
Aap abhi wahi kar rahe ho jo tester tankhwah le kar karta hai:
un jodon ko dhoondhna jo likhne wale ke dimaag mein nahi aaye.

## SOCHNE KE LIYE

1. (derivation) Do features wale app mein features ke aapas ke
jod ginno: 1. Ab 10 features pe kitne jod? Aur is se nikaalo:
"bas ek chhota sa feature aur daal do na" pe engineer ka chehra
kyun utar jaata hai?

> **Jawab:** 2 features = 1 jod. 10 features = har ek ka har
> doosre se jod = 45. Feature 5 guna badhe, jod 45 guna. Har
> naya feature purane SAB ke saath naye jod laata hai, aur har
> jod ek nayi jagah hai jahan bug chhup sakta hai. Isliye
> "chhota sa feature" chhota kabhi nahi hota: uski asli keemat
> uske jodon mein hai. Founder ke liye iska naam hai: feature
> ki keemat = banane ka waqt + hamesha ke liye badha hua
> jodon ka bojh. Isliye behtareen products features JODNE se
> nahi, feature NA jodne ki zid se bante hain.
