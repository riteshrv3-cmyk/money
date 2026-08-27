# PART 2 चा शेवट: नकाशा आणि पुढचं पाऊल

## जे तुमच्याकडे आता आहे

```
भाषांतराची शिडी    machine code -> assembly -> languages -> AI;
                   प्रत्येक मजला खालचा लपवतो
तीन गोष्टी         ठेवा (variable), विचारा (if), पुन्हा करा
                   (loop): प्रत्येक program यांचंच जाळं
दोन भाषांतरकार     compiler (आधी, वेगवान) vs interpreter (सोबत,
                   आरामाचा): चुकीची किंमत vs बदलाचा वेग
LANGUAGES          प्रत्येक भाषा चार सौद्यांची जोडणी; "कुठली
                   best" नाही, "कुठल्या कामाला कुठली"
OS                 machine चा मालक: पाळ्या, भिंती, दरबानी;
                   मालक जकात वसूल करतो (platform tax)
PROCESS            file झोपलेली recipe; process जिवंत copy
                   आपल्या state सह; restart = नवी स्वच्छ state
फुकटचा खेळ         दरवाजा / freemium / तुम्ही-माल / open
                   source: पैसा नेहमी दुसरीकडून
BUG                लिहिलं vs हवं ची फट; जोड्यांचा स्फोट;
                   मोजणी आहे, हलगर्जीपणा नाही
TESTING            तपासणंही code आहे; किती, हा business प्रश्न:
                   चुकीची किंमत काय
VERSION CONTROL    प्रत्येक बदलाचा photo + परत जायचं button
                   = हिमतीची व्यवस्था (Git, GitHub)
ENVIRONMENT        software = code + माहोल; म्हणून "माझ्या
                   machine वर चालत होतं" (Docker, deploy)
ESTIMATE           प्रत्येक software पहिल्यांदा बनतंय; इलाज
                   माप नाही, छोटे चालते तुकडे (MVP)
```

## एक परीक्षा, स्वतःसाठी

पुस्तक न उघडता, बोलून उत्तरं द्या:

1. iPhone ची app Android वर का चालत नाही?
2. Google Android फुकट का वाटतो?
3. "Bug-free software" चं वचन खोटं का आहे?
4. Software बनवून घेताना पैसा कशावर द्यायचा: वचनावर की कशावर?
   आणि का?

अडलात तर: 1 -> 3.5, 2 -> 3.5/3.7, 3 -> 4.1/4.2, 4 -> 4.5.

## Part 3 मध्ये काय आहे

आतापर्यंतची पूर्ण गोष्ट **एका** machine च्या आत होती. पण तुमचा
प्रत्येक message दुसऱ्या machine कडे जातो: शहरापलीकडे,
समुद्रापलीकडे, अर्ध्या second मध्ये. कसा? Machines एकमेकींना
शोधतात कशा? रस्त्यात कोण-कोण बसलं आहे? "Public रस्त्यावर private
बोलणं" (तुमचा password!) कसं वाचतं? आणि internet चा मालक शेवटी
कोण? Part 3: MACHINES चं जाळं.

# PART 2 चा MINI-GLOSSARY

```
agile            छोट्या चालत्या तुकड्यांची पद्धत (4.5)
assembly         numbers च्या नावांची भाषा, machine जवळची (3.1)
binary/executable
                 भाषांतर झालेली, थेट चालणारी file (3.3)
branch / merge   प्रयोगाची copy / ती परत जोडणं (4.3)
bug              लिहिलं आणि हवं यांच्यामधली फट (4.1)
CI               प्रत्येक बदलावर सगळे tests आपोआप (4.2)
code             कडक व्याकरणात लिहिलेली recipe (3.2)
commit           बदलाचा photo + "का" ची नोंद (4.3)
compiler         पूर्ण भाषांतर आधी करणारा (3.3)
condition (if)   अटीवर रस्ता निवडणं (3.2)
container/Docker code + माहोल एका डब्यात बंद (4.4)
crash            program चं अचानक मरणं (4.1)
debugging        bug शोधून दुरुस्त करणं (4.1)
deploy           code खऱ्या server पर्यंत पोहोचवणं (4.4)
DevOps           deploy आणि माहोलाची व्यवस्था-पेशा (4.4)
driver           hardware शी बोलणारा OS चा तुकडा (3.5)
edge case        कोपऱ्यातली दुर्मिळ परिस्थिती (4.1)
environment      recipe भोवतीची पूर्ण दुनिया (4.4)
file system      OS ची files ची व्यवस्था (3.5)
freemium         फुकट अर्धं, पूर्ण विकलं जातं (3.7)
Git / GitHub     version control चं हत्यार / त्याचा अड्डा (4.3)
interpreter      ओळी-ओळीने सोबत चालणारा दुभाषी (3.3)
loop             एक काम पुन्हा पुन्हा; code मधला leverage (3.2)
loss leader      फुकट चव, विक्री दुसरीकडे (3.7)
machine code     numbers ची भाषा जी CPU थेट समजतो (3.1)
merge conflict   दोन बदलांची टक्कर (4.3)
MVP              पहिलं छोटं चालतं रूप (4.5)
open source      उघडा code, सगळ्यांचं सामायिक हत्यार (3.7)
OS               machine चा मालक: पाळी, भिंत, दरबान (3.5)
platform (tax)   दरवाजाचा मालक आणि त्याची जकात (3.5)
process / state  जिवंत copy / तिची आत्ताची पूर्ण अवस्था (3.6)
regression       नव्या बदलाने जुनं काही तुटलं (4.2)
scheduling       CPU च्या पाळ्या वाटणं (3.5)
syntax (error)   कडक व्याकरण (त्याची चूक) (3.2)
tech stack       project च्या tools/भाषांची पूर्ण जोडणी (3.4)
unit test        छोटी आपोआप चालणारी तपासणी (4.2)
variable         नावाचा खण (3.2)
version control  बदलांच्या इतिहासाची व्यवस्था (4.3)
```
