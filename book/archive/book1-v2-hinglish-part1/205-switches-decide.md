# Chapter 1.5 [DEPTH]: Switches decide kaise karte hain

(Yeh DEPTH chapter hai. Pehli baar mein bhaari lage toh aage badho, Part
1 khatam karke lautna. Lekin laut zaroor aana, kyunki yahin pe "machine
sochti hai" wala jaadu poora tootta hai.)

Chapter 1.3 mein humne maana tha ki "jodne ka dibba" aur "compare karne
ka dibba" ban sakte hain. Ab banate hain. Sirf teen chhote purze chahiye,
teeno switchon se bante hain:

**AND:** do raaste ek ke baad ek (line mein). Bijli tabhi paar hogi jab
DONO switch on hon. Matlab: "dono haan, toh haan."

**OR:** do raaste side by side (samanantar). Bijli paar hogi agar KOI
BHI ek on ho. Matlab: "koi bhi haan, toh haan."

**NOT:** ulta karne wala. Input 1 toh output 0, input 0 toh output 1.

Bas. Yeh teen hi hain. Ab inse kaam karwao.

**Compare banao:** "Kya A aur B alag hain?" Socho: alag ka matlab hai
(A haan, B na) YA (A na, B haan). Yeh toh AND, OR, NOT ka jod hai:
(A AND (NOT B)) OR ((NOT A) AND B). Ho gaya. Machine ab "alag hai ya
nahi" bata sakti hai. Aur "barabar hai?" uska NOT hai.

**Jodna banao:** ek bit jodo: 0+0=0, 0+1=1, 1+0=1, 1+1=10 (do bits ka
jawab: "0 likho, 1 haath mein"). Dekho, jawab ka pehla hissa "alag
hain?" wala purza hai, aur haath wala hissa AND hai (dono 1 hon tabhi
haath mein jaata hai). School wali jod ki recipe, switchon mein utar
gayi. Aise 64 jodo, aur 64-bit numbers ka jod tayyar.

**"Agar" banao:** "AGAR yeh 1 hai TOH is taar ka signal aage jaane do."
Yeh sirf ek AND hai: signal AND shart. Recipe ka har "agar aisa toh
waisa" aakhir mein inhi AND/OR/NOT ki chain hai.

Ab poora minaar neeche se upar dekho:

```
transistor  ->  AND/OR/NOT  ->  jod/compare/agar  ->  recipe ke kadam
            ->  poora program  ->  WhatsApp
```

Har manzil apne neeche wali manzil ke purzon se bani hai. Kahin bhi,
kisi bhi manzil pe, "soch" naam ka koi purza nahi hai. Sirf switch hain,
design mein jade hue.

## NAAM

In purzon ka naam **logic gates** hai. AND gate, OR gate, NOT gate.
"Logic" isliye ki yeh haan/na wale tarkon ko bijli mein utaarte hain.
Aapke phone ki chip in gates ke arabon jodon se bani hai, aur gates
transistors se.

## ASLI DUNIYA SE EK EXAMPLE

ATM ka faisla: "paise do AGAR pin sahi hai AND balance kaafi hai AND
aaj ki limit baaki hai." Teen shartein, ek AND chain. Jis din aap ATM
se paisa nikaalte ho, ek AND gate ka jhund aapke haq mein 1 bolta hai.
Bank ka poora risk intezaam aise hi gates ki chains mein likha hai.

## YAHAN LOG KYA GALAT SAMAJHTE HAIN

"Machine decide karti hai, matlab uske andar kahin koi chhota dimaag
hai." Ab aap jaante ho decide ka matlab kya hai: pehle se design ki
hui AND/OR/NOT ki chain, jisme har possible input ka output PEHLE SE
tay hai. Machine ke paas surprise nahi hota. Jab machine ka jawab
aapko surprise kare, toh matlab aap design nahi jaante, machine kuch
naya nahi soch rahi.

## MAP PE

Kaun kamata hai: chip design karne wale. Gates ko jodkar tez, chhoti,
kam bijli wali chain banana duniya ki sabse scarce skills mein hai.
Nvidia isi khel mein duniya ki sabse keemti companies mein pahunchi:
unke gates ka intezaam AI ke kaam ke liye sabse tez nikla. Jo cheez
aapne aaj 15 minute mein samjhi, usi ki behtareen jamawat kharabon
dollar ki company banati hai. Farq gehraai ka hai, idea ka nahi.

## KHUD DEKHO (5 minute)

Kaagaz pe yeh table khud banao, bina dekhe: A aur B ke chaar jod
(00, 01, 10, 11), aur har jod ke liye AND, OR, aur "alag hain?" ka
jawab. Aakhri column khud sochna padega. Jab ban jaaye, aapne aaj
gate design kiya.

## SOCHNE KE LIYE

1. (derivation) NOT gate hata do. Sirf AND aur OR bache. Kya "alag
hain?" wala purza ab bhi ban sakta hai? Kyun ya kyun nahi?

> **Jawab:** Nahi ban sakta. AND aur OR dono "milaane" wale hain: agar
> saare inputs 1 hain, toh dono ka output 1 hi hoga, ulatne wala koi
> nahi. Lekin "alag hain?" ko 11 pe 0 dena hota hai. Bina kisi ulatne
> wale purze ke, 1 se 0 banta hi nahi. Isliye NOT zaroori hai. Sabak:
> chhota sa purza bhi poore system ki taakat badal deta hai, aur design
> ka matlab hi yeh jaan-na hai ki kaunsa purza kya jodta hai.
