# Chapter 5.1 [SPINE]: Ek machine puri padat nahi

Part 1 ani 2 ni tumhala ek shaktishali machine dili: universal
machine, jya var kuthlihi recipe chalte. Mag prashna asa: ekach
machine puri ka padat nahi? WhatsApp tumchya phone var aahe na?

Nahi. Tumchya phone var WhatsApp cha fakt DARVAJA aahe. Vichar
kara: tumhi message pathavla ani mitracha phone band aahe. Tari
message pohochto, to phone chalu kartach. Mhanje message madhe
kuthe tari THAMBLA hota. Kuthe? Tumchya phone var nahi (tumhi
pathavla, gela). Tyachya phone var nahi (band hota). Mhanje
madhye TISRI machine aahe, jya var message vaat baghat basla
hota.

Ti tisri machine WhatsApp chya company chi aahe, ani ashya
machines lakhoni aahet. Ka lagtat? Teen karana, tinhi tumhi
swataha kadhu shakta:

**Data sagl-yancha ekatra asava lagto.** Tumcha bank balance
tumchya phone var thevla tar? Phone haravla, paisa gela. Ani
dukandarala kasa kalel ki tumchyakade paise aahet? Jo data
DOGHANNA lagto, to doghanchya madhye, tisrya jaagi rahava lagto.

**Ek machine crore lokanna serve karu shakat nahi.** Ek CPU,
ek second madhe arab kadam (Part 1). Vaatun ghya: crore lok ale
tar pratyekala kiti? Kaam vaatava lagta, khup machines madhe.

**Machines padtat.** Bijli jate, disk jalte. Sagla ekach jaagi
thevla ani ti jaaga padli, tar sagla gela. Prati (copies)
veglya jaagi lagtat.

Mhanun jag ashya do bhaagat vibhagla gela: tumchya hatatli
machine (magnaari) ani company chya building madhli machine
(denari). Ani ata sagLYAT motha prashna: ya machines ekmekashi
BOLNAR kashya?

Don machines madhe taar odha, current cha pattern pathva (Part
1, Chapter 1.2: signal mhanje he ch), bits gele. Don machines
zalya. Pan crore machines? Pratyekala pratyekashi taar jodli
tar? Ganit kara: 100 machines la 4,950 taara lagtil, crore
machines la... jamnar nahi. (He "n squared" aahe: sankhya vadhli
ki jod tya sankhyechya varga ne vadhtat. He naav lakshat theva,
ya part madhe he rakshasa parat parat yeil, ani pratyek veli
koni tari tyala harvun shrimant hoil.)

Upay tumhi rozchya jagat baghitla aahe: rasta. Pratyek ghara
pasun pratyek ghara paryant rasta nasto; galli aste, chowk asto,
highway asto. Tasach machines cha rasta banto: tumchi machine
javlchya chowkala jodleli, chowk mothya chowkala, ase jod-jodun
sagla jag. Ha rasta ch NETWORK aahe.

## NAAV

Magnaari machine: **client**. Denari machine: **server** (serve
karnari, mhanun). Jodlelya machines cha jaal: **network**. Ani
"pratyekala pratyekashi jodne jamnar nahi" hi problem: **n
squared problem**.

## KHARYA JAGATLA EK EXAMPLE

Tumhi Zomato var order karta. Tumcha phone (client) Zomato chya
server la magni pathavto. Server tumcha order thevto, restaurant
chya screen la (dusra client) dakhavto, delivery walyachya phone
la (tisra client) pathavto. Teen client, ek server, ani sagle
ekmekanna kadhich thet jodlele nahit: pratyek jan fakt server
shi bolto. Chowk ek, raste tin. N squared la asech harvtat.

## ITHE LOK KAY CHUKICHE SAMAJTAT

"Majha message thet mitrachya phone la jato." Kadhich nahi.
Pratyek message aadhi company chya server la jato, mag mitrala.
(End-to-end encryption asel tar company VACHU shakat nahi, pan
rasta tyanchyach madhun jato: Chapter 5.6 madhe he ughdel.)
Mhanunach "fukat" apps chya company kade evdhi takat aste:
sagla traffic tyanchya chowkatun jato.

## MAP VAR

Rupayacha rasta: tumhi mahina bharla (Level 1 pasun paisa
ghusla) -> telecom company (Jio/Airtel) la, ti rasta dete.
App company chya server cha kharcha ti cloud la dete (Part 5).
Ani he baghaa: jya business kade SERVER aahe, tyachya kade
DATA aahe; jya kade data, tyachya kade takat. Client banavne
sopa ani swasta zala aahe; server chi baju hich khari malmatta
aahe. Tumhi jo business banval, tyat "server var kay rahnaar"
ha prashna mhanje "malmatta kay asnaar" ha prashna aahe.

## SWATAHA BAGHA (5 minute)

Phone airplane mode var taka. Ata apps ughda: WhatsApp chats
distat (juna data, phone var sathavlela), pan nave message
yet nahit. Google Maps cha naksha adhvat ughdto, search chalat
nahi. Camera purna chalto. Ata tumhala pratyek app che don
bhaag distil: jo tumchya hatat aahe, ani jo koni-tari-dusrya-
chya machine var aahe. Hi rekha baghayla shikne mhanje network
samajne.

## VICHAR KARA

1. (derivation) 100 lokanchi society aahe. Pratyekane
pratyekashi thet bolayche tharvle tar 4,950 jod lagtat. Ek
chowk (server) banavla tar fakt 100. Pan ata ek navin kimmat
ali, ti kuthli? (Chapter 0.1 chi aathvan kara: register
thevnarya var kay prashna hota?)

> **Uttar:** Bharosa. Sagli bolni eka chowkatun jaate, mhanje
> chowk cha malak sagla baghto, thambvu shakto, badlu shakto.
> N squared sutla, pan satta ek jaagi ekavtali. Mhanunach he
> pattern parat parat disel: sopa rasta = madhla malak. Ani
> tyachya virudh che prayog pan (blockchain vagaire) yach
> dukhavar ubhe aahet. Tantradnyan cha pratyek design ek
> sauda asto: ithe suvidha vs satta ha sauda aahe. Jo he
> baghto, to batmya nahi, DHANDA vachto.
