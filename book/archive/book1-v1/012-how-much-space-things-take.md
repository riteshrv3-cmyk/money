# Chapter 2.1  [SPINE]
## Ek cheez kitni jagah leti hai

---

### Samvaad

**Madhav:** Ek akshar rakhne ke liye kitne switch chahiye?

**Kabir:** Angrezi ke akshar 128 ki list mein aate hain, toh saat.

**Madhav:** Log aath istemaal karte hain. Ek fazool bacha lete hain kyunki aath ka hisaab aasan hai. Ab ek shabd, paanch akshar ka?

**Kabir:** Chalis switch.

**Madhav:** Ek page, do hazaar akshar?

**Kabir:** Solah hazaar.

**Madhav:** Ek kitaab, teen sau page?

**Kabir:** Lagbhag paanch karod.

**Madhav:** Ab dhyaan do. Paanch karod switch. Ek switch ek baal se bahut chhota hai. Toh ek poori kitaab jagah leti hai...

**Kabir:** Bahut kam.

**Madhav:** Ab ek photo. Ek photo mein chhote dabbe hote hain, har dabbe ka apna rang. Ek aam phone ki photo mein lagbhag ek karod dabbe hote hain. Aur ek rang rakhne ke liye teen numbers chahiye: laal kitna, hara kitna, neela kitna. Har number aath switch. Toh ek photo?

**Kabir:** Ek karod guna teen guna aath. Chobees karod switch.

**Madhav:** Aur kitaab paanch karod thi. Toh ek photo ek kitaab se kitni badi hai?

**Kabir:** Paanch guna. Ek photo, paanch kitaabein.

**Madhav:** Ab video. Video kya hai?

**Kabir:** Bahut saari photos, ek ke baad ek.

**Madhav:** Ek second mein kitni?

**Kabir:** Tees ke aas-paas?

**Madhav:** Toh ek second ka video kitni kitaabein hua?

**Kabir:** Tees guna paanch. Ek sau pachas kitaabein. Ek second mein?

**Madhav:** Ek second mein. Ab ek ghante ka video ginti karo.

**Kabir:** Ek ghante mein 3,600 second. Yaani paanch lakh se zyada kitaabein.

**Madhav:** Ab ek sawal. Tumhare phone mein ghanton ke video hain. Toh phone mein karodon kitaabon jitni jagah hai?

**Kabir:** Nahi. Ho hi nahi sakti.

**Madhav:** Toh video usmein aata kaise hai?

**Kabir:** Kuch toh chhoda ja raha hoga.

**Madhav:** Kya chhoda ja sakta hai? Socho. Do lagatar photos mein, video ke andar, kitna farak hota hai?

**Kabir:** Bahut kam. Aadmi thoda hila, baaki sab wahi hai.

**Madhav:** Toh agar main pehli photo poori rakhun, aur uske baad sirf **farak** rakhun?

**Kabir:** Toh bahut kam jagah lagegi. Kyunki farak chhota hai.

**Madhav:** Aur ek hi photo ke andar? Aasman ka bada hissa ek jaisa neela hai. Kya karoge?

**Kabir:** Har dabbe ka rang alag se nahi rakhunga. Likh dunga: yeh rang, itne dabbon tak.

**Madhav:** Tumne abhi do sabse badi hoshiyaariyan khud nikaal li. Ek: jo cheez dohrayi ja rahi hai use ek baar likho. Do: jo cheez pehle jaisi hai use dobara mat likho, sirf farak likho.

---

### Naam

Aath bit ko ek **byte** kehte hain. Yeh sabse aam naap hai, kyunki ek angrezi akshar aksar ek byte leta hai.

Uske baad har kadam pe lagbhag ek hazaar guna:

```
1 byte            ek akshar
1 KB   (kilobyte) hazaar akshar          ek chhota paragraph
1 MB   (megabyte) das lakh akshar        ek moti kitaab
1 GB   (gigabyte) sau karod akshar       lagbhag ek hazaar kitaabein
1 TB   (terabyte) das lakh MB            ek chhoti library
```

Aur jo Kabir ne nikaala, us poore idea ka naam hai **compression**.

Uske do tareeke wahi hain jo usne bataye:

```
DOHRAV HATANA     "neela, neela, neela x 500"  →  "neela x 500"
FARAK RAKHNA      poori photo mat rakho, pichhli se farak rakho
```

Aur ek teesra bhi hai, jo sirf photo, awaaz aur video mein chalta hai:

```
JO DIKHTA HI NAHI USE PHENK DO
```

Insaan ki aankh kuch rangon ka halka farak pakad hi nahi paati. Kaan kuch awaazein sun hi nahi sakta. Toh unhe rakhna hi kyun.

Yahan se do tarah ki compression bantee hai:

```
LOSSLESS   kuch nahi khota. Wapas kholo toh bilkul wahi milta hai.
           Likhavat, program, hisaab. Yahan ek bit bhi kho nahi sakta.

LOSSY      kuch hamesha ke liye chala jaata hai.
           Photo, gaana, video. Jo aankh-kaan pakad nahi paate, woh gaya.
```

