## विषयसूची

1. [SDLC परिचय](#१-sdlc-परिचय)
2. [SDLC का चरणहरू](#२-sdlc-का-चरणहरू)
3. [SDLC को सामान्य प्रक्रिया](#३-sdlc-को-सामान्य-प्रक्रिया)
4. [SDLC Models र Methodologies](#४-sdlc-models-र-methodologies)
5. [Model/Approach तुलना र छनोट](#५-modelapproach-तुलना-र-छनोट)
6. [QA विकासपछि मात्र किन सुरु गर्नु हुँदैन?](#६-qa-विकासपछि-मात्र-किन-सुरु-गर्नु-हुँदैन)
7. [QA, QC र Testing बीचको फरक](#७-qa-qc-र-testing-बीचको-फरक)
8. [Shift-Left, Continuous र Shift-Right Testing](#८-shift-left-continuous-र-shift-right-testing)
9. [Requirement र Acceptance Criteria को उदाहरण](#९-requirement-र-acceptance-criteria-को-उदाहरण)
10. [Test Levels र Test Types](#१०-test-levels-र-test-types)
11. [MERN Project मा SDLC र QA](#११-mern-project-मा-sdlc-र-qa)
12. [Quality Gates र Definition of Done](#१२-quality-gates-र-definition-of-done)
13. [सामान्य गल्ती र राम्रो अभ्यास](#१३-सामान्य-गल्ती-र-राम्रो-अभ्यास)
14. [शब्दावली](#१४-शब्दावली)
15. [अभ्यास प्रश्न र उत्तर](#१५-अभ्यास-प्रश्न-र-उत्तर)
16. [छोटो पुनरावलोकन](#१६-छोटो-पुनरावलोकन)
17. [थप अध्ययनका स्रोत](#१७-थप-अध्ययनका-स्रोत)

---

## १. SDLC परिचय

### १.१ SDLC भनेको के हो?

**Software Development Life Cycle (SDLC)** भनेको सफ्टवेयरलाई योजना बनाउने, आवश्यकताहरू बुझ्ने, डिजाइन गर्ने, विकास गर्ने, परीक्षण गर्ने, प्रयोगमा ल्याउने र निरन्तर सुधार गर्ने व्यवस्थित प्रक्रिया हो। यसको उद्देश्य प्रयोगकर्ताको आवश्यकता पूरा गर्ने, सुरक्षित, भरपर्दो, गुणस्तरीय र मर्मत गर्न सजिलो सफ्टवेयर निर्माण गर्नु हो।

SDLC ले परियोजनामा के-कस्ता काम गर्नुपर्छ, ती काम कसरी व्यवस्थापन गर्ने, जिम्मेवारी कसको हुन्छ र काम पूरा भएको कसरी जाँच्ने भन्ने विषय व्यवस्थित गर्न मद्दत गर्छ।

> **महत्त्वपूर्ण:** SDLC का चरणहरूको संख्या र नाम पुस्तक, संस्था वा प्रयोग गरिएको प्रक्रियाअनुसार फरक हुन सक्छ। यस नोटमा अध्ययनका लागि Planning सहितको सामान्य प्रक्रिया र पछि प्रचलित ६ चरणको वर्गीकरण दुवैको व्याख्या गरिएको छ।

### १.२ SDLC किन आवश्यक छ?

- प्रयोगकर्ता र संस्थाको आवश्यकता स्पष्ट बनाउन।
- परियोजनाको Scope, समय, बजेट र जिम्मेवारी व्यवस्थित गर्न।
- गलत बुझाइ र अनावश्यक पुनःकाम (Rework) घटाउन।
- सुरक्षा, गुणस्तर र प्रयोगयोग्यता सुरुदेखि विचार गर्न।
- Development, Testing र Deployment को काम व्यवस्थित गर्न।
- जोखिम र त्रुटि चाँडै पहिचान गर्न।
- सफ्टवेयरको maintenance तथा आगामी सुधार सजिलो बनाउन।

### १.३ मुख्य अवधारणाबीचको भिन्नता

- **SDLC Phases:** परियोजनामा कुन-कुन प्रकारका काम हुन्छन् भन्ने देखाउँछन्।
- **SDLC Models/Approaches:** ती काम कुन क्रममा वा कुन तरिकाले व्यवस्थित गरिन्छन् भन्ने बताउँछन्।
- **QA (Quality Assurance):** गुणस्तर कायम राख्न आवश्यक प्रक्रिया र अभ्यासमा ध्यान दिन्छ।
- **QC (Quality Control):** उत्पादन वा deliverable को गुणस्तर जाँच्ने गतिविधि हो।
- **Software Testing:** सफ्टवेयरको व्यवहार जाँचेर त्रुटि पत्ता लगाउने र आवश्यकतासँग मेल खान्छ कि खाँदैन भन्ने प्रमाण जुटाउने गतिविधि हो।

### १.४ SDLC को सामान्य चरण

अध्ययनका लागि एउटा सामान्य वर्गीकरण:

1. Requirement Analysis — आवश्यकता विश्लेषण
2. Design — डिजाइन
3. Development — विकास
4. Testing — परीक्षण
5. Deployment — प्रयोगमा ल्याउने
6. Maintenance — मर्मत तथा सुधार

कतिपय प्रक्रियामा **Planning** छुट्टै चरण हुन्छ। Planning लाई Requirement Analysis सँगै वा परियोजनाभरि चल्ने गतिविधिका रूपमा पनि व्यवस्थित गर्न सकिन्छ।

---

## २. SDLC का चरणहरू

### २.१ Planning — योजना निर्माण

परियोजना किन बनाउने, के परिणाम चाहिन्छ, कति समय/बजेट लाग्छ र सम्भावित जोखिम के हुन् भन्ने प्रारम्भिक योजना बनाइन्छ।

**मुख्य काम:**
- समस्या र परियोजनाको उद्देश्य परिभाषित गर्ने।
- प्रारम्भिक Scope र अपेक्षित परिणाम तय गर्ने।
- बजेट, समय, टोली र आवश्यक स्रोत अनुमान गर्ने।
- प्राविधिक सम्भाव्यता (Feasibility) जाँच्ने।
- प्रमुख जोखिम र निर्भरता पहिचान गर्ने।
- प्रारम्भिक Project Plan र जिम्मेवारी तय गर्ने।

**उदाहरण:** नगरपालिकाले नागरिकलाई अनलाइन सिफारिस आवेदन दिन सक्ने पोर्टल बनाउने निर्णय गर्छ। सुरुमा बजेट, आवश्यक सेवा, प्रयोगकर्ता समूह, डेटा सुरक्षा र सञ्चालन जिम्मेवारीको मूल्याङ्कन गरिन्छ।

**Deliverables:** Project Charter/Brief, feasibility notes, प्रारम्भिक schedule, risk list, scope statement।

**QA को भूमिका:** उद्देश्य मापन गर्न सकिने छ कि छैन, गुणस्तरसम्बन्धी अपेक्षा छन् कि छैनन् र प्रमुख जोखिम छुटेका छन् कि छैनन् समीक्षा गर्ने।

### २.२ Requirement Analysis — आवश्यकता विश्लेषण

प्रयोगकर्ता र संस्थालाई के चाहिन्छ भन्ने पत्ता लगाई आवश्यकताहरू स्पष्ट, पूर्ण, प्राथमिकताबद्ध र परीक्षण गर्न मिल्ने रूपमा लेखिन्छ।

**मुख्य काम:**
- Stakeholders र प्रयोगकर्ताको आवश्यकता सङ्कलन गर्ने।
- Functional र Non-functional requirements छुट्याउने।
- Scope, सीमा र प्राथमिकता तय गर्ने।
- Acceptance Criteria बनाउने।
- अपवाद अवस्था र सम्भावित जोखिम पहिचान गर्ने।
- अस्पष्ट, अपूर्ण वा एकअर्कासँग विरोधाभास भएका requirement समीक्षा गर्ने।

**Functional Requirement** ले प्रणालीले *के गर्नुपर्छ* बताउँछ।  
उदाहरण: नागरिकले अनलाइन सिफारिसका लागि आवेदन दिन सक्नुपर्छ।

**Non-functional Requirement** ले प्रणालीको गुणस्तर वा सञ्चालनसम्बन्धी अपेक्षा बताउँछ।  
उदाहरण: मोबाइलमा प्रयोग गर्न सजिलो हुनुपर्छ; अनधिकृत प्रयोगकर्ताले संवेदनशील विवरण हेर्न नपाउनुपर्छ; निर्धारित load मा प्रतिक्रिया समय स्वीकार्य हुनुपर्छ।

**नगरपालिका पोर्टलको उदाहरण:**
- नागरिकले खाता खोल्न र लगइन गर्न सक्ने।
- नागरिकले सिफारिस आवेदन भर्न र आवश्यक कागजात upload गर्न सक्ने।
- नागरिकले आवेदनको अवस्था हेर्न सक्ने।
- वडा कर्मचारीले आफूलाई अधिकार दिइएका अभिलेख मात्र हेर्न सक्ने।

**QA को भूमिका:** Requirement review, अस्पष्टता पहिचान, testability जाँच, acceptance criteria समीक्षा र प्रारम्भिक जोखिम विश्लेषण।

**Deliverables:** Requirement Specification, user stories, acceptance criteria, prioritized backlog, requirement traceability को प्रारम्भिक सूची।

### २.३ Design — डिजाइन

आवश्यकता पूरा गर्न प्रणालीको संरचना, प्रयोगकर्ता इन्टरफेस, डेटा र module हरू कसरी बनाउने भन्ने योजना तयार गरिन्छ।

**मुख्य काम:**
- UI/UX wireframe र prototype बनाउने।
- System architecture र module boundaries तय गर्ने।
- Database schema र data relationships डिजाइन गर्ने।
- API contract, request/response र status codes परिभाषित गर्ने।
- Authentication र authorization को व्यवस्था डिजाइन गर्ने।
- Error handling, privacy र security controls योजना बनाउने।
- Responsive layout, accessibility र performance आवश्यकता समेट्ने।

**उदाहरण:** React frontend, Node.js/Express backend र MongoDB database बीचको संरचना बनाउने। नागरिक, वडा कर्मचारी र प्रशासकका अधिकार छुट्याउने।

**QA को भूमिका:**
- UI/UX र accessibility review गर्ने।
- API contract र data flow जाँच्ने।
- Threat modeling र access-control design समीक्षा गर्ने।
- Requirement अनुसार test plan तथा test scenarios तयार गर्न सुरु गर्ने।

**Deliverables:** Architecture diagram, UI/UX prototype, database model, API specification, permission matrix, design notes।

### २.४ Development — विकास

स्वीकृत आवश्यकता र डिजाइनअनुसार code लेखेर सफ्टवेयरका सुविधा निर्माण गरिन्छ।

**मुख्य काम:**
- Frontend, backend र database logic विकास गर्ने।
- Input validation र error handling लागू गर्ने।
- Git जस्ता Version Control System प्रयोग गर्ने।
- Code review, linting र static analysis गर्ने।
- Unit/component tests लेख्ने र चलाउने।
- Secrets, password र API key source code मा नराख्ने।
- आवश्यकता अनुसार documentation अद्यावधिक गर्ने।

**उदाहरण:** नागरिक लगइन, सिफारिस फाराम, आवेदन सूची र प्रशासनिक dashboard निर्माण गर्ने।

**QA को भूमिका:**
- Code review र testability मा सहयोग गर्ने।
- Test data तयार गर्ने।
- Unit, component र API tests चलाउन सहयोग गर्ने।
- Defect लेख्ने र developer सँग छिटो feedback आदानप्रदान गर्ने।
- केवल frontend मा नभई backend मा पनि validation र authorization लागू भएको जाँच्ने।

**Deliverables:** Source code, automated tests, code review records, updated technical documentation।

### २.५ Testing — परीक्षण

सफ्टवेयरले आवश्यकता पूरा गर्छ कि गर्दैन, अपेक्षित व्यवहार देखाउँछ कि देखाउँदैन र प्रमुख जोखिम नियन्त्रणमा छन् कि छैनन् जाँचिन्छ।

**मुख्य काम:**
- Unit, Component, Integration, System र Acceptance testing आवश्यकताअनुसार गर्ने।
- API, UI, database flow र user permissions जाँच्ने।
- Positive, negative, boundary र failure scenarios परीक्षण गर्ने।
- आवश्यकताअनुसार regression, security, performance, accessibility र responsive checks गर्ने।
- Defect रिपोर्ट गर्ने, fix verify गर्ने र सम्बन्धित परीक्षण पुनः चलाउने।

**उदाहरण:**
- मोबाइलमा आवेदन फाराम ठीकसँग चल्छ कि चल्दैन।
- आवेदन database मा सुरक्षित हुन्छ कि हुँदैन।
- वडा कर्मचारीले अनुमति नभएको वडाको अभिलेख हेर्न सक्छ कि सक्दैन।
- API असफल हुँदा प्रयोगकर्तालाई उपयुक्त error देखिन्छ कि देखिँदैन।

**QA को भूमिका:** जोखिमअनुसार test coverage सुनिश्चित गर्ने, defect triage मा सहयोग गर्ने, परीक्षण प्रमाण सङ्कलन गर्ने र release का लागि बाँकी जोखिम स्पष्ट पार्ने।

> Testing एउटा महत्त्वपूर्ण चरण हो, तर QA यस चरणमा मात्र सीमित हुँदैन। Requirement र Design review देखि Maintenance सम्म पनि गुणस्तरसम्बन्धी गतिविधि चल्छ।

**Deliverables:** Test plan, test cases, execution results, defect reports, test summary/report।

### २.६ Deployment — प्रयोगमा ल्याउने

परीक्षण र स्वीकृतिपछि सफ्टवेयरलाई वास्तविक प्रयोग हुने वातावरण (Production) मा प्रकाशित गरिन्छ।

**मुख्य काम:**
- Production configuration र environment variables मिलाउने।
- Domain, HTTPS/TLS, secrets र database access सुरक्षित गर्ने।
- Build, deployment र rollback प्रक्रिया तयार गर्ने।
- आवश्यक database migration र backup/restore योजना जाँच्ने।
- CI/CD pipeline, health checks, logs र monitoring तयार गर्ने।
- Release पछि smoke test चलाउने।

**उदाहरण:** React frontend लाई Cloudflare Pages मा र Node.js backend लाई Render जस्तो hosting मा deploy गर्ने; MongoDB Atlas access rules र production environment variables सुरक्षित रूपमा मिलाउने।

**QA को भूमिका:** Staging verification, deployment checklist, migration validation, smoke tests र rollback readiness जाँच्ने।

**Deliverables:** Release notes, deployment record, smoke-test result, rollback plan, production monitoring setup।

### २.७ Maintenance — मर्मत तथा सुधार

Release पछि प्रणालीको समस्या समाधान, सुरक्षा अपडेट, monitoring र प्रयोगकर्ताको feedback का आधारमा सुधार गरिन्छ।

**मुख्य काम:**
- Bug fixing र regression testing।
- Dependency तथा security updates।
- Performance र usability सुधार।
- Backup बनेको मात्र होइन, restore गर्न सकिन्छ कि सकिँदैन परीक्षण गर्ने।
- Logs, metrics, alerts र incident response व्यवस्थापन गर्ने।
- नयाँ आवश्यकता आएमा अर्को development cycle सुरु गर्ने।

**उदाहरण:** प्रयोगकर्ताको प्रतिक्रियाअनुसार नयाँ सिफारिस थप्ने, त्रुटि सच्याउने र database backup बाट restore परीक्षण गर्ने।

**QA को भूमिका:** Fix verification, regression testing, production feedback विश्लेषण र आगामी release को गुणस्तर सुनिश्चित गर्ने।

**Deliverables:** Patch/release notes, defect fixes, monitoring reports, updated backlog, post-incident review जहाँ आवश्यक हुन्छ।

---

## ३. SDLC को सामान्य प्रक्रिया

```text
Planning
   ↓
Requirement Analysis
   ↓
Design
   ↓
Development
   ↓
Testing
   ↓
Deployment
   ↓
Maintenance
   ↺
Feedback / New Requirements
```

यो एउटा सामान्य चित्र हो। वास्तविक परियोजनामा सबै चरण सधैँ एकपटक मात्र र कडाइका साथ क्रमिक रूपमा हुँदैनन्। Agile जस्ता दृष्टिकोणमा Requirement, Design, Development र Testing प्रत्येक iteration मा दोहोरिन सक्छन्। QA ले यी सबै चरणमा सहयोग गर्छ।

### ३.१ Entry Criteria र Exit Criteria

- **Entry Criteria:** कुनै चरण सुरु गर्नुअघि पूरा हुनुपर्ने न्यूनतम सर्त।
- **Exit Criteria:** अर्को चरणमा जान वा काम पूरा मान्न पूरा हुनुपर्ने सर्त।

उदाहरण:
- Development सुरु गर्न स्वीकृत requirement र पर्याप्त design जानकारी आवश्यक हुन सक्छ।
- Testing सुरु गर्न testable build, test environment र test data आवश्यक हुन सक्छ।
- Release अघि आवश्यक critical tests पास भएको, गम्भीर defect को अवस्था समीक्षा भएको र rollback plan तयार भएको हुन सक्छ।

यी सर्तहरू परियोजनाको जोखिम र प्रक्रियाअनुसार तय गरिन्छन्।

---

## ४. SDLC Models र Methodologies

> **शब्द प्रयोगबारे:** Waterfall, V-Model र Spiral लाई प्रायः SDLC models भनिन्छ। Agile एउटा व्यापक approach हो; Scrum Agile सँग सम्बन्धित framework हो। RAD विकास दृष्टिकोण हो भने DevOps विकास र सञ्चालनलाई जोड्ने संस्कृति, अभ्यास र toolchain को संयोजन हो। यी सबै एउटै प्रकारका वस्तु होइनन्, तर अध्ययनका लागि तुलना गर्न सकिन्छ।

### ४.१ Waterfall Model — क्रमिक मोडेल

एउटा चरणको काम पूरा गरी समीक्षा गरेपछि अर्को चरणमा जाने परम्परागत दृष्टिकोण हो।

**सामान्य क्रम:** Requirements → Design → Implementation → Verification/Testing → Deployment → Maintenance

**उपयुक्त अवस्था:**
- आवश्यकता स्पष्ट र तुलनात्मक रूपमा स्थिर छ।
- चरणगत documentation र औपचारिक approval महत्त्वपूर्ण छन्।

**फाइदा:**
- योजना, चरण र deliverables बुझ्न सजिलो।
- जिम्मेवारी र कागजात स्पष्ट राख्न सकिन्छ।

**कमजोरी:**
- Feedback ढिलो आउन सक्छ।
- पछिल्लो चरणमा आवश्यकता परिवर्तन भए rework बढ्न सक्छ।

**QA सम्बन्धी कुरा:** Waterfall मा पनि requirement review र test planning सुरुदेखि गर्न सकिन्छ। Formal system testing प्रायः development पछө केन्द्रित भए पनि QA को सम्पूर्ण काम पछिल्लो चरणमा मात्र सीमित हुनु हुँदैन।

### ४.२ Agile — पुनरावृत्तिमूलक र लचिलो दृष्टिकोण

सफ्टवेयरलाई साना उपयोगी increments मा विकास गर्दै नियमित feedback र सुधार गर्ने दृष्टिकोण हो।

**मुख्य विशेषता:**
- कामलाई साना प्राथमिकताबद्ध भागमा विभाजन गर्ने।
- छोटो development cycle मा काम गर्ने।
- Stakeholder बाट नियमित feedback लिने।
- आवश्यकता अनुसार योजना अद्यावधिक गर्ने।
- प्रत्येक increment मा testing र quality practices समावेश गर्ने।

**फाइदा:** छिटो feedback, परिवर्तनसँग अनुकूलता र क्रमशः मूल्य प्रदान।

**चुनौती:** प्राथमिकता, documentation, architecture र stakeholder सहभागिता व्यवस्थित गर्नुपर्छ। Agile भनेको योजना वा documentation नगर्ने भन्ने होइन।

### ४.३ Scrum Framework

Scrum, Agile सिद्धान्तसँग मेल खाने काम व्यवस्थित गर्ने framework हो। कामलाई निश्चित अवधिका **Sprint** मा व्यवस्थित गरिन्छ। Sprint एक महिनासम्मको हुन सक्छ; धेरै टोलीले १–२ हप्ताका Sprint पनि प्रयोग गर्छन्।

**मुख्य Accountabilities:**
- **Product Owner:** Product Goal र Product Backlog को मूल्य तथा प्राथमिकता व्यवस्थापन गर्ने।
- **Scrum Master:** Scrum बुझ्न र प्रभावकारी रूपमा लागू गर्न सहयोग गर्ने।
- **Developers:** Sprint मा उपयोगी Increment निर्माण गर्ने; testing र quality सहित काम पूरा गर्ने।

**मुख्य Events:** Sprint, Sprint Planning, Daily Scrum, Sprint Review र Sprint Retrospective।

**मुख्य Artifacts:** Product Backlog, Sprint Backlog र Increment।

**महत्त्वपूर्ण:** Scrum र Agile पर्यायवाची होइनन्। Scrum Agile सँग सम्बन्धित एउटा framework हो। Scrum मा testing Sprint को अन्त्यमा मात्रै गर्ने होइन; कामको क्रममा नै गुणस्तर कायम राखिन्छ।

### ४.४ V-Model — Verification and Validation Model

V-Model मा विकास/verification का चरण र तिनसँग सम्बन्धित testing/validation स्तरबीच स्पष्ट सम्बन्ध राखिन्छ। बायाँपट्टि आवश्यकता र डिजाइनबाट implementation तर्फ जान्छ; दायाँपट्टि सम्बन्धित testing स्तरहरू हुन्छन्।

| विकास/Verification पक्ष | सम्बन्धित Testing/Validation पक्ष |
|---|---|
| Business/User Requirements | Acceptance Testing |
| System Requirements | System Testing |
| High-level/System Architecture Design | Integration Testing |
| Detailed/Module Design | Unit Testing |
| Implementation/Coding | Code निर्माण |

यो एउटा सामान्य mapping हो; परियोजना, संगठन र testing strategy अनुसार mapping फरक हुन सक्छ।

**फाइदा:**
- Test planning सुरुदेखि हुन्छ।
- Requirement र test बीच traceability बलियो बनाउन मद्दत गर्छ।

**कमजोरी:**
- परिवर्तनशील आवश्यकता भएका परियोजनामा औपचारिक प्रक्रिया भारी हुन सक्छ।

**उपयुक्त अवस्था:** स्पष्ट specification, traceability वा औपचारिक verification आवश्यक भएका परियोजना।

### ४.५ Spiral Model — जोखिममा आधारित चक्रिय मोडेल

सफ्टवेयर धेरै चक्रमा विकास गरिन्छ। प्रत्येक चक्रमा योजना, जोखिम विश्लेषण, विकास/प्रमाणीकरण र मूल्याङ्कन गरिन्छ।

**सामान्य चक्र:**
1. उद्देश्य, विकल्प र सीमाहरू निर्धारण।
2. जोखिम पहिचान र विश्लेषण; आवश्यक परे prototype।
3. विकास र परीक्षण।
4. Stakeholder समीक्षा तथा अर्को चक्रको योजना।

**फाइदा:** जोखिमलाई चाँडै पहिचान र व्यवस्थापन गर्न मद्दत।

**कमजोरी:** जोखिम विश्लेषणमा विशेषज्ञता, समय र खर्च बढी लाग्न सक्छ।

**उपयुक्त अवस्था:** ठूला, जटिल वा उच्च जोखिम भएका परियोजना।

### ४.६ Prototyping — नमुना निर्माण

अन्तिम प्रणाली बनाउनु अघि नमुना (Prototype) तयार गरी प्रयोगकर्ताबाट feedback लिइन्छ।

**उपयुक्त अवस्था:** प्रयोगकर्ताको आवश्यकता वा UI/UX पूर्ण रूपमा स्पष्ट नभएको अवस्था।

**फाइदा:** गलत बुझाइ चाँडै पत्ता लाग्छ र प्रयोगकर्ताले अपेक्षित व्यवहार हेरेर प्रतिक्रिया दिन सक्छन्।

**जोखिम:** Prototype लाई production-ready प्रणाली ठान्नु हुँदैन। वास्तविक security, accessibility, data validation र architecture छुट्टै डिजाइन तथा परीक्षण गर्नुपर्छ।

### ४.७ RAD (Rapid Application Development)

Prototype, reusable components र प्रयोगकर्ताको निरन्तर सहभागिताबाट सीमित दायराका application छिटो निर्माण गर्ने दृष्टिकोण हो।

**फाइदा:** छिटो feedback र छोटो विकास चक्र।

**सीमा:** जटिल integration, उच्च performance/security आवश्यकता वा धेरै dependency भएका प्रणालीमा थप योजना र सावधानी चाहिन्छ।

### ४.८ DevOps — Development र Operations बीच सहकार्य

DevOps ले विकास, testing, deployment र सञ्चालनलाई जोड्दै automation, साझा जिम्मेवारी, CI/CD, monitoring र निरन्तर feedback मा जोड दिन्छ।

**मुख्य अभ्यास:**
- Automated build तथा test।
- CI/CD pipeline र repeatable deployment।
- Infrastructure/configuration as code जहाँ उपयुक्त हुन्छ।
- Logs, metrics, alerts र incident response।
- Backup/restore तथा rollback अभ्यास।
- Security checks लाई pipeline मा समावेश गर्ने; यससँग सम्बन्धित अभ्यासलाई DevSecOps पनि भनिन्छ।

**महत्त्वपूर्ण:** DevOps कुनै एउटा tool वा deployment method मात्र होइन। यसले QA हटाउँदैन; automated र निरन्तर quality checks लाई थप प्रभावकारी बनाउन सक्छ।

---

## ५. Model/Approach तुलना र छनोट

| Model/Approach | मुख्य विशेषता | QA/Testing को स्वरूप | उपयुक्त अवस्था |
|---|---|---|---|
| Waterfall | क्रमिक चरण | चरणगत review; formal system testing प्रायः पछि | स्थिर आवश्यकता |
| Agile | छोटा iteration र feedback | प्रत्येक iteration मा निरन्तर | बदलिँदो आवश्यकता |
| Scrum | Sprint मार्फत काम व्यवस्थापन | Sprint भित्र testing र Definition of Done | Product development टोली |
| V-Model | विकास चरणसँग testing mapping | प्रारम्भिक test planning र traceability | औपचारिक verification |
| Spiral | जोखिम विश्लेषणसहित चक्र | प्रत्येक चक्रमा risk-based verification | ठूला/उच्च जोखिमका system |
| Prototyping | नमुना र feedback | prototype बाट requirement/usability जाँच; production testing छुट्टै | अस्पष्ट आवश्यकता |
| RAD | छिटो निर्माण र reusable components | बारम्बार validation/testing | सीमित दायराको छिटो विकास |
| DevOps | automation, delivery र operations सहकार्य | CI/CD, automated tests, monitoring | नियमित release/सञ्चालन |

### कुन सबैभन्दा राम्रो?

सबै परियोजनाका लागि एउटै उत्तम model हुँदैन। छनोट गर्दा विचार गर्नुहोस्:
- आवश्यकता कति स्थिर वा परिवर्तनशील छ?
- जोखिम र सुरक्षा आवश्यकता कति उच्च छन्?
- बजेट, समय र टोलीको सीप कस्तो छ?
- प्रयोगकर्ताको feedback कति छिटो उपलब्ध हुन्छ?
- नियमन, audit वा औपचारिक documentation आवश्यक छ कि छैन?
- Release कति पटक गर्नुपर्छ?

**MERN नगरपालिका पोर्टलका लागि उदाहरणीय संयोजन:** Agile/Scrum बाट काम व्यवस्थित गर्ने, V-Model-जस्तो requirement-to-test traceability अपनाउने, र DevOps/CI/CD बाट repeatable testing/deployment गर्ने। यो अनिवार्य recipe होइन; परियोजनाको सन्दर्भअनुसार मिलाउनुपर्छ।

---

## ६. QA विकासपछि मात्र किन सुरु गर्नु हुँदैन?

QA (Quality Assurance) विकास सकिएपछि मात्र सुरु हुने अन्तिम काम होइन। यो Requirement चरणदेखि सुरु भएर Design, Development, Testing, Deployment र Maintenance सम्म चल्ने गुणस्तरसम्बन्धी गतिविधिहरूको समष्टि हो।

### ६.१ प्रत्येक चरणमा QA

**Requirement चरण**
- आवश्यकता स्पष्ट, पूर्ण, सम्भव र परीक्षण गर्न मिल्ने छ कि छैन?
- अपवाद अवस्था र user roles उल्लेख छन् कि छैनन्?
- Acceptance Criteria परिभाषित छन् कि छैनन्?

उदाहरण: कुन कर्मचारीले सिफारिस स्वीकृत गर्न सक्छ? अर्को वडाको कर्मचारीले आवेदन हेर्न पाउँछ कि पाउँदैन? नियम अस्पष्ट भए गलत प्रणाली बन्न सक्छ।

**Design चरण**
- UI/UX, API, database र architecture आवश्यकता अनुरूप छन्?
- Authorization र privacy सुरुदेखि डिजाइन गरिएको छ?
- Accessibility, responsive layout र error states विचार गरिएको छ?

उदाहरण: वडा कर्मचारीलाई आफ्नो अधिकारभित्रका record मात्र हेर्न दिने authorization rule डिजाइन गर्ने।

**Development चरण**
- Code review, linting र automated tests चलाइएका छन्?
- Frontend validation मात्र होइन, backend validation पनि छ?
- Error handling, logging र secure coding practices अपनाइएका छन्?

उदाहरण: React form मा required field जाँच्ने र Express API मा पनि server-side validation लागू गर्ने।

**Integration/System Testing चरण**
- Frontend, API, database, authentication र authorization एकसाथ सही चल्छन्?
- सामान्य flow मात्र होइन, failure/edge cases पनि जाँचिएका छन्?
- विभिन्न role र device मा व्यवहार सही छ?

उदाहरण: आवेदन बुझाएपछि MongoDB मा सुरक्षित हुने, सही dashboard मा देखिने र गलत role ले त्यसलाई स्वीकृत गर्न नसक्ने कुरा जाँच्ने।

**Deployment/Production चरण**
- Environment variables, domain/TLS, database permissions र migrations सही छन्?
- Smoke test, rollback र monitoring तयार छन्?
- Production मा प्रकाशित build अपेक्षित रूपमा चल्छ?

**Maintenance चरण**
- Bug fix पछि regression tests चलाइन्छ?
- Dependency/security updates समीक्षा गरिन्छ?
- Backup restore परीक्षण र monitoring alerts जाँचिन्छ?

### ६.२ ढिलो त्रुटि पत्ता लगाउँदा लागत किन बढ्न सक्छ?

Requirement चरणमै गलत बुझाइ पत्ता लागेमा document वा acceptance criteria सच्याउनु पर्याप्त हुन सक्छ। Production पछि पत्ता लागेमा code, database migration, data correction, frontend, backend, regression testing, release र incident handling समेत आवश्यक हुन सक्छ।

कहिलेकाहीँ शिक्षण सामग्रीमा Requirement = 1×, Design = 3×, Development = 5×, System Testing = 10× र Production = 30× जस्ता उदाहरण देखाइन्छन्। **यी निश्चित वा सार्वभौमिक वैज्ञानिक अनुपात होइनन्।** वास्तविक लागत त्रुटिको प्रकृति, प्रभाव, architecture र परियोजनाअनुसार फरक हुन्छ। मुख्य कुरा: प्रारम्भिक review ले धेरै defect सस्तो अवस्थामा समात्न मद्दत गर्छ।

### ६.३ QA सुरुदेखि गर्दा हुने फाइदा

- गलत requirement अनुसार code बनाउने जोखिम घट्छ।
- Security र access-control कमजोरी चाँडै देखिन्छ।
- Rework, ढिलाइ र अनावश्यक खर्च घटाउन मद्दत हुन्छ।
- Test cases र acceptance criteria स्पष्ट हुन्छन्।
- Developer र tester बीच feedback चक्र छोटो हुन्छ।
- Release निर्णय परीक्षण प्रमाणमा आधारित हुन सक्छ।

**निष्कर्ष:** Development पछि system testing अझै आवश्यक छ; तर त्यो सम्पूर्ण QA होइन। QA ले सुरुदेखि नै गुणस्तर निर्माण गर्ने काम गर्छ।

---

## ७. QA, QC र Testing बीचको फरक

| पक्ष | QA (Quality Assurance) | QC (Quality Control) | Testing |
|---|---|---|---|
| मुख्य उद्देश्य | गुणस्तर कायम राख्ने प्रक्रिया सुधार्ने र defect रोक्न मद्दत गर्ने | deliverable/उत्पादनको गुणस्तर जाँच्ने | व्यवहार जाँचेर defect पत्ता लगाउने र आवश्यकता पूरा भएको प्रमाण जुटाउने |
| केन्द्रबिन्दु | प्रक्रिया, मापदण्ड, review र prevention | उत्पादन र deliverables | code, UI, API र प्रणालीको व्यवहार |
| कहिलेदेखि? | योजना/Requirement चरणदेखि | जाँच्न मिल्ने output उपलब्ध भएपछि विभिन्न चरणमा | परीक्षण गर्न मिल्ने artifact उपलब्ध भएपछि; विकासक्रम र release अघि/पछि |
| उदाहरण | requirement review, process audit, Definition of Done | deliverable inspection, test result review | API test, UI test, regression test |
| कसले गर्छ? | सम्पूर्ण टोलीको योगदान; QA specialist ले नेतृत्व गर्न सक्छ | QA/QC specialist, developer वा सम्बन्धित टोली | developer, tester, automation engineer र अन्य सदस्य |

Практиकमा QA र QC शब्दहरू संस्थाअनुसार केही फरक अर्थमा प्रयोग हुन सक्छन्। सिकाइका लागि QA लाई प्रक्रिया/defect prevention, QC लाई deliverable quality control र Testing लाई उत्पादनको व्यवहार जाँच्ने गतिविधिका रूपमा छुट्याएर बुझ्नु उपयोगी हुन्छ। **Testing भनेको केवल bug खोज्नु होइन; आवश्यकता पूरा भएको प्रमाण सङ्कलन गर्नु पनि हो।**

---

## ८. Shift-Left, Continuous र Shift-Right Testing

### ८.१ Shift-Left Testing

गुणस्तर जाँचलाई SDLC को सुरुवाती चरणतर्फ सार्ने अभ्यास।

- Requirement review र acceptance criteria।
- Design review र threat modeling।
- Development कै क्रममा unit/component/API tests।
- Pull request मा lint, type-check र automated test।

### ८.२ Continuous Testing

Development र delivery प्रक्रियामा आवश्यक automated/manual testing निरन्तर चलाउने अभ्यास। प्रत्येक test सबै commit मा चलाउनुपर्छ भन्ने होइन; गति, लागत र जोखिमअनुसार pipeline बनाइन्छ।

### ८.३ Shift-Right Testing

Release पछि वास्तविक प्रयोगको व्यवहारबाट सिक्ने अभ्यास।

- Production health monitoring र error rates।
- सुरक्षित रूपमा प्रयोगकर्ता feedback सङ्कलन।
- Canary/gradual release जहाँ उपयुक्त हुन्छ।
- Alerts, incident review र post-release verification।

```text
Requirement → Design → Development → Integration/System Test → Release
     ↑            ↑          ↑                 ↑                 ↓
   Review       Review   Unit/API Tests   E2E/Security      Monitoring
     └────────────── feedback and improvement loop ───────────────┘
```

तीनै अभ्यास एकअर्काका विकल्प होइनन्; सँगै प्रयोग गर्न सकिन्छ।

---

## ९. Requirement र Acceptance Criteria को उदाहरण

Requirement ले प्रणालीले के गर्नुपर्छ भन्ने स्पष्ट रूपमा बताउनुपर्छ। QA ले requirement लाई testable acceptance criteria र test cases मा रूपान्तरण गर्न मद्दत गर्छ।

### ९.१ अस्पष्ट Requirement

> “प्रयोगकर्ताले पासवर्ड रिसेट गर्न सक्ने हुनुपर्छ।”

यो उपयोगी सुरुवात हो, तर reset कसरी हुन्छ, link कति समय मान्य हुन्छ, link पुनः प्रयोग गर्न मिल्छ कि मिल्दैन र account enumeration कसरी रोक्ने भन्ने खुल्दैन।

### ९.२ सुधारिएको Requirement

- **Requirement ID:** `AUTH-001`
- **शीर्षक:** Password Reset Functionality
- **प्रकार:** Functional + Security
- **विवरण:** प्रयोगकर्ताले सुरक्षित password-reset प्रक्रिया प्रयोग गरी आफ्नो पासवर्ड परिवर्तन गर्न सक्ने हुनुपर्छ। अनुरोध प्राप्त भएपछि प्रणालीले दर्ता भएको email ठेगानामा reset link पठाउने प्रक्रिया सुरु गर्नुपर्छ।

**Acceptance Criteria:**
1. Login page बाट “Forgot Password” विकल्प खोल्न सकिन्छ।
2. प्रयोगकर्ताले email ठेगाना पेश गर्न सक्छ।
3. सार्वजनिक प्रतिक्रियाले email दर्ता छ कि छैन भन्ने अनावश्यक रूपमा खुलासा गर्दैन।
4. Reset token अनुमान गर्न कठिन, सुरक्षित र सीमित अवधिसम्म मात्र मान्य हुन्छ।
5. Token एकपटक प्रयोग भएपछि अमान्य हुन्छ।
6. मान्य token बाट नयाँ password नीति अनुसार सेट गर्न सकिन्छ।
7. अमान्य, expired वा प्रयोग भइसकेको token बाट password परिवर्तन हुँदैन।
8. सफल reset पछि पुष्टि सन्देश देखिन्छ।
9. Password reset गर्दा पुराना session/token revoke गर्ने व्यवहार स्पष्ट रूपमा परिभाषित गरिन्छ।
10. Reset token वा password plaintext रूपमा logs मा लेखिँदैन।

**थप सुरक्षा विचार:**
- Token database मा भण्डारण गर्दा सम्भव भएसम्म token को hash मात्र राख्ने।
- Reset link HTTPS बाट मात्र खोल्ने।
- Registered र unregistered email का लागि सार्वजनिक प्रतिक्रिया समान राख्ने; response timing बाट account existence खुल्ने जोखिम पनि विचार गर्ने।
- Rate limiting वा abuse protection लागू गर्ने।

> Token expiry को ठ्याक्कै अवधि (उदाहरणका लागि 10–30 मिनेट) परियोजनाको security policy अनुसार तय गर्नुपर्छ; यो उदाहरण सार्वभौमिक नियम होइन।

### ९.३ QA Test Cases

| ID | परीक्षण अवस्था | परीक्षण चरण | अपेक्षित नतिजा |
|---|---|---|---|
| TC-01 | दर्ता भएको email | Reset अनुरोध | सुरक्षित reset प्रक्रिया सुरु हुन्छ; सार्वजनिक सन्देशले account existence खुलाउँदैन |
| TC-02 | दर्ता नभएको email | Reset अनुरोध | समान प्रकारको सामान्य सन्देश; account enumeration जोखिम घटाइन्छ |
| TC-03 | गलत ढाँचाको email | Reset अनुरोध | स्पष्ट validation; अनुचित request अस्वीकार |
| TC-04 | Valid reset link | नयाँ password पेश | Password policy पूरा भए reset सफल |
| TC-05 | Expired token | Link खोल्ने | Password परिवर्तन अस्वीकार |
| TC-06 | Reused token | दोस्रोपटक प्रयोग | Password परिवर्तन अस्वीकार |
| TC-07 | कमजोर password | नयाँ password पेश | नीति अनुसार अस्वीकार र उपयोगी error |
| TC-08 | सफल reset | नयाँ password बाट login | नयाँ password बाट login सम्भव; session revocation नीति लागू |
| TC-09 | धेरै reset requests | Rate/abuse check | Rate limit वा abuse protection नीति लागू |
| TC-10 | Logging जाँच | Reset flow | Password/token plaintext log नभएको |

### ९.४ राम्रो Requirement का गुण

- **Clear:** एउटै अर्थ लाग्ने।
- **Complete:** आवश्यक अवस्था र अपवाद समेटिएको।
- **Consistent:** अर्को requirement सँग विरोधाभास नभएको।
- **Feasible:** समय, बजेट र प्रविधिले सम्भव हुने।
- **Testable:** पास/फेल निर्धारण गर्न सकिने।
- **Traceable:** requirement बाट test case र release evidence सम्म सम्बन्ध देखाउन सकिने।
- **Prioritized:** महत्त्व र जोखिमअनुसार क्रम निर्धारण गरिएको।

---

## १०. Test Levels र Test Types

### १०.१ मुख्य Test Levels

| स्तर | के जाँचिन्छ? | MERN उदाहरण |
|---|---|---|
| Unit Testing | सानो function/module अलग्गै | password validation helper |
| Component Testing | UI component वा component समूह | React login form validation |
| Integration Testing | दुई वा बढी भागबीचको सम्बन्ध | Express route + service + MongoDB |
| System Testing | सम्पूर्ण integrated system ले निर्दिष्ट requirement पूरा गर्छ कि गर्दैन | सम्पूर्ण नगरपालिका पोर्टलको functional/system checks |
| End-to-End (E2E) Testing | प्रयोगकर्ताको सुरुदेखि अन्त्यसम्मको workflow | Login → आवेदन → submit → status हेर्ने |
| Acceptance Testing (UAT) | प्रयोगकर्ता/व्यावसायिक आवश्यकता पूरा भए/नभएको | वडा कर्मचारीले वास्तविक कार्यप्रवाह स्वीकार गर्ने |

**System Testing र E2E Testing एउटै होइनन्।** System Testing ले सम्पूर्ण प्रणालीको व्यवहार र requirement coverage जाँच्छ। E2E Testing ले वास्तविक प्रयोगकर्ताको workflow सुरुदेखि अन्त्यसम्म पूरा हुन्छ कि हुँदैन भन्नेमा विशेष ध्यान दिन्छ। व्यवहारमा यी परीक्षणका केही क्षेत्र एकअर्कासँग overlap हुन सक्छन्।

### १०.२ सामान्य Test Types

- **Functional Testing:** सुविधा आवश्यकता अनुसार चल्छ कि चल्दैन।
- **Regression Testing:** नयाँ परिवर्तनले पुरानो सुविधा बिगारेको छ कि छैन।
- **Smoke Testing:** build/deployment का मुख्य सुविधाहरू आधारभूत रूपमा चल्छन् कि चल्दैनन्।
- **Sanity Testing:** सीमित परिवर्तनपछि सम्बन्धित भागको छिटो जाँच।
- **Security Testing:** authentication, authorization, input validation, access control र अन्य जोखिम।
- **Performance/Load Testing:** response time, throughput र निर्धारित load मा व्यवहार।
- **Usability Testing:** प्रयोग गर्न सहज छ कि छैन।
- **Accessibility Testing:** keyboard, labels, contrast, screen reader आदि आवश्यकताहरू।
- **Responsive/Cross-browser Testing:** फरक screen size र browser मा व्यवहार।
- **Recovery/Backup Testing:** failure पछि recovery र backup restore सम्भव छ कि छैन।
- **Compatibility Testing:** समर्थित browser/device/environment मा प्रणाली चल्छ कि चल्दैन।

### १०.३ Severity र Priority

- **Severity:** defect ले प्रणाली वा प्रयोगकर्तामा कति गम्भीर असर पार्छ?
- **Priority:** defect कति छिटो समाधान गर्नुपर्छ?

उदाहरण: संवेदनशील नागरिक विवरण अर्को वडाले हेर्न सक्नु उच्च severity र उच्च priority हुन सक्छ। UI मा सानो spacing समस्या कम severity भए पनि release वा demo अघि उच्च priority पाउन सक्छ।

---

## ११. MERN Project मा SDLC र QA

React + Node.js/Express + MongoDB परियोजनाका लागि तलको workflow उपयोगी सुरुवात हो।

### चरण १: Requirement र Backlog

- प्रत्येक feature को उद्देश्य, user role र acceptance criteria लेख्ने।
- Happy path सँगै invalid input, permission denied र failure states लेख्ने।
- Feature लाई जोखिम र मूल्यअनुसार प्राथमिकता दिने।
- Requirement ID लाई test cases सँग जोड्ने।

**Deliverables:** `REQUIREMENTS.md`, user stories, acceptance criteria, prioritized backlog।

### चरण २: UI/UX र Architecture Design

- Wireframes/prototype, responsive states र form error states समीक्षा गर्ने।
- API request/response contract र status codes परिभाषित गर्ने।
- MongoDB schema, indexes र data relationships समीक्षा गर्ने।
- Role/permission matrix तयार गर्ने।
- Threat model: sensitive data, trust boundaries र misuse cases पहिचान गर्ने।

**Deliverables:** design notes, API specification, data model, permission matrix, test plan।

### चरण ३: Development + Developer Testing

- Feature branch र pull request workflow प्रयोग गर्ने।
- Lint/type-check र code review चलाउने।
- Unit/component tests लेख्ने।
- Backend मा server-side validation, authorization र centralized error handling लागू गर्ने।
- Test data र environment variables सुरक्षित रूपमा व्यवस्थापन गर्ने।

**Deliverables:** code, tests, review record, defect list।

### चरण ४: Integration र System Testing

- Frontend → API → database सम्म data flow जाँच्ने।
- Authentication र authorization सबै protected endpoints मा verify गर्ने।
- Role-based access matrix अनुसार सकारात्मक र नकारात्मक tests चलाउने।
- Mobile layout, keyboard navigation र लामो नेपाली text जाँच्ने।
- Regression suite चलाउने।
- E2E test मार्फत महत्त्वपूर्ण user journey पूरा हुन्छ कि जाँच्ने।

**उदाहरणका test scenarios:**
- नागरिकले आफ्नै आवेदन मात्र हेर्न पाउने।
- वडा कर्मचारीले अनुमति प्राप्त वडाको record मात्र access गर्ने।
- Role नभएको user ले admin API call गर्दा नीति अनुसार `401` वा `403` बाट अस्वीकार हुने।
- Client-side validation bypass गरे पनि backend ले invalid data अस्वीकार गर्ने।
- Database वा email service असफल हुँदा उपयोगी error र सुरक्षित logging हुने।

### चरण ५: Security, Performance र Accessibility

- Dependency vulnerability scan र static analysis चलाउने।
- Secrets repository मा commit नभएको जाँच्ने।
- Rate limiting, secure cookies/session/JWT handling र CORS configuration समीक्षा गर्ने।
- Object-level authorization र IDOR-जस्ता जोखिम परीक्षण गर्ने।
- उचित test environment मा load/performance test गर्ने।
- Labels, keyboard focus, contrast, error announcements र responsive overflow जाँच्ने।

**सुरक्षा नोट:** Testing आफूले अधिकार पाएको development/staging environment मा गर्नुहोस्। Production मा intrusive load/security test गर्नुअघि स्पष्ट स्वीकृति र योजना चाहिन्छ।

### चरण ६: Staging र Release तयारी

- Production-जस्तै staging environment मा critical workflows चलाउने।
- Environment variables र secrets deployment platform मा configure गर्ने।
- Database migration तथा backup/restore योजना जाँच्ने।
- Release notes, rollback plan र incident contact तयार गर्ने।
- Release को risk अनुसार quality gate पास भएपछि मात्र production मा जाने।

### चरण ७: Deployment र Post-release Verification

- Build/deploy result र health checks जाँच्ने।
- Login, प्रमुख API, database connectivity र मुख्य user journey का smoke tests चलाउने।
- Logs, error rate, latency, resource use र backup status monitor गर्ने।
- समस्या आएमा rollback/mitigation प्रक्रिया अपनाउने।

### चरण ८: Maintenance र Feedback

- Defect को root cause विश्लेषण गर्ने।
- Fix पछि regression tests चलाउने।
- Dependencies र security advisories समीक्षा गर्ने।
- Backup को सफलतासँगै restore परीक्षण पनि गर्ने।
- प्रयोगकर्ता feedback बाट backlog अद्यावधिक गर्ने।

### प्रत्येक Feature को सानो cycle

```text
Requirement + Acceptance Criteria
              ↓
       Design / Risk Review
              ↓
          Development
              ↓
  Unit / Component / API Tests
              ↓
      Integration / E2E Tests
              ↓
        Fix + Regression
              ↓
     Review + Quality Gate
              ↓
            Release
              ↓
    Monitor + Feedback → Next Cycle
```

---

## १२. Quality Gates र Definition of Done

### १२.१ उदाहरणीय Quality Gates

- [ ] सबै critical/high-priority requirements र acceptance criteria समीक्षा भएका छन्।
- [ ] Pull request/code review पूरा भएको छ।
- [ ] आवश्यक unit, integration र E2E tests पास भएका छन्।
- [ ] Known critical/high security defects बाँकी छैनन्, वा औपचारिक risk acceptance गरिएको छ।
- [ ] Role/permission र sensitive-data access परीक्षण गरिएको छ।
- [ ] आवश्यक responsive, accessibility र browser checks पास भएका छन्।
- [ ] Production secrets/configuration सुरक्षित रूपमा सेट गरिएको छ।
- [ ] Database migration, backup र rollback योजना तयार छ।
- [ ] Staging smoke test पास भएको छ।
- [ ] Monitoring, logging र alerting आवश्यकताअनुसार तयार छन्।
- [ ] Release पछि smoke test र जिम्मेवार व्यक्ति तोकिएको छ।

यी उदाहरण हुन्; सबै परियोजनामा एउटै gate अनिवार्य हुँदैन। जोखिम र नियमनअनुसार gate परिभाषित गर्नुपर्छ।

### १२.२ Definition of Done (DoD)

कुनै feature “Done” मानिने न्यूनतम साझा मापदण्ड हो। उदाहरण:
- Acceptance criteria पूरा।
- Code review स्वीकृत।
- आवश्यक automated tests पास।
- Validation, authorization र error handling लागू।
- UI responsive तथा आवश्यक accessibility जाँच पूरा।
- Documentation/observability आवश्यकताअनुसार अद्यावधिक।
- ज्ञात defect र बाँकी जोखिम स्पष्ट रूपमा लेखिएको।

**“मेरो कम्प्युटरमा चल्यो” मात्र Done को प्रमाण होइन।**

---

## १३. सामान्य गल्ती र राम्रो अभ्यास

| सामान्य गल्ती | राम्रो अभ्यास |
|---|---|
| सबै code बनेपछि मात्र QA बोलाउने | Requirement review देखि नै quality activity सुरु गर्ने |
| Requirement अस्पष्ट राख्ने | Testable acceptance criteria लेख्ने |
| Frontend validation मात्र गर्ने | Backend मा पनि authoritative validation गर्ने |
| Login जाँचेर authorization नजाँच्ने | प्रत्येक role र resource access test गर्ने |
| केवल happy path जाँच्ने | Negative, edge, failure र abuse cases समेट्ने |
| Unit tests मात्र भएर E2E नगर्ने | जोखिमअनुसार unit देखि end-to-end सम्म परीक्षण गर्ने |
| Test पास भयो भन्दै सबै गुणस्तर प्रमाणित ठान्ने | Test scope, environment र बाँकी जोखिम दस्तावेज गर्ने |
| Production मा सिधै पहिलो परीक्षण गर्ने | Staging, release checklist र smoke test प्रयोग गर्ने |
| Backup बनेको देखेर restore सम्भव ठान्ने | Restore drill नियमित रूपमा गर्ने |
| Bug fix पछि पुराना test नचलाउने | Regression tests पुनः चलाउने |
| सबै test हरेक commit मा चलाउने | गति, लागत र जोखिमअनुसार test pipeline डिजाइन गर्ने |
| DevOps लाई deployment tool मात्र ठान्ने | Automation, collaboration, monitoring र feedback सहित बुझ्ने |
| System Testing र E2E लाई एउटै मान्ने | उद्देश्य र scope स्पष्ट गरी छुट्टाछुट्टै परिभाषित गर्ने |

---

## १४. शब्दावली

| शब्द | नेपाली अर्थ/सरल व्याख्या |
|---|---|
| SDLC | सफ्टवेयर विकास जीवनचक्र |
| Requirement | आवश्यकता |
| Scope | परियोजनाको दायरा |
| Functional Requirement | प्रणालीले गर्नुपर्ने कार्य |
| Non-functional Requirement | गुणस्तर/सञ्चालनसम्बन्धी अपेक्षा |
| Acceptance Criteria | सुविधा स्वीकार गर्न पूरा हुनुपर्ने स्पष्ट सर्त |
| Design | संरचना र व्यवहारको योजना |
| Architecture | प्रणालीका मुख्य भाग र तिनको सम्बन्ध |
| QA | गुणस्तर सुनिश्चितता |
| QC | गुणस्तर नियन्त्रण |
| Test Case | परीक्षण अवस्था, input, steps र expected result |
| Defect/Bug | अपेक्षित र वास्तविक व्यवहारबीचको त्रुटि |
| Regression Testing | परिवर्तनले पुरानो सुविधा बिगारेको छ कि छैन जाँच |
| UAT | प्रयोगकर्ता स्वीकृति परीक्षण |
| CI | Continuous Integration |
| CD | Continuous Delivery/Deployment; सन्दर्भअनुसार अर्थ फरक हुन सक्छ |
| CI/CD | build, test र release/deployment स्वचालित गर्ने pipeline अभ्यास |
| Sprint | Scrum मा निश्चित अवधिको काम गर्ने अवधि |
| Backlog | प्राथमिकताबद्ध काम/आवश्यकताको सूची |
| Prototype | प्रारम्भिक नमुना |
| Deployment | सफ्टवेयरलाई target environment मा प्रकाशित गर्ने प्रक्रिया |
| Production | वास्तविक प्रयोगकर्ताले प्रयोग गर्ने वातावरण |
| Smoke Test | मुख्य कार्यहरू आधारभूत रूपमा चल्छन् कि जाँच |
| Shift-Left | गुणस्तर जाँचलाई सुरुवाती चरणतर्फ सार्ने |
| Shift-Right | release पछिको व्यवहार/feedback बाट सिक्ने |
| Rollback | परिवर्तन समस्या हुँदा अघिल्लो सुरक्षित अवस्थामा फर्काउने |
| Traceability | requirement, test र result बीचको सम्बन्ध पछ्याउन सक्ने अवस्था |

---

## १५. अभ्यास प्रश्न र उत्तर

पहिले आफैँ उत्तर दिनुहोस्; त्यसपछि उत्तर कुञ्जी हेर्नुहोस्।

### भाग A — बहुविकल्पीय प्रश्न

**१. SDLC को पूरा रूप के हो?**
- A. Software Design Level Control
- B. Software Development Life Cycle
- C. System Data Link Cycle
- D. Software Deployment Logic Code

**२. आवश्यकता स्पष्ट र स्थिर भएको परियोजनामा कुन model उपयुक्त हुन सक्छ?**
- A. Waterfall
- B. Spiral मात्र
- C. Scrum मात्र
- D. Prototype मात्र

**३. Agile अन्तर्गत Sprint प्रयोग गर्ने framework कुन हो?**
- A. V-Model
- B. Waterfall
- C. Scrum
- D. Spiral

**४. जोखिम विश्लेषणमा विशेष जोड दिने model कुन हो?**
- A. Waterfall
- B. Spiral
- C. V-Model
- D. Scrum

**५. Deployment पछि नियमित bug fixing र updates कुन चरणमा पर्छन्?**
- A. Design
- B. Requirement
- C. Maintenance
- D. Initial Planning

**६. QA किन Requirement चरणबाटै सुरु गर्नुपर्छ?**
- A. Coding हटाउन
- B. अस्पष्ट/गलत आवश्यकता चाँडै पत्ता लगाउन
- C. Testing आवश्यक नपरोस् भनेर
- D. Deployment तुरुन्त गर्न

**७. V-Model को विशेषता के हो?**
- A. Testing सधैँ हटाइन्छ
- B. Development चरण र testing चरणबीच सम्बन्ध हुन्छ
- C. केवल UI बनाइन्छ
- D. कुनै documentation हुँदैन

**८. DevOps ले मुख्यतः केमा जोड दिन्छ?**
- A. Development र Operations बीच सहकार्य, automation र feedback
- B. केवल manual testing
- C. केवल database design
- D. Requirement नलेख्ने

**९. Reset password link को कुन व्यवहार सुरक्षित अभ्यास हो?**
- A. सधैँ मान्य रहने
- B. धेरैपटक प्रयोग गर्न मिल्ने
- C. सीमित अवधिसम्म मान्य र एकपटक प्रयोग गर्न मिल्ने
- D. Password नै URL मा राख्ने

**१०. Backend authorization किन आवश्यक छ?**
- A. UI सुन्दर बनाउन
- B. Client-side control मात्र पर्याप्त हुने भएकाले
- C. अनधिकृत API/resource access रोक्न
- D. Database हटाउन

**११. System Testing र E2E Testing बारे कुन भनाइ सही हो?**
- A. दुवै सधैँ एउटै हुन्
- B. E2E ले workflow सुरुदेखि अन्त्यसम्म जाँच्छ; System Testing ले सम्पूर्ण प्रणालीको requirement conformance जाँच्छ
- C. E2E मा कुनै user workflow हुँदैन
- D. System Testing केवल रंग जाँच्ने हो

### भाग B — छोटो उत्तर

1. SDLC phases र SDLC models बीचको फरक लेख्नुहोस्।
2. QA, QC र Testing बीच कम्तीमा तीन फरक लेख्नुहोस्।
3. Shift-Left Testing के हो? MERN project बाट एउटा उदाहरण दिनुहोस्।
4. Functional र Non-functional requirement को एक-एक उदाहरण लेख्नुहोस्।
5. Scrum र Agile एउटै कुरा किन होइनन्?
6. Production deployment अघि जाँच्नुपर्ने पाँचवटा विषय लेख्नुहोस्।
7. Feature “Done” मान्नुअघि Definition of Done मा के-के समावेश गर्न सकिन्छ?
8. Requirement बाट Test Case सम्म traceability किन उपयोगी हुन्छ?
9. System Testing र E2E Testing बीचको फरक उदाहरणसहित लेख्नुहोस्।

### भाग C — व्यावहारिक अभ्यास

**अभ्यास १: नगरपालिकाको अनलाइन सिफारिस**

निम्न विषय समेटेर एउटा requirement तयार गर्नुहोस्:
- नागरिकले आवेदन भर्न सक्ने।
- आवश्यक कागजात upload गर्न सक्ने।
- आवेदनको अवस्था हेर्न सक्ने।
- कर्मचारीले आफ्नो अधिकारभित्रका आवेदन मात्र हेर्न सक्ने।

कम्तीमा ५ acceptance criteria र ५ test cases लेख्नुहोस्। Invalid file, unauthorized access र network failure जस्ता अवस्थासमेत विचार गर्नुहोस्।

**अभ्यास २: QA सुरुदेखि लागू गर्ने**

कुनै एउटा feature छान्नुहोस् र Requirement, Design, Development, Testing, Deployment र Maintenance मा गरिने quality activities को सूची बनाउनुहोस्।

**अभ्यास ३: Release checklist**

आफ्नो परियोजनाका लागि critical user journey, security, responsive UI, database backup/restore, environment configuration, smoke tests र rollback समेटिएको checklist तयार गर्नुहोस्।

### उत्तर कुञ्जी — भाग A

| प्रश्न | सही उत्तर | कारण |
|---|---|---|
| १ | B — Software Development Life Cycle | SDLC को पूरा रूप यही हो। |
| २ | A — Waterfall | स्पष्ट र स्थिर आवश्यकता भएको अवस्थामा उपयुक्त हुन सक्छ। |
| ३ | C — Scrum | Scrum मा काम Sprint मार्फत व्यवस्थित गरिन्छ। |
| ४ | B — Spiral | प्रत्येक चक्रमा जोखिम विश्लेषण महत्त्वपूर्ण हुन्छ। |
| ५ | C — Maintenance | Release पछिको सुधार र updates यसमा पर्छन्। |
| ६ | B — आवश्यकता चाँडै पत्ता लगाउन | Requirement review ले गलत बुझाइ र rework घटाउन मद्दत गर्छ। |
| ७ | B — विकास र testing बीच सम्बन्ध | V-Model मा test planning/traceability महत्त्वपूर्ण हुन्छ। |
| ८ | A — सहकार्य, automation र feedback | DevOps ले delivery र operations सुधारमा जोड दिन्छ। |
| ९ | C — सीमित अवधि र एकपटक प्रयोग | यसले reset-token दुरुपयोगको जोखिम घटाउँछ। |
| १० | C — अनधिकृत access रोक्न | Client-side UI bypass गर्न सकिन्छ; server ले अधिकार जाँच्नुपर्छ। |
| ११ | B — System Testing र E2E का उद्देश्य फरक छन् | दुवै overlap हुन सक्छन्, तर तिनको मुख्य focus एउटै होइन। |

---

## १६. छोटो पुनरावलोकन

- SDLC का चरणहरूको संख्या र नाम प्रयोग गरिएको प्रक्रियाअनुसार फरक हुन सक्छ। यस नोटमा Planning सहितको सामान्य प्रक्रिया र ६ चरणको प्रचलित वर्गीकरण व्याख्या गरिएको छ।
- सामान्य ६ चरण: **Requirement → Design → Development → Testing → Deployment → Maintenance**।
- Phases ले *के काम हुन्छ* भन्छन्; models/approaches ले *काम कसरी व्यवस्थित हुन्छ* बताउँछन्।
- Waterfall क्रमिक, Agile पुनरावृत्तिमूलक, Scrum Sprint-आधारित framework, V-Model development/testing mapping, Spiral risk-based र Prototyping feedback-आधारित हो।
- DevOps ले Development र Operations बीच automation, collaboration, monitoring र feedback जोड्छ।
- **QA Requirement चरणदेखि सुरु हुन्छ; Testing पनि विकासको क्रममा र release अघि/पछि आवश्यकताअनुसार चल्छ।**
- Shift-Left ले सुरुवाती जाँच, Continuous Testing ले delivery क्रममा जाँच र Shift-Right ले release पछिको feedback/monitoring मा जोड दिन्छ।
- राम्रो requirement स्पष्ट, पूर्ण, consistent र testable हुनुपर्छ।
- System Testing र E2E Testing सम्बन्धित भए पनि तिनको उद्देश्य र scope पूर्ण रूपमा एउटै होइन।
- MERN परियोजनामा frontend, backend, database, authentication, authorization, security, responsive UI र end-to-end workflow सबै परीक्षण गर्नुपर्छ।
- Production मा release गर्नु अघि जोखिमअनुसार quality gates पास हुनुपर्छ; release पछि monitoring, backup/restore र maintenance जारी रहन्छ।

> **अन्तिम सम्झना:** गुणस्तर अन्तिममा परीक्षण गरेर मात्र थपिने वस्तु होइन। आवश्यकता, design, code, test, deployment र maintenance — हरेक चरणमा गुणस्तर निर्माण गर्नुपर्छ।

---

## १७. थप अध्ययनका स्रोत

यी स्रोतहरू अवधारणा थप बुझ्नका लागि हुन्। यस नोटका सबै वाक्य वा उदाहरण कुनै एउटै स्रोतबाट जस्ताको तस्तै लिइएका होइनन्।

- **ISTQB Glossary:** Software Testing का शब्दावली र testing अवधारणा — https://glossary.istqb.org/
- **The Scrum Guide:** Scrum framework को आधिकारिक guide — https://scrumguides.org/
- **OWASP Cheat Sheet Series:** Web application security अभ्यासहरू — https://cheatsheetseries.owasp.org/
- **OWASP Web Security Testing Guide:** Web application security testing का मार्गदर्शन — https://owasp.org/www-project-web-security-testing-guide/
