# Chapter 2.2 [SPINE]: Text, photo, awaaz, video: sab numbers hain

Machine sirf numbers jaanti hai. Toh aapki shaadi ki photo, maa ki
awaaz wali recording, yeh kitaab ka text, yeh sab machine mein kaise
ghusa? Har ek ka jawab ek hi chaal se niklega. Chaal yeh hai:

**Cheez ko chhote chhote tukdon mein kaato, har tukde ko ek number do,
aur numbers ka matlab pehle se sab mil kar tay kar lo.**

Ab chaaron pe lagao:

**Text.** Tukda = akshar. Sab ne mil kar tay kiya: A = 65, B = 66,
space = 32. Toh "HI" machine mein 72, 73 hai. Bas. Aapke naam ka
spelling numbers ki qataar hai. (Hindi ke aksharon ke bhi numbers tay
hain, अ = 2309.)

**Photo.** Tukda = bindu (pixel). Photo ko jaali mein kaato, har
khaane ka ek rang. Aur rang? Har rang laal, hara, neela ke mel se
banta hai, toh teen numbers (0-255) har bindu ke liye: (255, 0, 0) =
poora laal. 40 lakh bindu x 3 numbers = aapki photo.

**Awaaz.** Awaaz hawa ka kampan hai. Tukda = waqt ka pal. Har second
ko ~44,000 palon mein kaato, har pal pe kampan ki oonchai naapo, woh
number likh lo. Numbers ki qataar wapas bajao, awaaz wapas. Maa ki
awaaz 44,000 numbers prati second hai.

**Video.** Tukda = frame. Har second 30 photos, plus awaaz. Isliye
video sabse bhaari hai: photo ka kharcha x 30 x seconds.

Teeno kadmon mein sabse zaroori kaunsa hai? Kaatna? Naapna? Nahi:
**"matlab pehle se sab mil kar tay kar lo."** 72 ka matlab H tabhi
hai jab bhejne wala aur paane wala dono ek hi table maante hon. Agar
mera 72 H hai aur tumhara kuch aur, toh message kachra ban jaayega.
Yeh baat, ki **numbers ka matlab samjhauta hai, numbers mein nahi
hota**, aage internet (Part 3) aur AI (Book 2) dono ki neev hai.

## NAAM

Matlab tay karne wale table ka naam **encoding** hai. Text ka sabse
purana table **ASCII** (1963), aaj ka poora table **Unicode**, jisme
duniya ki har bhasha aur emoji tak hai (emoji bhi bas ek number hai:
"laughing face" = 128514). Photo ke bindu ka naam **pixel**, awaaz ke
pal ka naam **sample**, video ki photo ka naam **frame**.

## ASLI DUNIYA SE EK EXAMPLE

Jab aap Hindi mein type karte ho aur kisi purani website pe ??? ya
dibbe dikhte hain, toh kya hua? Aapke numbers pahunch gaye, lekin us
taraf ka software Unicode ka Hindi wala hissa nahi jaanta tha. Numbers
sahi, matlab kho gaya. Poori duniya ka software dheere dheere Unicode
pe isliye aaya kyunki bina ek jaisi table ke, bhaashaon ka internet
ban hi nahi sakta tha. Ek boring sa samjhauta, arabon logon ko jodne
ki shart nikla.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

Log sochte hain machine photo "dekhti" hai ya gaana "sunti" hai. Nahi.
Machine ke liye photo 1.2 crore numbers hain aur gaana 1.5 crore.
Usko na rang pata hai na raag. Aur phir bhi (yeh aage Book 2 ka beej
hai) numbers ke pattern se machine bata deti hai ki photo mein billi
hai. Dekhna nahi, ginti se pehchaan. Jab woh baat aaye, yeh chapter
yaad rakhna: sab kuch numbers hi tha, hamesha.

## MAP PE

Company case: JioCinema/Hotstar jab cricket dikhata hai, toh 4 crore
log ek saath frames ke numbers maang rahe hote hain. Unka poora
engineering kharcha isi chapter ke anupaat se aata hai: video = sabse
bhaari numbers. Aur unka business model bhi wahi tay karta hai: ads
aur subscription zaroori hain, kyunki har viewer ka data kharcha asli
hai. Level 1 zaroorat: manoranjan. Uske numbers: sabse mehnge.

## KHUD DEKHO (5 minute)

Kisi ko yeh message bhejo: "72 69 76 76 79". Aur bolo har number 64
ghata ke A=1, B=2 wali ginti pe akshar banao. Jawab aayega HELLO. Aapne
abhi apna encoding table banaya aur ek insaan ko decode karwaya. Machine
bas yahi karti hai, arab guna tez.

## SOCHNE KE LIYE

1. (derivation) WhatsApp voice message bhejte waqt "bhejne se pehle
daba do" (compress) kaise possible hai? Awaaz toh naapi hui thi,
44,000 number prati second. Kaunse numbers phenke ja sakte hain?

> **Jawab:** Woh jo insaan ke kaan waise bhi nahi pakadte. Bahut
> ooncha kampan, bahut halki awaaz jo tez awaaz ke peeche dab gayi,
> do palon ke beech ka farak jo andaaze se wapas ban sakta hai. Recipe
> unhe phenk deti hai, size das guna girta hai, kaan ko farq nahi
> padta. Sabak: compression ka matlab hai "matlab bachao, numbers
> phenko." Aur dhyaan do, yeh ek FAISLA hai ki kya phenkna hai, aur
> har faisla kisi insaan ki recipe mein likha hai. Machine mein har
> jagah aise chhupe hue faisle milenge.
