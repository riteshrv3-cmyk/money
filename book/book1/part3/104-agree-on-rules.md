# Chapter 5.4 [SPINE]: Niyam var aadhich sahmati

Address aahe, packets aahet. Pan ajun ek prashna lapla aahe,
ani to sagLyat khol aahe.

Phone call chi suruvat aathva: "Hello?" "Haan, bola." "Mi
Ramesh boltoy..." He shabd mahiti det nahit; he KRAM aahe.
Kon aadhi bolnaar, kasa kalel ki samor koni aahe, "aika ka"
cha ishara kay. Doghanni ha kram AADHICH manlela asto, mhanun
call chalte. Ek jan Japani kram ni bolla ani dusra Marathi
kram ni, tar shabd pohochtil pan bolne honar nahi.

Machines madhe ha prashna ajun tikat asto, karan machine
kade "samjun ghene" nahi (Part 2, Chapter 3.1: exact lagta).
Don machines na bolayche tar SAGLA aadhich tharlela lagta:

- Kon suruvat karnaar? Kasa mhannaar "mi tayar aahe"?
- Message cha format kay? Kuthle bits address, kuthle maal?
- "Pohochla" kasa kalvnaar? Nahi pohochla tar kay?
- Chuk zali tar kon parat pathavnaar, kiti vela?

Ashya aadhich-tharlelya niyamanchya yaadila protocol mhantat.
Ani internet mhanje kay, yacha ARDHA uttar he aahe: **internet
ek vastu nahi, niyamanchi yaadi aahe.** Jo koni te niyam
paalto, tyachi machine jaalat samil hote. Parvangi konachi
ghyaychi nahi, fee konala dyaychi nahi. Niyam public aahet,
darvaja sagLyanna ughada.

Ani niyam EKA thara var nahit, SHIDI var aahet (abstraction,
parat!): sagLyat khali "taar var current kasa" che niyam,
tyavar "address ani packets" che (IP), tyavar "harvlela parat
magva" che (TCP), ani sagLyat var "app la kay have" che niyam.
Website magvaychya niyamanche naav tumhi roj baghta: **HTTP**.
Browser chya pattyat "https://..." mhanje "hi baat HTTP chya
niyamani honar" evdhach. Pratyek thar fakt aaple kaam janto,
khalcha thar kasa chalto he tyala mahit nasta. (Chapter 0.4:
har level, khalchya cha fakt handle dharto.)

Ata dhandyachi nazar laava. Jithe protocol KHULA asto, tithe
koni-hi dukan ughdu shakto: email che niyam khule, mhanun
hazaro email companies. Jithe niyam EKA company che astat,
tithe tichi hukumat: WhatsApp che niyam Meta chech aahet,
mhanun WhatsApp la jodnara dusra app banuch shakat nahi.
Khule niyam = spardha = grahakala swasta. Band niyam = kila.
Doghanchehi dhande chaltat, pan konta khel khelto aahot he
kalayla have.

## NAAV

Aadhich-tharlele niyam: **protocol**. Web cha protocol:
**HTTP** (surakshit roop: HTTPS, Chapter 5.6). Email cha:
SMTP. Niyamanchi shidi: **protocol stack** ya **layers**.

## KHARYA JAGATLA EK EXAMPLE

UPI he protocol aahe, app nahi. NPCI ni niyam banavle: paisa
magnyacha format kay, banks ni kase bolayche, "zala" kasa
kalvaycha. Niyam KHULE thevle: mhanun GPay, PhonePe, Paytm,
koni-hi bank, sagle ekmekanshi chaltat. Tumhi GPay varun
PhonePe walyala paise pathavta ani vichar pan karat nahi,
he kevdha motha chamatkar aahe: don spardhak companies chya
apps madhe paisa binadhok vahto, karan protocol samaan aahe.
Ani parinam jag baghta aahe: mahina 10 arab+ vyavhar. Niyam
banavnara (NPCI) swataha motha "app" nahi, pan sagLya khela
cha aadhaar to aahe.

## ITHE LOK KAY CHUKICHE SAMAJTAT

"Internet chi malak kuthli tari company aahe (Google?
Microsoft?)." Nahi. Internet konachich malmatta nahi, karan
to niyamancha samuh aahe, ani niyam sagLyankade aahet.
Google chya SEVA (search, YouTube) tyachya aahet; RASTA
tyacha nahi. Ha farak mahatvacha aahe: seva band hou
shakte, rasta band karayla jagbharche niyam badlave lagtil.
(Kon niyam banavto, ha prashna Chapter 5.8 madhe.)

## MAP VAR

N squared cha rakshasa parat aala hota, baghitla ka? UPI
chya aadhi pratyek app la pratyek bank shi VEGLA jod banvava
lagla asta: 50 apps x 300 banks = 15,000 jod. Protocol ni
te 350 kele (pratyekane fakt niyamanshi jodayche). **Jo
n-squared la protocol ni maarto, to purna bajaracha payabhut
thar banto.** NPCI ni he payment madhe kele. Tumchya 4-level
naksha var: jithe pratyekala pratyekashi jodave lagta aahe
ani sagle metaakle aahet, tithe protocol chi jaaga rikaami
aahe. Ashi jaaga disli tar neat baghaa: ti arabonchi aahe.

## SWATAHA BAGHA (5 minute)

Browser madhe kuthlihi website ughda ani pattyakade LAKSH
dya: https:// ne suruvat. Ata ek juni goshta: kahi varshan-
purvi fakt http:// aste (s nahi). Ata browser http varchya
site la "Not secure" mhanto. Ek akshar (s) mhanje ek purna
protocol-badal, ani to badal jagbhar ka ghadla he Chapter
5.6 sangel. Aaj fakt te aksharaa dise ka baghaa.

## VICHAR KARA

1. (derivation) UPI sarkha khula protocol banavnyat NPCI
la (ani banks na) kay milte? Tyanni band, aaplya-malkicha
system ka nahi banavla, jasa Visa/Mastercard ni banavla
hota?

> **Uttar:** Band system ni pratyek vyavhaarat fee milte
> (Visa cha model: dukandara kadun 1-2%). Khula system ni
> VAAPAR sphotasarkha vadhto: UPI fukat thevla mhanun
> chahawalya pasun bhajiwalya paryant sagle aale, ani 10
> varshat rok-paisa (cash) cha desh digital zala. NPCI
> sarkari-sahakari aahe, tila fee peksha VYAAPTI havi
> hoti; ani banks na sagLya deshacha paisa system madhe
> aala he milala. Dhanda-shikvan: fee-per-vyavhaar ha ek
> khel aahe, purna bajarachi payabharni dusra. Doosra
> khel motha asto, pan to khelayla lambi saans lagte, ani
> kamai thet nahi tar var-chya tharatun yete (data,
> seva, darvaja). Google ni Android madhe hech kele hote,
> aathvta? Pattern ekach aahe.
