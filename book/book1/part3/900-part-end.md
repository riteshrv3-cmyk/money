# PART 3 चा शेवट: नकाशा आणि पुढचं पाऊल

## जे तुमच्याकडे आता आहे

```
CLIENT / SERVER   मागणारी machine / देणारी machine;
                  मालमत्ता server च्या बाजूला असते
N SQUARED         प्रत्येकाला प्रत्येकाशी जोडणं अशक्य; जो हे
                  चौक/protocol ने सोडवतो तो मालक होतो
IP ADDRESS        machine चा number-पत्ता; public vs private
                  (router = building चा watchman)
PACKETS           message चे numbered तुकडे, स्वतंत्र प्रवास;
                  "connection" हा फक्त भास आहे
TCP vs UDP        बरोबरपणा vs वेग: file vs video call
PROTOCOL          आधीच ठरलेले नियम; internet म्हणजे वस्तू
                  नाही, नियमांचा समूह (UPI = protocol!)
DNS               नाव -> number ची phonebook; शिडी + cache;
                  domain = पाटी, server = दुकान
ENCRYPTION        public रस्त्यावर गणिती लिफाफा; दोन किल्ल्या
                  (public कुलूप लावते, private उघडते);
                  कुलूप = रस्ता सुरक्षित, माणूस नाही!
INTERNET          हजारो मालकांची जाळी, जोडलेली; 99% समुद्री
                  cables; केंद्र नाही, मालक नाही
NIYAM             IETF/ICANN/W3C + मोठ्या companies; standard
                  बनवणारा बाजार आखतो (भारताचं DPI)
```

## एक परीक्षा, स्वतःसाठी

पुस्तक न उघडता, बोलून उत्तर द्या:

1. WhatsApp message थेट मित्राच्या phone ला का जात नाही?
2. Video call मध्ये आवाज robotic का होतो, पण file download
   मध्ये file कधीच अर्धवट का येत नाही?
3. कुलूप-icon (https) काय सांगतो आणि काय सांगत नाही?
4. UPI ला "protocol" का म्हणावं, app का नाही? आणि त्याने
   भारताला काय दिलं?

अडाल तर: 1 -> 5.1, 2 -> 5.3, 3 -> 5.6, 4 -> 5.4/5.8.

## Part 4 मध्ये काय आहे

Server ला कोटी लोकांचा data मिळतो. तो ठेवायचा कुठे? एका
कोटीमधून एक नोंद शोधायची कशी, डोळ्याच्या पापणी लवण्याच्या आत?
दोन लोक एकाच वेळेस एक गोष्ट बदलतात तेव्हा काय होतं? आणि सगळा
data उडाला तर? Part 4: DATA आणि आठवणी: database चं जग, जिथे
प्रत्येक मोठ्या company ची खरी संपत्ती पडलेली असते.

# PART 3 चा MINI-GLOSSARY

```
cache             उत्तर लक्षात ठेवणं, परत शिडी न चढण्यासाठी (5.5)
certificate       "ही site खरीच ती आहे" चा दाखला (5.6)
client / server   मागणारी / देणारी machine (5.1)
DNS               नाव-ते-number phonebook, शिडी-रचनेची (5.5)
domain            website चं नाव; भाड्याची नोंद, मालमत्ता-पाटी (5.5)
DPI               भारताचा सरकारी-protocol खेळ: UPI, Aadhaar (5.8)
encryption        गणिती लिफाफा; वाचू फक्त किल्लीवाला शकतो (5.6)
end-to-end        किल्ल्या फक्त दोन टोकांवर; मधली company पण आंधळी (5.6)
HTTP / HTTPS      web चा protocol / त्याचं सुरक्षित रूप (5.4, 5.6)
ICANN             नावं आणि numbers वाटणारी संस्था (5.8)
IETF / RFC        मूळ नियम बनवणारी संस्था / खुला प्रस्ताव (5.8)
IP address        machine चा number-पत्ता (IPv4 जुना, IPv6 नवा) (5.2)
ISP               internet-रस्ता विकणारी company: Jio, Airtel (5.7)
last mile         तुमच्या घरापर्यंतचा शेवटचा (महाग) तुकडा (5.7)
latency           एक फेरा किती वेळ; bandwidth पेक्षा वेगळी गोष्ट (5.3)
n squared         जोड संख्येच्या वर्गाने वाढतात ही अडचण (5.1)
network           जोडलेल्या machines चं जाळं (5.1)
packet            message चा numbered, स्वतंत्र तुकडा (5.3)
peering           दोन जाळ्यांची "तू माझा, मी तुझा" सौदेबाजी (5.7)
private key       उघडणारी किल्ली; कधीच कोणाला नाही (5.6)
protocol          आधीच ठरलेले बोलण्याचे नियम (5.4)
public key        कुलूप लावणारी किल्ली; जगाला वाटलेली (5.6)
router            packets पुढे ढकलणारा चौक; घरचा watchman (5.2)
standard          सर्वमान्य नियम; बनवणारा बाजार आखतो (5.8)
TCP / UDP         बरोबरपणा-वाले / वेग-वाले नियम (5.3)
undersea cable    समुद्री काच-तार; जगाचा 99% data इथून (5.7)
```
