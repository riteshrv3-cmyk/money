# THE CLIMB

## 90 दिवस: Top 0.00001 AI Builder चा रस्ता

(Books 1-2 नंतरचा नकाशा. सगळे sources 29 Aug 2026 रोजी
तपासलेले: जिवंत आहेत, ताजे आहेत. मेलेले आणि जुने झालेले
बाहेर काढले आहेत.)

**पहिलं सत्य, पुस्तक उघडण्याआधी:** top 0.00001 हा "सगळं
वाचलेला माणूस" नसतो. तो **रोज बांधणारा माणूस असतो जो नेमकं
वाचतो.** 100 लोकांचं काम एकटा करणारा माणूस जास्त हुशार नसतो:
त्याचा **harness** चांगला असतो. 2026 चं मुख्य सूत्र हेच:

```
Agent = Model + Harness

Model   = भाड्याने मिळतं (सगळ्यांना सारखंच)
Harness = tools + परवानगी + तपासणी + memory + evals
          हे तुम्ही बांधता; हीच तुमची मालकी, हाच फरक
```

Prompt engineering (2023) -> context engineering (2025) ->
**harness engineering (2026).** ~95% agents prototype मध्येच
मरतात; उरलेले 5% production पर्यंत नेणारी गोष्ट harness आहे.
हा 90 दिवसांचा नकाशा तुम्हाला त्या 5% बांधणाऱ्यांत नेतो.

**रोजचे 6+ तास असे वाटा:**

```
30 मिनिटं   बातम्या-system (खाली दिलेली, दिवस 1 पासून)
2 तास       वाचन / course (त्या महिन्याचं)
3.5+ तास    बांधणं (हाच खरा अभ्यास; बाकी सगळं तयारी)
```

---

# 90 दिवसांचा नकाशा: एका नजरेत

```
महिना 1   यंत्र स्वतःच्या हाताने बांधा
          Karpathy + nanochat + fine-tuning
          Project: स्वतः train केलेलं छोटं model, चालू करून

महिना 2   Agents, Harness, Evals (गाभा)
          Anthropic canon + 12-Factor + evals-शिस्त
          Project: खरा agent + त्याची eval-परीक्षा

महिना 3   Production: infra, सुरक्षा, scale, ship
          inference + injection-बचाव + MCP + multi-agent
          Project: एक खरी गोष्ट खऱ्या माणसाच्या हातात
```

तीन महिन्यांत तीन projects. **Project पूर्ण = महिना पूर्ण.**
वाचन संपलं पण project अर्धा, तर महिना अर्धाच झाला.

---

# महिना 1: यंत्र स्वतःच्या हाताने बांधा

Book 2 ने तुम्हाला यंत्र **समजावलं.** आता ते **हाताने बांधायचं.**
हा फरक तोच जो "engine चं चित्र बघणं" आणि "engine खोलून पुन्हा
जोडणं" यात आहे. Top 0.00001 दुसऱ्या गटात असतात.

**आठवडा 1-2: पाया (बघा + करा)**

```
1. Deep Dive into LLMs (Karpathy, video, 3.5 तास)
   youtube.com -> Karpathy channel, Feb 2025 चा video
   पूर्ण training stack एका बैठकीत; Book 2 चा x-ray

2. Neural Networks: Zero to Hero (Karpathy, videos + code)
   karpathy.ai/zero-to-hero.html
   8 videos, ~15 तास बघणं + तितकाच वेळ स्वतः code लिहिणं
   किमान हे तीन: micrograd, "Let's build GPT", Tokenizer
   जगातला सर्वात मानला जाणारा from-scratch course; मोफत

3. The Bitter Lesson (Rich Sutton, निबंध, 15 मिनिटं)
   incompleteideas.net -> Bitter Lesson
   70 वर्षांचा धडा: हाताने कोरलेली हुशारी हरते, scale जिंकतं
   Agent-design च्या प्रत्येक वादात हाच निबंध quote होतो
```

**आठवडा 3-4: स्वतःचं model**

