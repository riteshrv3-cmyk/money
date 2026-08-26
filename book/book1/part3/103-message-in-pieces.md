# Chapter 5.3 [DEPTH]: Message che tukde karne

(DEPTH chapter. Vagalla tari goshta pudhe jaeel, pan ha lahaan
aahe ani yachya nantar "packet" ani "network slow" che khare
arth ughadtat.)

Address zala. Ata message pathvaycha aahe: samja 3 MB cha photo
(Part 1: mhanje sadharan 2.5 crore bits). Sopa vaatnara rasta:
sagle bits ek-saath, ek lambach-lamb pravah mhanun pathva.

Ha design VAIT aahe. Ka, te tumhi truck chya udaharana ne kadhu
shakta. Samja Mumbai-Pune rasta aahe ani tya varun ek 3 km
lamba truck jato aahe:

1. Jya veles to jato, DUSRA konich rasta vapru shakat nahi.
   Ek motha message = baki saglyanchi thambleli line.
2. Truck madhe kuthe bighad zala tar? SAGLA parat pathva.
   3 MB madhla shevatcha bit chukla, tar purna 3 MB parat.
3. Ani rasta ekach asel tar to padla ki sagla thambla.

Mag design tumhi kara. Rasta-yantrana kashi asavi?

Uttar: **message che LAHAAN tukde kara.** Pratyek tukdyavar
liha: konala jaycha (address), konakadun aala, ani tukda
number kiti (1 of 2000, 2 of 2000...). Ata pratyek tukda
SWATANTRA pravaas karto. Faayde aapoaap yetat:

Raste vaatle jatat: tumchya tukdyanchya madhun dusryanche
tukde pan jaatat, koni rasta adkvat nahi. Tukde VEGVEGLYA
rastyani pan jau shaktat: ek highway ne, ek gaava-madhun; jo
mokala tya tya kshani. Ek tukda haravla tar FAKT TOCH parat
magvaycha, purna message nahi. Ani pohochlyavar number pramane
lavun message parat jodla jato. (Order ulti-sulti pohochli
tari chalte: numbers aahet na.)

Ekach goshta lakshat theva: tumhala vaatta tumhi "connection"
ughdla aahe, ek paip, ek dhaga. Prat-yakshat DHAGA NAHI. Fakt
tukde aahet, swatantra udya maarnare. "Connection" ha ek
bhaas aahe jo donhi tokanchi software tumhala dakhavte:
tukde mojun, harvlele parat magvun, order lavun. Bhaas
sundar aahe, pan to bhaas AAHE he samajlyavar network chya
sagLya vichitra goshti sopya hotat: video call madhla robotic
aawaz, adkleli file, "reconnecting..." sagla.

## NAAV

Message cha tukda: **packet**. Tukde-karun-pathavnyachi hi
yantrana: **packet switching** (1960s cha shodh, ani internet
chi khari payabharni). "Harvlela parat magva, order lava,
bharosa dya" he kaam karnare niyam: **TCP**. "Parat magvaycha
nahi, jo pohochla to pohochla, VEGA mahatvacha" he niyam:
**UDP**. (Donhi naave batmyan-madhe yetat; ata tumhala arth
mahit aahe.)

## KHARYA JAGATLA EK EXAMPLE

File download hotana network 2 second gela: download THAMBTO,
mag tithunach pudhe chalto. Karan file la TCP: pratyek tukda
pohochlach pahije, kimmat mhanun vel. Video call madhe network
2 second gela: aawaz robotic hoto, chehra atakto, pan call
CHALU rahto. Karan call la UDP-sarkhe niyam: juna tukda parat
magvun kay upyog? To kshan tar gela. Don design, don dhanda-
garja: barobar-pana vs vega. Kuthla kadhi nivdaycha he
samajne mhanje network engineer chi ardhi vidya.

## ITHE LOK KAY CHUKICHE SAMAJTAT

"Net slow aahe mhanje speed kami aahe." Adhura. Don vegLya
goshti astat: ek second madhe KITI tukde jaatat (bandwidth)
ani EKA tukdyala jaun-yeun kiti vel lagto (latency, Chapter
2.3 madhe bhetleli). Movie baghayla bandwidth lagte; game
ani video call la latency maarte. Mhanunach "100 Mbps" cha
plan asun pan game madhe "lag" yeto: tukde khup jaatat, pan
pratyek tukdyacha pheraa lamba aahe. Dukandar tumhala fakt
ek number vikto; khela don numbers cha aahe.

## MAP VAR

Company case: packet switching ni junya telephone jagala
harvle. Telephone company kade "ek call = ek rakhiv line"
asa mahag design hota; packets ni tich taar hazaro lokan-
madhe vaatli. Jo rasta swasta karto to jinkto: he pattern
parat. Ani aaj packets chya rastyavarchi yantre (routers)
banavnari Cisco ek kaali jagatli sagLyat moulyavaan company
hoti. Rasta jithe navin banto, tithe yantre viknara pahila
shrimant hoto. (AI madhe aaj Nvidia tech kaam karte aahe:
navin rasta, yantre viknara.)

## SWATAHA BAGHA (5 minute)

Pudhchya video call chya veles network kharab zala ki
LAKSH dya: aawaz robotic ka hoto? Karan software harvlele
packets bharun kadhnyacha prayatna karte aahe. Chehra ka
"atakto" ani mag udi maarto? Karan madhle frames (packets)
gele, software ni te sodle ani navin var udi maarli. Tumhi
ata bighad NAHI, DESIGN baghat aahat: vega sathi barobar-
pana sodlela.

## VICHAR KARA

1. (derivation) Live cricket match streaming madhe ek packet
haravla. To parat magvava ka? TCP ka UDP-vichar? Ani bank
transaction madhe? Donhi uttare ka veg-vegli aahet?

> **Uttar:** Cricket: parat magvu naka. To kshan gela; parat
> magvun jo tukda yeil to juna asel, ani tya sathi thambne
> mhanje purna stream ushira. Prekshakala 2 second juna
> perfect picture nako, AATTACHA thoda kharab chalel. Bank:
> parat magva, ani jo paryant pakka pohochat nahi to paryant
> kahihi pudhe jau deu naka. Ek rupaya chukla tari chalnar
> nahi; vel lagla tari chalel. Niyam asa nighto: jithe
> KSHAN mahatvacha tithe vega jinkto, jithe BAROBAR-PANA
> mahatvacha tithe kimmat mhanun vel dyava lagto. Tumchya
> product madhla pratyek feature ya do rangaat vaatun
> baghaa; tantra-nivad aapoaap sopa hoto.
