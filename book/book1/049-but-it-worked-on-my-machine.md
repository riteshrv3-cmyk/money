# Chapter 7.4  [DEPTH]
## "Mere machine pe toh chal raha tha"

---

*DEPTH chapter. Yeh software banane ka sabse purana mazaak hai, aur uska hal poore internet ki shakal badal chuka hai.*

---

### Samvaad

**Madhav:** Ek program aapke laptop pe theek chalta hai. Server pe daala aur woh nahi chala. Wajah kya ho sakti hai?

**Kabir:** Alag machine hai.

**Madhav:** Kya alag hai? Ginti karo.

**Kabir:** OS alag ho sakta hai. Version alag ho sakta hai.

**Madhav:** Aur?

**Kabir:** Jo doosri cheezein program istemaal karta hai, unke version alag ho sakte hain.

**Madhav:** Aur?

**Kabir:** Settings alag ho sakti hain. Files alag jagah ho sakti hain.

**Madhav:** Aur ek aur, jo sabse zyada hoti hai. Aapke laptop pe kuch aisa hai jo aapne mahine pehle lagaya tha aur aap bhool gaye.

**Kabir:** Aur server pe woh nahi hai.

**Madhav:** Ab batao, kitni cheezein ek jaisi honi chahiye?

**Kabir:** Sab.

**Madhav:** Toh?

**Kabir:** Toh main ek list bana lun ki kya kya chahiye.

**Madhav:** Aur agar list adhoori ho? Kyunki jo cheez aap bhool gaye ho, woh list mein bhi nahi hogi.

**Kabir:** Toh list bekaar hai.

**Madhav:** Ek doosra tareeka socho. List banane ki jagah, kya bheja ja sakta hai?

**Kabir:** Poori machine bhej doon?

**Madhav:** Kaise?

**Kabir:** Ek poori machine ki copy... woh toh bahut bhaari hoga. Poora OS.

**Madhav:** Bhaari hai, aur log ne pehle wahi kiya tha. Ab socho: kya poora OS bhejna zaroori hai?

**Kabir:** Nahi. Server pe toh pehle se ek OS hai.

**Madhav:** Toh kya chahiye?

**Kabir:** Sirf mera program aur woh cheezein jo woh istemaal karta hai. Baaki neeche wala hissa saanjha ho sakta hai.

**Madhav:** Aur agar do program ko alag alag version chahiye ek hi cheez ka?

**Kabir:** Toh dono apna apna leke chalein, aur ek doosre ko na dekh sakein.

**Madhav:** Yeh kaunsi soch hai? Kahan dekh chuke ho?

**Kabir:** Chapter 3.4. OS har app ko alag rakhta hai.

**Madhav:** Bas. Wahi soch, ek parat upar. Ab ek aakhri sawal. Agar poora dabba ek hi jaisa chal sakta hai kahin bhi, toh usse aur kya kya mumkin hua?

**Kabir:** Main use kahin bhi utha kar rakh sakta hoon.

**Madhav:** Aur agar bojh badhe?

**Kabir:** Toh usi dabbe ki das copy chala doon.

**Madhav:** Aur ek mar jaaye?

**Kabir:** Nayi chala dun. Woh bilkul waisi hi hogi.

**Madhav:** Ab tumne dekha ki yeh sirf ek jhanjhat ka hal nahi tha. Isne poori Part 6 wali duniya ko aasan bana diya.

---

### Naam

Us dabbe ka naam hai **container**, aur sabse mashhoor tareeke ka naam **Docker** hai.

Farak samajhna zaroori hai:

```
POORI MACHINE KI COPY (virtual machine)
├── poora OS andar
├── bhaari: GB mein
├── shuru hone mein minute
└── poora alagav

DABBA (container)
├── sirf program aur uski cheezein
├── neeche ka OS saanjha
├── halka: MB mein
├── shuru hone mein second
└── kaafi alagav, poora nahi
```

Aur woh cheez jo iss chapter ki asli seekh hai:

**Container ne "chalta kaise hai" ko "chalta kahan hai" se alag kar diya.**

Pehle ek program aur ek machine bandhe hue the. Program us machine ke liye banaya jaata tha.

Ab program ek dabbe mein hai jo kahin bhi chal sakta hai. Machine sirf ek jagah hai jahan dabba rakha ja sakta hai.

Aur isse teen cheezein apne aap aa gayin, jo Part 6 mein bahut mehnat maangti thin:

```
BADA HONA      dus copy chala do (Chapter 6.1)
BADALNA        purana dabba hatao, naya rakho, sekend mein
CHALTE RAHNA   ek mar gaya toh naya utha do (Chapter 6.2)
```

Aur jab dabbe hazaaron ho jaate hain, toh unhe koi sambhalta hai: kaun kahan chalega, kaun mar gaya, kaun naya chahiye. Us kaam ke liye ek aur parat hai, jiska sabse aam naam **Kubernetes** hai.

Ab dhyaan do ki yeh kya hua. **Ek manager, jo dabbon ko machinon pe baantta hai.**

Chapter 3.4 mein OS programs ko ek machine pe baant raha tha. Ab wahi soch machinon ke poore jhund pe lag gayi.

