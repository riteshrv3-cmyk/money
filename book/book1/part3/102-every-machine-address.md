# Chapter 5.2 [SPINE]: Pratyek machine la ek address

Network banla, raste zale. Ata post office cha juna prashna
ubha rahto: patra pohochvayche tar POTTA (address) lagto. "Ram
la dya" ne kaam hot nahi; Ram lakho aahet. Machines chya jagat
pan tech: message pathvaycha tar tya machine cha nemka address
lagto.

Address kasa asava? Part 1 ne uttar aadhich dila aahe: machine
la fakt numbers samajtat. Mhanun machine cha address ek NUMBER
aahe. Sadharan roop: char numbers, pratyek 0 te 255 madhla
(olakhicha vaatla? 8 bits = 256 sthiti, Chapter 1.4):

```
142.250.183.14     (he Google chya eka server cha address)
192.168.1.5        (he tumchya ghartlya phone cha asu shakta)
```

Ata ek ganit kara. Char numbers, pratyek 256 prakarcha: ekun
kiti address? 256 x 256 x 256 x 256 = sadharan 430 crore. 1980
madhe he "kadhich sampnar nahit" vaatle. Aaj jagat arabo phones,
TVs, gadya, ghadyala... address SAMPLE. Ha kharokhar ghadlela
prasang aahe: internet chya designers ni jag kevdha hoil he
kami andajle. (Upay pan aala: navin lamb address, IPv6, jya
madhe address sampuch shakat nahit. Pan juna system ajun
sagLikde aahe.)

Sampat aalele address jag ni kase vaparle? Ithun ek sundar
yukti nighali, jee tumchya gharat aahe: tumchya WiFi router la
EKACH public address milto (building la ek post-box). Ghartlya
sagLya devices na router aatlya-aat aaple chhote private
address deto (khli number 1, 2, 3...). Baherun sagle ekach
distat; aat router hishob thevto ki kuthla jawab kuthlya
device cha aahe. Ek address, dahaa machines. (Building cha
watchman jasa: patra building chya naavavar yeto, watchman
flat baghun pohochvto.)

## NAAV

Machine cha number-address: **IP address** (Internet Protocol
cha address). Juna char-number roop: **IPv4**, nava lamb roop:
**IPv6**. Ghartla vaatnara-watchman: **router**. Router chya
aatle address: **private IP**, jagala disnara: **public IP**.

## KHARYA JAGATLA EK EXAMPLE

Cyber crime chya batmya madhe "police ni IP address varun
aaropi shodhla" he vakya asta. Ata tumhala te vachta yeta:
pratyek internet connection chya magey ek public IP asto, ani
telecom company kade register asto ki tya veles to IP konala
dila hota (Chapter 0.1 cha ledger, parat!). Mhanunach VPN
naavachi cheez vikli jate: ti tumcha khara IP lapavte, dusrya
deshatla dakhavte. Suraksha ani lapan-chhapan, donhi ek
address chya bhovti firtat.

## ITHE LOK KAY CHUKICHE SAMAJTAT

"IP address mhanje majhi kayamchi olakh." Nahi. Tumcha public
IP telecom company ROJ badlu shakte (bhadyane dilela number
aahe, malkicha nahi). Ani ek IP magey shambhar lok asu
shaktat (router!). Mhanun IP fakt "tya veles, tya jaagecha"
pattaa aahe, aadhaar card nahi. Donhi disha ni chuk hote:
lok ghabartaat "majha IP disla, sagla sampla" (nahi), ani
lok nishchint pan astat "IP badalte mhanje mi lapla" (nahi:
register aahe na).

## MAP VAR

Kon kamavta: address SWATAHA ek malmatta zali. IPv4 address
sample, mhanun juna saatha asnaryanni te VIKAYLA kadhle: ek
IPv4 address aaj hazaro rupayala jato, companies chya kade
lakho address che block aahet, tyanchi kimmat arabo madhe.
1990 madhe fukat vaatlele numbers aaj sona zale. Dhanda
shikvan: jya cheez chi ginti THARLELI aahe ani magni vadhnaar
aahe, ti cheez lavkar dharun theva. (Domains madhe he parat
yeil, Chapter 5.5.)

## SWATAHA BAGHA (5 minute)

Phone chya Settings madhe WiFi ughda, jodlelya network var
tap kara: tithe "IP address" disel, sadharan 192.168.x.x asa.
Ha tumcha PRIVATE address. Ata browser madhe search kara:
"what is my IP". Vegla number disel! Ha tumchya router cha
PUBLIC address. Don address, don duniya: aat ani baher.
Watchman-system tumhi swataha baghitli.

## VICHAR KARA

1. (derivation) Postman la "Mumbai, Andheri, XYZ building,
flat 402" asa address TUKDYA-TUKDYANI kaam karto: aadhi
shahar, mag bhaag, mag building. IP address pan asach
tukdyani vachla jato (aadhi motha bhaag, mag aatla). Sagle
routers jagatlya SAGLYA machines chi yaadi ka thevat nahit,
ha design ka nivadla?

> **Uttar:** Karan yaadi arabo entries chi hoil ani ROJ
> badlel; pratyek chowkat ti thevne ani taji rakhne ashakya.
> Tukdya-tukdyancha design mhanje: pratyek router la fakt
> evdhach mahit lagta ki "ha bhaag tya dishela." Mumbai cha
> postman flat 402 janat nahi, fakt Andheri kuthe te janto.
> Kaam vaatle gele, koni-ekala sagla janave lagat nahi. He
> design-tattva (hierarchy) tantradnyanat sagLikde aahe:
> DNS madhe (5.5), company chya sanghatnet, ani AI chya
> aat pan. Jithe scale motha, tithe yaadi nahi, SHIDI aste.
