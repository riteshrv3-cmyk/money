# Chapter 4.4  [SPINE]
## Rules pe pehle se agree karna

---

### Samvaad

**Madhav:** Ek packet pahunch gaya. Usmein numbers hain. Lene wali machine ab kya kare?

**Kabir:** Padhe.

**Madhav:** Kaise? Chapter 1.4 yaad karo.

**Kabir:** Andar sirf numbers hain, matlab bahar se aata hai. Toh use pata hona chahiye ki inhe kaise padhna hai.

**Madhav:** Aur use kaise pata chalega?

**Kabir:** Bhejne wala bata de.

**Madhav:** Kis shakal mein batayega?

**Kabir:** Numbers mein hi.

**Madhav:** Aur un numbers ko kaise padhega?

**Kabir:** Hmm. Yeh toh ghoom raha hai.

**Madhav:** Bilkul ghoom raha hai. Toh iska ek hi hal hai. Batao.

**Kabir:** Dono ko pehle se pata hona chahiye. Baat shuru hone se pehle.

**Madhav:** Bas. Ek aisa niyam jo dono taraf pehle se maujood ho, aur jise koi bhi baat-cheet mein tay na kiya jaaye. Ab woh niyam kaisa dikhega? Ek chitthi socho. Usmein kya hoga?

**Kabir:** Upar kuch jaankari, phir asli baat.

**Madhav:** Aur padhne wale ko kaise pata chalega ki jaankari khatam hui aur asli baat shuru?

**Kabir:** Beech mein koi nishaan hoga.

**Madhav:** Aur asli baat kitni lambi hai, yeh kaise pata chalega?

**Kabir:** Ya toh upar likha ho, ya aakhir mein koi nishaan ho.

**Madhav:** Tumne ek poora protocol bana liya. Ab ek asli wala dekhte hain. Tum ek website kholte ho. Tumhara browser server se kya kehta hai?

**Kabir:** "Mujhe yeh page do."

**Madhav:** Aur usmein kya kya likhna padega?

**Kabir:** Kaunsa page. Aur shayad ki main kaun hoon.

**Madhav:** Aur kya batana chahoge?

**Kabir:** Ki main kaunsi bhasha samajhta hoon. Ki mera phone chhota hai ya bada.

**Madhav:** Aur server kya wapas bhejega?

**Kabir:** Page. Aur yeh bhi ki mila ya nahi mila.

**Madhav:** Kyun batayega ki mila ya nahi? Page bhej hi diya, kaafi nahi?

**Kabir:** Kyunki page na milna bhi ek jawab hai. Aur galti bhi ho sakti hai.

**Madhav:** Toh tumhe alag-alag jawab chahiye: mil gaya, nahi mila, tumhe ijaazat nahi hai, server kharab hai.

**Kabir:** Aur unhe numbers de dete honge, taaki chhota rahe.

**Madhav:** Bilkul. Ab aakhri sawal, aur yeh sabse zaroori hai. Yeh niyam kisne banaya?

**Kabir:** Kisi company ne?

**Madhav:** Agar ek company banati, toh baaki kyun maanteen?

**Kabir:** Nahi maanteen. Sabko milkar tay karna padega.

**Madhav:** Aur ek baar tay ho jaaye toh?

**Kabir:** Toh use badalna bahut mushkil hoga. Sabko ek saath badalna padega.

**Madhav:** Wahi baat jo IPv6 mein dekhi thi. Ab tum internet ka asli dhaancha samajhne lage ho.

---

### Naam

Aise pehle se tay niyam ko **protocol** kehte hain.

Protocol tay karta hai:

```
sandesh ki shakal kya hogi
kaunsa hissa jaankari hai, kaunsa asli baat
kaun pehle bolega
jawab kaise dikhega
galti kaise batayi jaayegi
```

Web ka protocol **HTTP** hai. Uska ek request kuch aisa dikhta hai:

```
GET /photo.jpg              ←  kya chahiye
Host: example.com           ←  kis jagah se
Accept-Language: hi         ←  kaunsi bhasha
                            ←  khaali line: jaankari khatam
```

Aur jawab:

```
200  mil gaya
404  woh cheez hai hi nahi
403  hai, lekin aapko ijaazat nahi
500  server ke andar kuch toot gaya
```

Ab woh baat jo iss chapter ko aage tak le jaati hai.

**Protocol ke bina do ajnabi baat nahi kar sakte.** Aur protocol koi bhej nahi sakta, kyunki bhejne ke liye bhi protocol chahiye.

Isliye har protocol pehle se maujood hona hi padta hai. Aur isliye protocol badalna lagbhag namumkin hai, kyunki sabko ek saath badalna padega.

