# Chapter 2.1 [SPINE]: Ek cheez kitni jagah leti hai

Kapda meter mein napta hai, doodh litre mein, aur digital cheezein?
Aapne naam sune hain: MB, GB. Ab unhe kamaane layak samajh lete hain.

Naap ki ikai wahi hai jo Chapter 1.4 mein bani: **bit**, ek switch ki
haalat. Aath bit ka jhund **byte**. Ek byte mein 256 haalat aati hain,
itna kaafi hai ek akshar rakhne ke liye. Toh ek moti baat pakdo:

**1 byte = lagbhag 1 akshar.**

Ab seedhi ginti, har kadam pe hazaar ka guna:

```
1 KB (kilobyte)  = ~1 hazaar byte     = ek paragraph
1 MB (megabyte)  = ~10 lakh byte      = ek moti kitaab ka text
1 GB (gigabyte)  = ~100 crore byte    = 1,000 moti kitaabein
1 TB (terabyte)  = ~1 lakh crore byte = ek chhoti library
```

Ab asli duniya ke anchors, yeh ratne laayak hain kyunki har baat-cheet
mein aayenge:

```
WhatsApp message (sirf text)     ~ 100 byte
Ek photo (phone camera)          ~ 3 MB
Ek gaana                         ~ 5 MB
Ek ghanta video call             ~ 500 MB - 1 GB
Ek movie (achhi quality)         ~ 2-4 GB
Aapke phone ka poora storage     ~ 128-256 GB
```

Ek pattern dikh raha hai? Text nanha hai. Photo usse hazaar guna.
Video photo se bhi sau guna. **Text : photo : video = 1 : hazaar :
lakh.** Yeh anupaat is poori kitaab ka sabse kaam ka number hai,
kyunki jahan size hai wahan kharcha hai.

Kyun aisa? Text mein har akshar ek byte hai. Photo mein har bindu
(pixel) ke teen byte hain, aur bindu lakhs mein hain. Video mein har
second pe 30 photos hain. Ginti khud guna hoti jaati hai.

## NAAM

In naapon ka poora parivaar **storage units** kehlata hai. Ek baareek
baat: internet ki speed **bits** mein napti hai (Mbps = megabits per
second), storage **bytes** mein (MB). Bit byte ka aathvan hissa hai.
Isliye "100 Mbps" ka connection ek second mein sirf 12.5 MB laata hai.
Telecom companies bits mein isliye bolti hain kyunki number aath guna
bada dikhta hai. Ab aap yeh chaal pakad sakte ho.

## ASLI DUNIYA SE EK EXAMPLE

WhatsApp par bheji photo halki kyun ho jaati hai? Kyunki WhatsApp use
bhejne se pehle daba deta hai (compress): 3 MB se ~100 KB, tees guna
chhoti. Karodo photos roz jaati hain; agar full size jaati, toh
WhatsApp ka data kharcha tees guna hota aur aapka data pack bhi. Ek
compression ki recipe ne company ke arabon bachaye. Size ka intezaam
hi paisa hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

Log KB, MB, GB ko bas "chhota, bada, aur bada" samajhte hain. Nahi:
har kadam HAZAAR ka guna hai. MB aur GB ka farq wahi hai jo 1 rupaye
aur 1,000 rupaye ka. Jab engineer kahe "yeh file GB mein hai," toh
woh keh raha hai "yeh MB wali se hazaar guna bhaari hai," aur uska
kharcha bhi waisa hi hoga.

## MAP PE

Rupaye ka rasta: aap Google ko storage ka kiraya dete ho (Google One:
100 GB ke liye mahina ~130 rupaye). Google woh data jinke machines pe
rakhta hai, unki disks Samsung/Seagate se aati hain. Neeche tak jao
toh ek zaroorat milegi: "meri yaadein na khoyein" (Level 1: yaadon ki
hifaazat). Us zaroorat ka poora stack: photos app (L2 service), cloud
storage (L3), disk factory (L3 ka hardware kona). Har GB kiraya de
raha hai.

## KHUD DEKHO (5 minute)

Phone mein koi ek photo kholo, uski details/info dekho (size milega,
~2-4 MB). Ab ek text message ka size socho (~100 byte). Ab khud gino:
ek photo kitne messages ke barabar hai? (~30,000). Ab samjho ki data
pack video dekhne se hi kyun khatam hota hai, text se kabhi nahi.

## SOCHNE KE LIYE

1. (derivation) Do startup ideas: ek mein log 200-word reviews likhte
hain, doosre mein log 1-minute video reviews banate hain. Dono ke 10
lakh users hain. Sirf size ke gyaan se batao: kiska kharcha kitna
zyada hoga, aur iska business pe kya asar padega?

> **Jawab:** Text review ~1 KB, video review ~50-100 MB: farq lagbhag
> LAKH guna. Toh video wale ka storage aur bhejne ka kharcha bhi
> hazaaron-lakhon guna hoga. Asar: text wala app muft users pe bhi
> zinda reh sakta hai, video wale ko pehle din se paise ka raasta
> chahiye (ads, subscription), warna har naya user use gareeb karta
> hai. Product ki shakal uske business model ki shakal tay kar deti
> hai. Yeh formula ab aapke paas hai, kisi bhi idea pe lagao.