```
4. nanochat (Karpathy, GitHub, 57K+ stars)
   github.com/karpathy/nanochat
   tokenizer -> pretrain -> SFT -> eval -> chat UI: पूर्ण
   साखळी स्वतः चालवा; ~$50 च्या cloud-GPU भाड्यात ChatGPT-2
   दर्जाचं स्वतःचं model. 2026 चा सर्वोत्तम hands-on project

5. Unsloth Fine-tuning + RL Guide (docs, मोफत)
   unsloth.ai/docs -> fine-tuning guide + RL guide
   3GB VRAM वरही चालतं; GRPO/RLVR सकट; मोफत Colab notebooks
   Practitioners खरोखर हेच वापरतात

6. RLHF Book (Nathan Lambert, web-आवृत्ती मोफत)
   rlhfbook.com
   Post-training चं standard पुस्तक: SFT, reward models,
   DPO, GRPO, reward hacking. आत्ता skim; संदर्भाला परत या
```

**महिना 1 चा project:** एक छोटं open model (Unsloth ने) तुमच्या
स्वतःच्या data वर fine-tune करा आणि चालू करून दाखवा. उदाहरण:
Books 1-3 चे प्रश्न-उत्तर deck बनवून त्यावर "तुमच्या पुस्तकांचं
model". Data बनवणं हेच खरं शिक्षण आहे.

---

# महिना 2: Agents, Harness, Evals (गाभा)

हा महिना सगळ्यात महत्त्वाचा. इथेच "AI वापरणारा" आणि "AI
बांधणारा" वेगळे होतात. सगळं वाचन मोफत आहे आणि जग हेच वाचतं.

**आठवडा 5-6: Anthropic canon (agent-बांधणीचं धर्मग्रंथ-कपाट)**

```
7. Building Effective Agents (Dec 2024)
   anthropic.com/engineering/building-effective-agents
   Workflows vs agents, 5 रचना-साचे; अजूनही सगळे हेच quote
   करतात (सुरुवातीची tooling-कलमं जुनी झाली, साचे जिवंत)

8. Effective Context Engineering for AI Agents (Sep 2025)
   anthropic.com/engineering/effective-context-engineering...
   Attention-budget, गरजेपुरतं retrieval, compaction,
   sub-agents. 2026 च्या papers मध्ये सर्वाधिक cited

9. Effective Harnesses for Long-running Agents (Nov 2025)
   anthropic.com/engineering/effective-harnesses...
   अनेक context-windows पार agent सुसंगत ठेवणं; harness
   engineering चा आजचा मुख्य संदर्भ

10. Writing Effective Tools for AI Agents (Sep 2025)
    anthropic.com/engineering/writing-tools-for-agents
    Tool-design: नावं, token-काटकसर, eval-चक्राने सुधारणा

11. Claude Code Best Practices (जिवंत docs)
    code.claude.com/docs -> best practices
    तपासणी-loops, plan mode, CLAUDE.md, subagents, hooks.
    जे रोज वापरता त्याचं आतलं यंत्र

12. Claude Agent SDK (docs + स्वतः चालवा, ~5-10 तास)
    code.claude.com/docs -> agent-sdk
    Claude Code चा agent-loop तुमच्या code मध्ये: हाच
    तुमच्या product चा पाया होणार

13. 12-Factor Agents (GitHub: humanlayer/12-factor-agents)
    Framework-मोहापासून वाचवणारी production-शिस्त: स्वतःचे
    prompts, स्वतःचा control-flow, स्वतःची state

14. OpenAI: Practical Guide to Building Agents (PDF, 34 पानं)
    + openai.github.io/openai-agents-python
    दुसऱ्या घराण्याची नजर; Anthropic-नजरेशी ताडून बघा
```

**आठवडा 7-8: Evals (हीच खरी विद्या)**

2026 चं ब्रीदवाक्य: **"Evals are the new unit tests."**
Agent बांधता येणं सोपं झालंय; तो **खरंच चांगला आहे का** हे
मोजता येणं ही दुर्मिळ विद्या आहे. Top 0.00001 इथे राहतात.