Aur yahin se ek badi karobaari baat nikalti hai: **jo protocol tay karta hai, woh us poore ilaake ki shakal tay kar deta hai, hamesha ke liye.** Woh us cheez ka maalik nahi hota, lekin uske baad har koi uske hisaab se hi chalta hai.

---

### Asli duniya se ek example

HTTP 1991 mein banaya gaya, ek aadmi ne, ek research lab mein: Tim Berners-Lee.

Usne aur uske saath ke logon ne teen cheezein banayin: page likhne ka tareeka (HTML), page maangne ka tareeka (HTTP), aur page ka pata (URL).

Phir unhone woh sab kuch **kisi ko bhi, muft** de diya. CERN ne 1993 mein saaf likh kar de diya ki koi bhi ise bina paise ke istemaal kar sakta hai.

Ab Chapter 3.6 wale chaar wajahon pe lagao. Agar unhone iska paisa maanga hota, toh kya hota?

Log doosra tareeka bana lete, ya sab alag-alag tareeke banate aur koi kisi se baat na kar pata. Web ki poori value hi iss baat mein thi ki sab ek hi niyam maanein. Paisa maangna us value ko hi maar deta.

Toh muft dena daan nahi tha. Woh ek hi tareeka tha jisse woh cheez kaam kar sakti thi.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **"internet" aur "web" ko ek hi cheez samajhna.**

Internet woh jaal hai: pate, packet, taar. Web usme se ek cheez hai jo uske upar chalti hai, HTTP ke through.

Email alag protocol pe chalta hai. Video call alag pe. Aapke phone ke app aksar apne khud ke tareeke istemaal karte hain.

Yaani web internet ka ek kirayedaar hai, maalik nahi.

Yeh galti tempting isliye hai ki zyadatar log internet ko browser ke through hi dekhte hain, toh dono ek hi lagte hain.

Iska seedha nateeja: log samajh nahi paate ki ek app bina browser ke kaise chalta hai, ya ki internet band kiye bina sirf ek cheez kaise band ki ja sakti hai. Alag protocol, alag raaste, alag taale.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  PROTOCOL     pehle se tay niyam        │  ← naya
    │               badalna lagbhag namumkin  │
    ├────────────────────────────────────────┤
    │  PACKET, TCP/UDP, PATA, NETWORK         │
    ├────────────────────────────────────────┤
    │  OS, PROCESS, CPU, RAM/DISK, SWITCH     │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Ek website kholi aur "404" aaya. Kya hua, aur kya yeh aapki galti hai ya server ki?

> **Jawab:** Server ne kaha ki us pate pe koi cheez hai hi nahi.
>
> Server theek chal raha hai. Usne aapki baat samajh li aur jawab bhi de diya. Bas woh cheez wahan nahi hai.
>
> Yeh 500 se alag hai, jismein server khud toot gaya hota hai. Aur 403 se bhi alag, jismein cheez hai lekin aapko ijaazat nahi.
>
> Yeh farak zaroori hai: **"nahi mila" aur "main toot gaya" do bilkul alag baatein hain**, aur unke ilaaj bhi alag hain.

**2. (samajh check)** Do log alag-alag desh mein hain, alag company ke phone, alag internet company. Phir bhi unka message pahunch jaata hai. Kaise?

> **Jawab:** Kyunki dono taraf wahi protocol pehle se maujood hai.
>
> Kisi ne beech mein tay nahi kiya. Woh niyam saalon pehle likhe gaye the aur dono ke phone unhi ke hisaab se bane hain.
>
> Yeh internet ka sabse bada karnama hai: **koi milkar tay nahi karta, sab pehle se tay hai.**
>
> Aur isiliye internet ka koi maalik nahi hai. Uske paas ek sarkar nahi hai, sirf kuch likhe hue kagaz hain jinhe sab maante hain.

**3. (jodne wala)** Chapter 3.6 mein hum ne poocha tha ki free cheezein kyun exist karti hain. HTTP ka muft hona un chaar wajahon mein se kaunsi hai?

> **Jawab:** Teesri, aur sabse teekhi shakal mein: **neeche wali parat pe kabza.**
>
> Lekin ek farak ke saath. Yahan kisi ne upar bechne ke liye neeche free nahi kiya. Yahan cheez ki value hi iss baat mein thi ki sab ek hi niyam maanein.
>
> Toh yeh ek nayi baat sikhata hai: **kuch cheezein sirf tab kaam karti hain jab sab unhe maanein. Aisi cheezon ka daam maangna unhe maar dena hai.**
>
> Yeh baat protocol, bhasha, naap-tol aur paise pe laagu hoti hai. Aur yeh yaad rakhna zaroori hai jab aap kuch banane ki soch rahe ho: kya aapki cheez ki value akele mein hai, ya sirf sehmati mein?
