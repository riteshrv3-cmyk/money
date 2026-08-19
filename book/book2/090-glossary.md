# Glossary

Book 2 ke shabd, aur woh chapter jahan aapne unhe kamaya. Book 1 ke shabd uski apni glossary mein hain.

---

**agent** (6.4) — ek model, kuch tools, aur ek dohrav. Iske alaawa kuch nahi. Woh har kadam pe agla sambhavit kadam chunta hai.

**agent loop** (6.4) — karo, nateeja dekho, phir tay karo, dohrao. Context har kadam pe bharta hai aur galtiyan judti jaati hain.

**attention** (3.3) — har shabd har doosre shabd ko dekhta hai, har jodi ka ek wazan nikalta hai, aur nayi jagah sabka mishran hoti hai. Doori se farak nahi padta, ginti ke varg se padta hai.

**batching** (4.1) — kai sawal ek saath chalana, taaki model ki file ek hi baar memory se aaye. Isi se daam gir ta hai, aur isi se vyast waqt mein jawab dheema lagta hai.

**benchmark** (5.3) — tay-shuda test. Teen kamzoriyan: woh training data mein aa jaata hai, uske liye taiyaari ki jaati hai, aur uska aapke kaam se koi rishta nahi hai.

**BPE** (1.6) — tokens banane ka tareeka: baar baar sabse aam jodi ko milaate jao. Isi se tay hota hai ki kaunsi bhasha sasti hai.

**calibrated** (1.3) — jab "70 percent" ka matlab sach mein yeh ho ki aise sau mein se lagbhag 70 baar hota hai. Mausam ke andaaze aksar calibrated hote hain. AI models aksar nahi.

**context window** (4.4) — kitna text ek baar mein diya ja sakta hai. Do seemayein isse banti hain: attention ka kaam varg mein, aur KV cache ki memory.

**cutoff** (2.6) — woh tarikh jiske baad ki duniya model ko pata nahi hai.

**decode** (4.2) — jawab banane ka hissa. Ek-ek token karke, aur har token pe poori file memory se aati hai. Isliye output input se mehnga hai.

**embedding** (3.1) — kisi cheez ke liye numbers ki ek lambi list, jo ek badi khali jagah mein uski jagah batati hai. Doori ka matlab rishta.

**emergence** (3.5) — kuch kaabiliyat chhote models mein nahi hoti aur ek paimane ke baad dikhne lagti hai. Kya woh sach mein chhalang hai, ispe bahas hai.

**hallucination** (5.1) — cheezein bana lena. Teen wajahein: uska kaam hi agla token dena hai, usmein khaali jagah nahi dikhti, aur use aatmvishwas ke liye dhaala gaya. Kam ho sakta hai, khatam nahi.

**inference** (4.1) — model ka istemaal. Training se alag aur bahut sasta. Aur ek chalte product mein kul kharcha training se bada ho jaata hai.

**KV cache** (4.1) — pichhle tokens ka bacha hua kaam. Iske bina lamba jawab varg mein mehnga hota. Iski keemat memory hai.

**layer** (3.3) — attention aur uske baad ka kaam, ek baar. Bade models mein sau se zyada baar dohraya jaata hai.

**learning rate** (2.5) — dhalaan pe kitna bada kadam. Bahut bada toh sab bikhar jaata hai, bahut chhota toh training kabhi khatam nahi hoti.

**loss** (2.4) — ek number jo batata hai ki model kitna galat hai. Poori training ka lakshya use girana hai. Woh sach nahi naapta.

**lost in the middle** (4.4) — bade context mein beech ka hissa aksar dab jaata hai. Context mein hona aur istemaal hona alag baatein hain.

**model** (2.9) — do cheezein: ek sthir file jismein numbers hain, aur use chalane wala code. Jo aap istemaal karte ho woh ek poora dher hai, aur uska bada hissa model ke bahar hai.

**model collapse** (2.7) — jab har agli peedhi pichhli ke likhe pe train hoti hai aur dheere dheere kamzor hoti jaati hai.

**multi-head** (3.3) — attention kai baar, alag alag tarah se, taaki alag kism ke rishte ek saath pakde ja sakein.

**multimodal** (3.6) — ek hi model jo text, photo, awaaz aur video sambhale. Sab tokens mein todi jaati hain, aur unka daam unke token count se aata hai.

**overfitting** (2.4) — model apne data ko ratt leta hai aur naye pe kamzor rehta hai. Isliye thodi galti rehna zaroori hai.

**parameters** (2.3) — weights ki ginti. "70 billion parameters" matlab 70 arab numbers. Ab yeh woh naap nahi raha jo do saal pehle tha.

**prefill** (4.2) — aapka sawal padhne ka hissa. Poora ek saath sambhala jaata hai, aur isi mein "pehla shabd" ka waqt jaata hai.

**prompt injection** (6.7) — bahar ki kisi cheez mein nirdesh chhupa dena, jise model padh kar maan leta hai. Iska koi poora hal abhi nahi hai. Asli bachaav: tools kam, daayra chhota.

**RAG** (6.2) — pehle dhoondho, phir jawab do. Model ko sikhaana nahi, use dikhana. Jab jawab kharaab aaye toh problem aksar dhoondhne mein hoti hai, model mein nahi.

**RLHF** (2.8) — insaan ki pasand se model ko dhaalna. Yahin se "sahayak" wali shakal aati hai, aur yahin se aatmvishwas aur chaploosi bhi.

**scaling laws** (3.5) — hisaab jo batata hai ki kitna kharch karne se loss kitna girega. Kharcha andaza laga sakte ho, kaabiliyat nahi.

**sycophancy** (2.8) — chaploosi. Model aapse zyada sehmat hota hai kyunki insaanon ne aise jawab chune the.

**temperature** (4.3) — chunav mein kitna random. Zero ka matlab "sahi" nahi, "dohraya ja sakne wala" hai.

**token** (1.5) — text ka ek tukda, model ke liye ek number. Akshar se bada, shabd se chhota. Model ko akshar dikhte hi nahi.

**tool call** (6.3) — model ka woh likha hua jo ek tool maangta hai. Model kuch karta nahi, woh maangta hai, aur ek program karta hai.

**training** (2.2) — agla token chhupao, guess karwao, galti naapo, numbers hilao, kharabon baar. Jawab data mein pehle se hota hai, isi chaalaki ne paimana mumkin banaya.

**transformer** (3.4) — poora design: tokens, jagah, kram, sau layers, aur aakhir mein sambhavna. 2017 se lagbhag wahi hai.

**vector database** (6.2) — woh database jo embedding se "paas wali" cheez dhoondhta hai. Book 1 ke index ka hi ek roop.

**weights** (2.3) — model ke andar ke numbers. Ek nichod, ek copy nahi. Ek weight ka koi matlab nahi hota.