Isiliye ek program ki file ko lossy compression nahi karte. Ek bhi number badal jaaye toh program chalega hi nahi. Lekin ek photo mein hazaaron numbers badal do, aankh ko pata bhi nahi chalega.

---

### Asli duniya se ek example

Ek aam phone ki photo agar kuch chhoda hi na jaaye toh lagbhag 30 MB ki hoti hai. Jab woh aapke phone mein JPEG bankar aati hai, toh woh 2 se 4 MB ki hoti hai.

Yaani lagbhag 90 pratishat phenk diya gaya, aur aapko dekh kar farak mushkil se pata chalta hai.

Video mein yeh aur zyada hai. Ek ghante ka bina kuch chhode video kai hazaar GB ka hota. Netflix aapko wahi ghanta lagbhag 3 GB mein bhej deta hai. Yaani hazaar guna se zyada nichod diya gaya.

Aur yeh sirf jagah bachane ki baat nahi hai. **Compression ke bina video internet pe chal hi nahi sakta tha.** Taar utna data le hi nahi ja sakte. YouTube, Netflix, video call, ye sab ek hisaab ki wajah se mumkin hain, kisi naye taar ki wajah se nahi.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **yeh sochna ki compression se kuch khota nahi.**

Log ek photo ko baar baar WhatsApp pe bhejte hain aur poochte hain ki woh dhundhli kyun ho gayi. Har baar bhejne pe compression dobara lagti hai, aur har baar thoda aur phenka jaata hai.

Isi tarah, ek lossy file ko wapas "poora" nahi kiya ja sakta. Jo phenk diya gaya woh gaya. Koi app use wapas nahi la sakta, chahe woh kuch bhi daawa kare. Woh sirf andaza laga kar naya bana sakta hai.

Yeh galti tempting isliye hai ki photo dekhne mein waisi hi lagti hai. Aankh ko farak nahi dikhta, toh dimaag maan leta hai ki farak hai hi nahi.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  COMPRESSION  dohrav hatao, farak rakho│  ← naya
    ├────────────────────────────────────────┤
    │  SIZE         byte, KB, MB, GB         │  ← naya
    ├────────────────────────────────────────┤
    │  PROGRAM      nirdesh bhi numbers hain │
    ├────────────────────────────────────────┤
    │  ENCODING     number ka matlab         │
    ├────────────────────────────────────────┤
    │  BINARY, SHARTEIN, SWITCH              │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

Har sawal pe ek minute socho, phir neeche jawab padho.

**1. (samajh check)** Do photos hain. Ek mein saaf neela aasman hai. Doosri mein ek ped hai jismein hazaaron patte hain. Dono ka size ek jaisa hai bina compression ke. Compression ke baad kaunsi chhoti hogi?

> **Jawab:** Aasman wali, aur bahut zyada chhoti.
>
> Aasman mein dohrav bahut hai. Lakhon dabbe lagbhag ek hi rang ke hain, aur unhe ek line mein likha ja sakta hai.
>
> Patton mein har dabba apne padosi se alag hai. Dohrav hai hi nahi, toh hatane ko kuch nahi hai.
>
> Isse ek gehri baat nikalti hai: **compression dohrav pe chalti hai. Jitna zyada dohrav, utni zyada bachat.** Aur jis cheez mein koi dohrav na ho, use compress kiya hi nahi ja sakta.

**2. (samajh check)** Aap ek zip file banate ho, phir usi zip file ko dobara zip karte ho. Doosri baar mein kitni jagah bachegi?

> **Jawab:** Lagbhag kuch nahi. Aksar file thodi **badi** ho jaati hai.
>
> Kyunki pehli zip ne saara dohrav pehle hi nikaal diya. Jo bacha hai usmein koi pattern nahi hai.
>
> Aur zip file mein thodi si jaankari bhi rakhni padti hai ki kholna kaise hai. Woh jud jaati hai.
>
> Yeh saabit karta hai ki compression jaadu nahi hai. Woh dohrav ka faayda uthati hai. Dohrav khatam, faayda khatam.

**3. (jodne wala)** Chapter 1.4 kehta tha ki matlab andar nahi hota, bahar se aata hai. Compression usse kaise judti hai?

> **Jawab:** Compressed file ke numbers dekh kar aapko kuch samajh nahi aayega. Woh asli photo ke numbers se bilkul alag hain.
>
> Unka matlab tabhi banta hai jab aap kholne ka sahi tareeka lagayein. Galat tareeka lagao, bakwaas milega.
>
> Toh compression ek aur parat hai, usi dher pe. Photo ke numbers ke upar, ek aur encoding.
>
> Isiliye `.jpg` aur `.png` alag hote hain. Andar dono photo hain, lekin nichodne ka tareeka alag hai, toh kholne ka tareeka bhi alag hai.