```
15. Hamel Husain चा Evals FAQ (hamel.dev, मोफत)
    "Error analysis हीच सगळ्यात महत्त्वाची कृती": आधी हे;
    त्याचा Maven course ($1-2K) नंतर, पैसे आल्यावर, गरज
    वाटली तरच

16. Demystifying Evals for AI Agents (Anthropic, Jan 2026)
    anthropic.com/engineering/demystifying-evals...
    Agent-evals: code-grading / model-grading / माणूस-grading

17. Eugene Yan: Task-Specific LLM Evals (eugeneyan.com)
    सर्वाधिक link होणारे स्वतंत्र eval-निबंध (लेखक आता
    Anthropic मध्ये)

18. promptfoo (promptfoo.dev, open-source)
    Local eval + red-teaming CLI; स्वतःच्या agent वर चालवा
    (टीप: OpenAI चा Evals platform Nov 2026 ला बंद होतोय;
    त्यावर काही बांधू नका)
```

**महिना 2 चा project:** तुमच्या तीन धंद्यांतल्या एका खऱ्या
दुखण्यावर agent बांधा + त्याची eval-परीक्षा. उदाहरणं:
college-project-तपासणी agent (KodeTalent), तक्रार-वर्गीकरण
agent (नेता-track), जमीन-कागद-तपासणी agent (Book 3 track).
**Golden set 30 प्रश्नांचा आधी बनवा, agent नंतर.** Eval
नसलेला agent म्हणजे speedometer नसलेली गाडी.

---

# महिना 3: Production, सुरक्षा, Scale, SHIP

**आठवडा 9-10: Infra-साक्षरता (बांधणाऱ्यापुरती)**

```
19. Modal GPU Glossary (modal.com/gpu-glossary, 4-6 तास)
    GPU-साक्षरतेचा सर्वात जलद रस्ता: compute-bound vs
    memory-bound, occupancy. Bill समजायला लागतं

20. vLLM docs (docs.vllm.ai, ~10 तास मूलभूत)
    Open model स्वतः serve करायचं झाल्यास जगाचं default
    engine: quantization, speculative decoding

21. How to Scale Your Model (jax-ml.github.io/scaling-book)
    DeepMind च्या लोकांचं scale-पुस्तक; निवडक प्रकरणं.
    खोल पाणी: जमेल तितकं, अडेल तिथे थांबा
```

**आठवडा 11: सुरक्षा (agent-युगाची तलवार-ढाल)**

```
22. Simon Willison: The Lethal Trifecta (simonwillison.net)
    खासगी data + बाहेरचा मजकूर + बाहेर-कृती = तीन एकत्र
    आले की agent फुटतोच; तपासलेल्या 100 production agents
    पैकी ~98% मध्ये तिन्ही हजर, ~11% च मूलभूत परीक्षा पास
23. Prompt injection ची 2026 स्थिती: अजून न सुटलेली.
    उत्तम बचावही adaptive हल्ल्यांपुढे >85% वेळा हरतो.
    म्हणून बचाव = थर: sandbox + कमी-अधिकार + माणूस-मोहोर
    (Book 2, 6.7-6.8 आठवा: तिथेच पाया घातलाय)
```

**आठवडा 11-12: कडा (edge) + SHIP**

```
24. स्वतःचा MCP server लिहा (modelcontextprotocol docs)
    MCP जिंकलंय: OpenAI/Google/Microsoft सगळ्यांनी
    स्वीकारलं, ~97M monthly downloads. "tools चा UPI"
    बांधता येणं = कुठल्याही धंद्याला AI जोडता येणं

25. Subagents / multi-agent (Claude Code docs + अनुभव)
    2026 चा निकाल: 80% गरजा subagents नेच भागतात:
    context-वेगळेपणा + समांतर शोध

26. RL environments ची लाट (वाचून ठेवा, बांधू नका अजून)
    Labs चा पैसा data-labeling कडून खोट्या software-जगांकडे
    (नकली CRM, browser, codebase) सरकला: Mechanize, Prime
    Intellect, Mercor. "Environments हाच नवा data."
    Verifier कच्चा तर model खोटारडं शिकतं (reward hacking)

27. Computer-use agents: Claude पूर्ण desktop चालवतं
    (OSWorld 44%, 2024 च्या 3 पट). GUI-agents production
    मध्ये आले; तुमच्या धंद्यांच्या automation चा पुढचा हात
```

