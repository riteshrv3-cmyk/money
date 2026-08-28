# PART 5 चा शेवट: नकाशा

## जे तुमच्याकडे आता आहे (Part 5)

```
SCALING          उभं (मोठी machine: भिंत) vs आडवं (अनेक +
                 load balancer); मंत्र: काम वाटा, आठवण एकत्र
UPTIME           मरणं गृहीत धरा: प्रती + मरण-ओळख + failover;
                 nines ची मोजपट्टी, प्रत्येक nine दहापट महाग
FRONT / BACK     dining hall vs kitchen; frontend वर कधीही
                 विश्वास नाही: खरी तपासणी kitchen मध्ये
API              program चं menu card; धंद्याचा दरवाजा;
                 वापरणारा भाडेकरू, देणारा जमीनमालक
CLOUD            दुसऱ्याच्या building मधल्या machines,
                 भाड्याने; लवचीकपणा हेच मोल, स्वस्ताई नाही
BOTTLENECK       साखळी = कमजोर दुवा; मीटर लावा; रुंद करा /
                 रांग लावा / दार आवळा; cascade + circuit breaker
LATENCY          second रस्त्यावर जातो: अंतर मारा (CDN) +
                 फेरे मारा + वजन घटवा
खर्च             bill च्या तीन ओळी: compute + storage +
                 egress; unit economics; bill shock चा गजर
दावा-तपासणी      पाच-प्रश्नांची चौकट: कुठल्याही धंद्याचा X-ray
जोडणी            60 seconds ची trace; सोपं-मध्यम-अवघड नकाशा;
                 सात-प्रश्नी spec; blameless postmortem;
                 जिंकण्याचे 5 नियम (जाळं, दरवाजा, खिळे,
                 वेळ, वाटप)
```

Book 1 ची परीक्षा मागच्या chapter मध्ये (8.6) झाली. पुढची दोन
पानं संदर्भासाठी आहेत: **पूर्ण पुस्तकाचा नकाशा** (भिंतीवर
लावण्यासाठी) आणि **master glossary** (पाचही parts चे शब्द एका
जागी). पुस्तक वाचून झाल्यावरही ही दोन पानं तुमच्या टेबलावर
जगतील: असा हेतू आहे.

# PART 5 चा MINI-GLOSSARY

```
API              programs चं ठरलेलं प्रश्नोत्तर-menu (7.4)
bottleneck       साखळीतला सगळ्यात अरुंद दुवा (7.6)
cascade          हळा भाग -> retries -> कोसळत जाणं (7.6)
CDN              जगभरच्या godowns मधल्या प्रती (7.7)
circuit breaker  आजारी भागाला श्वास: विचारणं थांबवणं (7.6)
cloud / region   भाड्याच्या machines / त्यांचं शहर-घर (7.5)
compute          CPU-वेळेचं भाडं; bill ची ओळ 1 (7.8)
egress           बाहेर जाणाऱ्या data ची जकात; ओळ 3, कपटी (7.8)
elastic          गरजेप्रमाणे ताणणारं-आकसणारं भाडं (7.5)
failover         मुख्य मेला की प्रत आपोआप पुढे (7.2)
frontend/backend दिसणारा भाग / kitchen; विश्वास फक्त kitchen वर (7.3)
full-stack       दोन्ही बाजू करणारा developer (7.3)
health check     "जिवंत आहेस?" ची नियमित विचारणा (7.2)
load balancer    दारावरचा वाटप करणारा (7.1)
load test        नकली गर्दीने आधीच सराव (7.6)
lock-in          एका मालकात खोल रुतणं; घर बदलणं महाग (7.5)
metrics          प्रत्येक भागावरचे मीटर (7.6)
network effect   प्रत्येक नवा user जुन्यांची किंमत वाढवतो (8.5)
nines / SLA      उपलब्धतेची मोजपट्टी / तिचं लिखित वचन (7.2)
postmortem       तुटल्यावर व्यवस्थेचं (blameless) विच्छेदन (8.4)
rate limit       दार आवळणं: प्रति-user मर्यादा (7.6)
rolling deploy   एक-एक counter बदलणं, दुकान चालू ठेवून (7.2)
spec             नेमकं-काय-हवं ची सात-प्रश्नी मागणी (8.3)
stateless        server रिकामा; state सामायिक जागी (7.1)
switching cost   सोडून जाण्याची वेदना = खिळे (8.5)
unit economics   एका user मागचा खर्च vs कमाई (7.8)
vertical/horizontal
                 उभं वाढणं / आडवं वाढणं (7.1)
```