**Ek hi shakal, teesri baar.**

---

### Asli duniya se ek example

2013 mein Docker aane se pehle, ek naye engineer ko apne laptop pe kaam shuru karne mein aksar do se paanch din lagte the. Ek lambi list hoti thi, aur usmein se aadhi cheezein purani ho chuki hoti thin.

Aaj wahi kaam aksar ek hukum aur kuch minute ka hota hai.

Aur uska asar sirf suvidha nahi tha. Chapter 6.8 yaad karo: **aadmi ka waqt machine se bahut mehnga hai.** Har naye aadmi ke teen din bachana, har baar, poori company mein, ek bada aankda ban jaata hai.

Iska ek aur asar hua jo shayad bada tha. Jab ek program kahin bhi ek jaisa chal sakta hai, toh cloud companies ko badalna aasan ho gaya. Chapter 6.5 wala lock-in thoda kamzor ho gaya.

Aur isiliye cloud companies ne apni khud ki aur upar wali cheezein banayin, jo sirf unke yahan chalti hain. Lock-in hataya nahi gaya, woh ek parat upar chala gaya.

---

### Yahan log kya galat samajhte hain

Sabse aam galti: **container ko ek poori machine samajhna.**

Container ke andar apna OS nahi hota. Woh neeche wale OS ka istemaal karta hai. Isliye woh halka hai, aur isliye uska alagav utna sakht nahi hai jitna log sochte hain.

Iska seedha nateeja: log maan lete hain ki container ke andar ki cheez poori tarah band hai aur bahar kuch nahi kar sakti. Woh kaafi alag hai, lekin poori tarah nahi. Jahan suraksha sach mein zaroori hai, wahan poori machine ki copy aaj bhi istemaal hoti hai.

Doosri galti: **yeh sochna ki container se scaling apne aap ho jaayegi.**

Container ne dabba ek jaisa bana diya. Usne Chapter 6.1 wala niyam nahi badla: machine khaali honi chahiye. Agar aapka program apne andar jaankari rakhta hai, toh dus copy chalane se woh dus alag jhoot bolengi.

Container ne cheezein le jaana aasan kiya. Usne banawat ke faisle nahi badle.

---

### Map pe

```
    ┌────────────────────────────────────────┐
    │  CONTAINER    program + uski cheezein   │  ← naya
    │               kahin bhi ek jaisa        │
    │  MANAGER      ab machinon ke jhund pe   │
    │               (teesri baar wahi shakal) │
    ├────────────────────────────────────────┤
    │  VERSION CONTROL, JAANCH, BUG           │
    ├────────────────────────────────────────┤
    │  CLOUD, API, UPTIME, BADA HONA          │
    ├────────────────────────────────────────┤
    │  OS, CPU, RAM/DISK, SWITCH              │
    └────────────────────────────────────────┘
```

---

### Sochne ke liye

**1. (samajh check)** Do program ek hi machine pe chalne hain, aur dono ko ek hi cheez ke alag version chahiye. Bina container ke kya hoga?

> **Jawab:** Ek hi version lag sakta hai, toh ek program tootega.
>
> Aur aksar aisa hota tha ki ek program ke liye version badalne se doosra toot jaata tha, jise koi mahinon baad dhoondhta tha.
>
> Container mein dono apna apna leke chalte hain aur ek doosre ko dekhte bhi nahi.
>
> Yeh Chapter 3.4 ka "alag rakhna" hai, ek parat upar lagaya hua. **Ek hi problem, ek hi hal, naya paimana.**

**2. (samajh check)** Aapne apna program container mein daal diya aur uski das copy chala di. Ab log ki login baar baar chali jaati hai. Kya hua?

> **Jawab:** Program apne andar login ki jaankari rakh raha hai.
>
> Har copy apna alag rakh rahi hai, aur user har baar kisi doosri pe pahunch jaata hai.
>
> Container ne ise theek nahi kiya, kyunki yeh container ki problem thi hi nahi. Yeh Chapter 6.1 ka niyam hai: **machine khaali honi chahiye.**
>
> Sabak: **ek naya tool purane faisle theek nahi karta. Woh unhe sirf pehle saamne le aata hai.**

**3. (jodne wala)** Iss kitaab mein ab teen jagah "manager" aa chuka hai. Teeno ginao aur batao ki saanjha kya hai.

> **Jawab:**
>
> ```
> Ch 3.4   OS         programs ko ek machine pe baantta hai
> Ch 6.1   load balancer  users ko machinon pe baantta hai
> Ch 7.4   Kubernetes dabbon ko machinon ke jhund pe baantta hai
> ```
>
> Saanjha: jab ek cheez hai aur maangne wale kai, tab koi beech mein baithkar baantta hai, aur usse yaad rakhna padta hai ki kaun kahan hai.
>
> Aur har baar wahi sawal aate hain: agar manager mar jaaye toh? Agar do maangne wale atak jaayein toh? Agar ek maangne wala sab kuch le le toh?
>
> **Yeh iss kitaab ki sabse badi baat hai. Aap 112 cheezein yaad nahi kar rahe. Aap dus shakalein seekh rahe ho jo baar baar dikhti hain.**