**महिना 3 चा project (सगळ्यात महत्त्वाचा):** महिना 2 चा agent
**एका खऱ्या माणसाच्या हातात द्या** आणि तो वापरताना बघा.
Production चा पहिला दिवस 100 पुस्तकांपेक्षा जास्त शिकवतो.
आणि: **जे बांधलं ते लिहा** (X वर, English मध्ये, thread).
Top 0.00001 सगळे लिहितात; लिहिण्यानेच जाळं आणि नाव बनतं.

---

# 2026 चा शब्दकोश: हे शब्द = तुम्ही आतले

(संभाषणात हे शब्द नीट वापरता आले की तुम्ही "बाहेरचे" नाही.
प्रत्येकाची एक ओळ; खोली वर दिलेल्या sources मध्ये.)

```
harness engineering   गोठलेल्या model भोवतीचं सगळं बांधणं:
                      tools, परवानगी, तपासणी, memory, evals
context engineering   खिडकीत नेमकं काय जाईल याचं शास्त्र;
                      चार शत्रू: poisoning, distraction,
                      confusion, clash
RLVR / verifiers      तपासता-येण्याजोग्या बक्षिसांवर RL
                      (test पास? उत्तर बरोबर?); आजचं मुख्य
                      post-training
reward hacking        कच्च्या verifier ला model फसवतं;
                      तुमचा verifier हीच तुमची स्पेक
test-time compute     मोठं train करण्याऐवजी उत्तरावेळी
                      जास्त विचार; reasoning models यातून
RL environments       शिकवणीसाठी खोटी software-जगं;
                      "environments हाच नवा data"
model spec            model ने कसं वागावं याचा लिखित करार
                      (OpenAI ने प्रघात पाडला)
distillation          मोठ्या model च्या उत्तरांवर छोटं
                      train करणं; स्वस्त-tier ची अर्थव्यवस्था
speculative decoding  छोटं सुचवतं, मोठं तपासतं: 2-4x वेग
MoE                   प्रत्येक token ला यंत्राचा अंशच जागा
                      होतो; frontier चं default architecture
```

```
agentic search        "RAG मेला" वादाचा निकाल: grep+tools+
                      लांब context, agent स्वतः ठरवतो काय
                      आणायचं
memory tools          सत्रापार आठवण tool ने (फक्त retrieval
                      ने नाही); Claude चा memory tool
MCP                   agent-ला-tool जोडणीचा जिंकलेला protocol
A2A                   agent-ला-agent protocol (Google);
                      अजून मागे: बघा, पैज लावू नका
spec-driven dev       आधी नेमकी स्पेक, मग agent बांधतो;
                      "vibe coding" चा production-दर्जा
                      उत्तरार्ध
vibe coding backlash  METR-अभ्यास: AI-सहाय्याने developers
                      19% हळू, स्वतःला 20% जलद वाटत असताना;
                      prototype ला vibe, production ला spec
lethal trifecta       खासगी data + बाहेरचा मजकूर + बाहेर-
                      कृती = फुटणारच (Willison)
LLM-as-judge          model ने model ला गुण देणं; माणसाशी
                      calibrate केलं तरच विश्वास
evals-driven dev      evals CI मध्ये: दर्जा घसरला तर merge
                      थांबतो; "evals are the new unit tests"
agent-native software दोन वाचकांसाठी लिहिलेला repo: माणूस
                      आणि agent (AGENTS.md, ठराविक commands)
post-training shift   प्रगती आता pre-training पेक्षा post-
                      training मधून; open weights म्हणून
                      frontier ला भिडले (DeepSeek, Kimi, Qwen)
```

---

# रोज-ताजं SYSTEM (दिवस 1 पासून, कायमचं)

AI दर महिन्याला बदलतं; पण सगळं वाचणारा बुडतो. हे यंत्र 30
मिनिटांत ~85% आणि आठवड्याच्या 2 तासांत ~95% पकडतं.
**यापेक्षा जास्त वाचणं म्हणजे बांधायचा वेळ खाणं.**

**रोज 30 मिनिटं:**

