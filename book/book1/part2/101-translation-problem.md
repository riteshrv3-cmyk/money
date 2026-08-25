# Chapter 3.1 [SPINE]: Translation problem

Part 1 ka aakhri sach yeh tha: CPU sirf numbers wale kadam samajhta
hai (machine code). 3 matlab jodo, 7 matlab chhalaang. Bas.

Toh 1940s ke pehle programmers ne kya kiya? Sach mein numbers hi
likhe. Kaagaz pe kadam sochte the, phir har kadam ka number tay
karte the, phir switchon aur cards se machine mein bharte the. Ek
chhoti si recipe mein hafta lagta tha, aur ek number galat toh sab
kachra, aur galti DHOONDHNA likhne se bhi mushkil.

Ab aap 1950 ke engineer ho. Yeh dard roz jhel rahe ho. Kya karoge?

Pehla kadam khud dikh jaata hai: numbers ke NAAM rakh do. "3" ki
jagah likho "ADD", "7" ki jagah "JUMP". Insaan naam padh sakta hai,
galti dikh jaati hai. Lekin machine toh naam nahi samajhti... toh ek
chhota program likho jo naam ko wapas number bana de. Yeh tarjuma
itna seedha hai (har naam = ek number) ki program aasaan tha.

Ruko. Yahan jo hua woh dhyaan se dekho, kyunki yeh poori software
duniya ka janam hai: **tarjuma karne ka kaam khud ek recipe ban
gaya.** Machine apni hi bhasha ka pul khud banati hai.

Ab agla dard. Naam number se behtar hain, lekin sochna ab bhi
machine ke level pe padta hai: "yeh uthao, wahan rakho, jodo,
chhalaang maaro." Insaan aise nahi sochta. Insaan sochta hai: "har
customer ka bill jodo aur sabse bada dikhao." Ek line, jisme machine
ke sau kadam chhupe hain.

Toh sapna bana: aisi bhasha jo insaan ki soch ke PAAS ho, aur ek
mota translator jo us ek line ko machine ke sau kadmon mein khol de.
Yeh translator ab seedha naam-badalna nahi hai, yeh asli tarjuma
hai: samajhna, todna, jamana. Mushkil program hai. Lekin ek baar ban
jaaye (leverage yaad hai?), toh har programmer hamesha ke liye
insaan ke level pe likh sakta hai.

Yeh ban gaya (1957 se shuru), aur tab se poori industry isi seedhi
pe upar chadh rahi hai: machine se door, insaan ke paas. Aakhri
kadam aap roz dekhte ho: aap Claude ko HINDI mein bolte ho aur code
ban jaata hai. Woh isi 70 saal purani seedhi ka sabse naya danda
hai.

## NAAM

Numbers wali bhasha: **machine code**. Naam wali: **assembly**.
Insaan ke paas wali bhaashaein: **programming languages** (Python,
Java, C, aage aayengi). Tarjuma karne wala program: **translator**
(iske do roop Chapter 3.3 mein). Is seedhi mein "machine se kitna
door" ko log **level** kehte hain: assembly low-level, Python
high-level. (Yeh "level" hamare 4-level stack se alag shabd hai,
dhyaan rahe.)

## ASLI DUNIYA SE EK EXAMPLE

Aapke phone mein yeh poori seedhi ek saath zinda hai. WhatsApp ke
engineers ne high-level bhasha mein likha. Translator ne use machine
code banaya. Ab aapka CPU numbers chala raha hai. Koi bhi manzil
gayab nahi hui, bas har manzil apne neeche wali ko chhupa deti hai.
Abstraction, Chapter 0.4 wala, yahan poori shakal mein khada hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Computer ab English samajhne laga hai." Nahi. CPU aaj bhi WAHI
numbers samajhta hai jo 1950 mein samajhta tha. Jo badla woh
TARJUMA hai: beech ki manzilein itni achhi ho gayin ki insaan ko
machine dikhna band ho gayi. Jab AI aapki Hindi se code banata hai,
toh bhi aakhir mein wahi 3 aur 7 wale numbers chal rahe hain. Seedhi
lambi hui hai, zameen wahi hai.

## MAP PE

Kaun kamata hai: har manzil pe alag log. Machine code ke paas
duniya ke sabse kam log (chip companies mein, sabse unchi tankhwah
prati aadmi). High-level pe crores log (aam software jobs). Aur ab
sabse upar wali manzil (AI se code banwana) sabse nayi hai, wahan
abhi bheed kam hai aur niyam ban rahe hain. Naya danda khulte hi
sabse pehle chadhne wale sabse zyada kamaate hain, har baar yahi
hua hai.

## KHUD DEKHO (5 minute)

Laptop pe koi bhi website kholo, khali jagah pe right-click karo,
"View Page Source" dabao. Jo dikha, woh us page ki recipe hai
(HTML). Ghabrao mat, padhna nahi hai. Bas yeh dekho ki har sundar
page ke neeche yeh text baitha hai, aur yeh text bhi aakhir mein
numbers ban ke hi chala. Parde ke peeche jhaankna aadat bana lo.

## SOCHNE KE LIYE

1. (derivation) Machine ko seedha Hindi ya English kyun nahi samjha
dete, beech ki bhaashaein hata ke? Kya rukavat hai?

> **Jawab:** Insaan ki bhasha mein matlab aadha bola jaata hai,
> aadha samjha jaata hai. "Thoda sa daal dena" mein kitna? Machine
> ko har kadam EXACT chahiye, kyunki uske paas "samajh jaao na"
> wala mode nahi hai (Chapter 1.5: sab pehle se tay). Isliye beech
> ki bhasha chahiye jisme matlab ka sirf ek roop ho. AI yahan
> pehli asli koshish hai: woh aapki adhoori baat ka matlab
> GUESS karta hai, phir exact code banata hai. Lekin guess kabhi
> kabhi galat hota hai, isliye AI ke zamaane mein bhi aakhri
> zimmedari wahi hai: exact kya chahiye, yeh AAPKO pata hona
> chahiye. Isi liye aap yeh kitaab padh rahe ho.
