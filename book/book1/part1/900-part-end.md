# PART 1 चा शेवट: नकाशा आणि पुढचं पाऊल

## जे तुमच्याकडे आता आहे

```
पैसा               विश्वासाची व्यवस्था; फक्त Level 1 वर घुसतो
कमाईचं सूत्र       size x scarcity x leverage (तास नाहीत)
चार LEVELS         गरज -> business -> technology -> AI;
                   पैसा खालून वर वाहतो
ABSTRACTION        प्रत्येक मजला खालचा लपवतो, आणि लपलेला
                   हिस्साच महाग असतो

MACHINE            billions switches (transistors), design
                   केलेल्या साखळ्यांमध्ये
BIT / BYTE         switch ची स्थिती / 8 switches चा गट
GATES              AND, OR, NOT: यांतूनच बेरीज, तुलना, "जर"
COMPUTER           numbers वर आधीच लिहिलेली recipe, billion
                   पावलं प्रति second, न थकता
UNIVERSAL MACHINE  recipe पण number आहे, म्हणून एक machine
                   सगळं काही: हाच software चा जन्म
सगळं NUMBER        text/photo/आवाज/video: कापा, मोजा, अर्थ
                   आधीच ठरवा (encoding)
माप                KB->MB->GB->TB, प्रत्येक पायरी हजारपट;
                   text : photo : video = 1 : हजार : लाख
आत VS बाहेर        CPU चं पाऊल nanosecond, internet चा फेरा
                   millisecond: 1 million पटीचा फरक
दोन स्मरणशक्ती     RAM (मेज: वेगवान, विसराळू) vs storage
                   (गोदाम: हळू, पक्कं)
```

## एक परीक्षा, स्वतःसाठी

पुस्तक न उघडता, कोणाला तरी (किंवा स्वतःला, बोलून) ही 4 उत्तरं द्या:

1. पैसा फक्त Level 1 वर का घुसतो?
2. Surgeon पेक्षा app वाला जास्त का कमावतो?
3. एकच phone camera पण, bank पण, game पण कसा बनतो?
4. "8 GB RAM, 128 GB storage" चा अर्थ काय?

चारही आली, तर Part 2 साठी तयार आहात. जे अडलं, त्याचा chapter
number वरच्या नकाशात मिळेल; तिथे परत जा.

## Part 2 मध्ये काय आहे

Machine recipe चालवते, हे कळलं. आता पुढचा प्रश्न: recipe **लिहिली**
कशी जाते? माणसाच्या भाषेपासून machine च्या numbers पर्यंत भाषांतर
कोण करतं? Languages इतक्या साऱ्या का आहेत? तो manager कोण जो
सगळ्या recipes ना एका machine वर भांडण्यापासून रोखतो (operating
system)? आणि software मध्ये bugs असतातच का? Part 2: MACHINE शी
बोलणं.

# PART 1 चा MINI-GLOSSARY

फक्त ते शब्द जे या part मध्ये आले. प्रत्येकापुढे त्याचा chapter,
म्हणजे परत जाणं सोपं.

```
abstraction        आतली गुंतागुंत झाकून सोपं handle देणं (0.4)
AND / OR / NOT     तीन मूळ gates: दोन्ही/कोणीही/उलट (1.5)
ASCII / Unicode    अक्षरांच्या numbers चा करार, जुना / आजचा (2.2)
binary             दुप्पट-वाली मोजणी, फक्त 0 आणि 1 (1.4)
bit                एका switch ची स्थिती: 0 किंवा 1 (1.4)
byte               8 bits; साधारण एक अक्षर (1.4)
circuit            विजेचा बंद रस्ता (1.1)
CPU / processor    recipe चालवणारा मुख्य भाग (1.3)
double coincidence of wants
                   दोघांना एकाच वेळेस एकमेकांची गोष्ट हवी (0.1)
encoding           numbers चा अर्थ ठरवणारं table (2.2)
fetch-decode-execute
                   CPU चं तीन-पावलांचं चक्र: उचला, समजा, करा (2.4)
frame              video चा एक photo; ~30 प्रति second (2.2)
GHz / clock speed  चक्राचा वेग: billion फेरे प्रति second (2.4)
hardware           हाताला लागणारी machine (1.3)
KB / MB / GB / TB  size ची शिडी, प्रत्येक पायरी हजारपट (2.1)
latency            काम सुरू होऊन उत्तर येईपर्यंतचा वेळ (2.3)
ledger             देवाण-घेवाणीची वही; पैसा चालती वही आहे (0.1)
leverage           काम एकदा, फायदा पुन्हा पुन्हा (0.2)
logic gates        switches पासून बनलेले ठरवणारे भाग (1.5)
market size        problem किती लोकांची, किती खोल (0.2)
pixel              photo चा एक ठिपका; तीन numbers चा रंग (2.2)
program            machine साठी लिहिलेली recipe (1.3)
program counter    "आत्ता पाऊल क्रमांक __ वर" वाला खण (2.4)
RAM                वेगवान, विसराळू स्मरणशक्ती; कामाचं मेज (2.5)
sample             आवाजाच्या एका क्षणाचं माप; ~44,000/second (2.2)
scarcity           हे किती कमी लोकांना जमतं (0.2)
software           सगळ्या recipes, मिळून (1.3)
stack              मजल्यांचा मनोरा: कोण कोणावर उभा (0.3)
storage            हळू, पक्की स्मरणशक्ती; गोदाम (2.5)
stored-program computer
                   recipe ला data च्या जागी ठेवणारं design (1.6)
transistor         विजेने दाबला जाणारा switch (1.1)
universal machine  एक machine जी कुठलीही recipe चालवते (1.6)
```