```
1. AI News (news.smol.ai)          daily digest    10 मिनिटं
   सगळ्या Discord/X/Reddit चा AI-गाळीव अर्क
2. simonwillison.net               जवळजवळ रोज      5 मिनिटं
   प्रत्येक release ची सर्वात जलद हाताळलेली परीक्षा
3. X ची List (खालचे ~15 लोक)       list, feed नको  10 मिनिटं
4. HF Daily Papers (huggingface.co/papers)         5 मिनिटं
   फक्त शीर्षकं; जास्तीत जास्त 1 उघडा
```

**आठवड्याला 2 तास:**

```
1. Interconnects (Lambert) + Import AI (Clark)     40 मिनिटं
2. एक podcast: Dwarkesh किंवा Latent Space (1.5x)  45 मिनिटं
3. Anthropic engineering चा नवा post / नव्या        20 मिनिटं
   model चं system card आलं असेल तर
4. r/LocalLLaMA आठवड्याचं top + (model निवडताना)   15 मिनिटं
   artificialanalysis.ai
```

**X वर हेच ~15 (list बनवा, तपासलेले, active):**

```
@karpathy        शिक्षक-सम्राट (May 2026 पासून Anthropic)
@simonw          practitioner-गाळणी #1
@swyx            AI-engineering चा नकाशा-वाला
@alexalbert__    Claude चे सर्वात आधीचे संकेत
@OfficialLoganK  Gemini बाजू
@amanrsanger     Cursor; agentic-coding रचना
@teortaxesTex    China open-models चा सर्वोत्तम अभ्यास
@_xjdr           inference/sampling ची खोली
@iScienceLuvr    रोजची paper-निवड
@polynoamial     reasoning ची frontier (OpenAI)
@_jasonwei       reasoning research (आता Meta)
@jackclarkSF     धोरण + Import AI
@natolambert     post-training
@steipete        प्रामाणिक agentic-engineering रोजनिशी
@VictorTaelin    वेगळ्या वाटेचं computation
```

**खोल-वाचनाच्या वेळेत (news च्या वेळेत नाही):** Sebastian
Raschka चं Ahead of AI (महिन्याला, architecture खोलात),
SemiAnalysis free tier (compute-अर्थकारण), ChinaTalk
(चीन-labs), 3Blue1Brown + Welch Labs (डोळ्यांनी गणित),
AI Engineer conference चे YouTube talks.

---

# दहा नियम (भिंतीवर)

```
 1. वाचन:बांधणं = 1:2 पेक्षा कमी कधीच नाही
 2. Project पूर्ण = महिना पूर्ण; वाचन पूर्ण = काहीच नाही
 3. Summary वाचू नका, मूळ वाचा (system cards, docs, code)
 4. प्रत्येक agent आधी: 30 प्रश्नांचा golden set
 5. जे बांधाल ते X वर लिहा: English, आठवड्याला एकदा
 6. Framework आधी नको: कच्चा API-loop आधी, साचे मग
 7. नवा शब्द ऐकला की मूळ post शोधा, थ्रेड नको
 8. Model भक्ती नको: तिन्ही घराणी चालवून बघा
    (Claude, GPT, Gemini + एक open: DeepSeek/Qwen)
 9. रोजचं news-बजेट 30 मिनिटं: संपलं की बंद
10. दर 90 दिवसांनी हा नकाशाच पुन्हा तपासा: AI मध्ये
    नकाशेही शिळे होतात (हा 29 Aug 2026 चा आहे)
```

---

# 90 दिवसांनंतर काय?

तेव्हाचे तुम्ही ठरवाल; पण दिशा आत्ताच स्पष्ट आहे: पुढची
पायरी वाचनाची नसून **पुनरावृत्तीची** आहे: बांधा -> ship करा
-> लिहा -> पुन्हा. Top 0.00001 चं शेवटचं गुपित हेच की तिथे
पोहोचल्यावरही रोज हेच चक्र चालू असतं.

आणि Books 1-2 चे दोन होकायंत्र इथेही तेच:
**"हे कुठलं दुखणं सोडवतं?"** आणि **"यावर किती विश्वास, का?"**

सुरू करा. आजच्या 6 तासांतले 3.5 बांधण्याचे आहेत.
