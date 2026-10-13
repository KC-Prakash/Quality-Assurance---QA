## विषयसूची

1. Software Testing Life Cycle (STLC) परिचय
2. STLC र SDLC बीचको फरक
3. STLC का मुख्य चरणहरू
4. उदाहरणका लागि प्रयोग गरिने परियोजना
5. चरण १ — Requirement Analysis
6. चरण २ — Test Planning
7. चरण ३ — Test Case Design / Test Design
8. चरण ४ — Test Environment Setup
9. चरण ५ — Test Execution
10. चरण ६ — Test Closure
11. STLC मा प्रयोग हुने मुख्य कागजात
12. Bug / Defect Life Cycle
13. Severity र Priority
14. Test Metrics र रिपोर्टिङ
15. Risk-Based Testing
16. Traceability Matrix (RTM)
17. Automation Testing र STLC
18. Agile/Scrum मा STLC
19. Beginner देखि Advanced सम्म अभ्यास योजना
20. अभ्यास प्रश्न तथा उत्तर
21. Glossary — महत्त्वपूर्ण शब्दावली
22. अन्तिम पुनरावलोकन चेकलिस्ट

---

# १. Software Testing Life Cycle (STLC) परिचय

## १.१ Software Testing भनेको के हो?

Software Testing भनेको सफ्टवेयरले तोकिएका आवश्यकता (Requirements) अनुसार काम गर्छ कि गर्दैन, अपेक्षित र वास्तविक नतिजा मिल्छ कि मिल्दैन, र त्यसमा त्रुटि वा जोखिम छन् कि छैनन् भनेर व्यवस्थित रूपमा जाँच्ने प्रक्रिया हो।

**उदाहरण:** अनलाइन लगइन पेजमा सही इमेल र पासवर्ड राख्दा प्रयोगकर्ता लगइन हुनुपर्छ। गलत पासवर्ड राख्दा लगइन हुनु हुँदैन र उपयुक्त त्रुटि सन्देश देखिनुपर्छ। यी व्यवहार जाँच्नु Software Testing हो।

Testing को उद्देश्य केवल bug खोज्नु मात्र होइन। यसको उद्देश्य गुणस्तरबारे जानकारी दिनु, जोखिम घटाउनु, आवश्यकताहरू पूरा भएको प्रमाण जुटाउनु र निर्णय गर्न सहयोग गर्नु हो। परीक्षणले सबै bug छैनन् भनेर शतप्रतिशत प्रमाणित गर्न सक्दैन; यसले परीक्षण गरिएका अवस्थाहरूमा देखिएका परिणाम र बाँकी जोखिमबारे जानकारी दिन्छ।

## १.२ STLC भनेको के हो?

**Software Testing Life Cycle (STLC)** भनेको परीक्षण कार्यलाई योजनाबद्ध, चरणबद्ध र मापनयोग्य तरिकाले सम्पन्न गर्न प्रयोग गरिने प्रक्रिया हो। प्रत्येक चरणमा निश्चित गतिविधि, परिणाम (Deliverables) र प्रवेश/समापन मापदण्ड हुन्छन्।

धेरै संस्थामा STLC का चरणहरू यसरी प्रस्तुत गरिन्छन्:

1. Requirement Analysis
2. Test Planning
3. Test Case Design / Test Design
4. Test Environment Setup
5. Test Execution
6. Test Closure

कहिलेकाहीँ पाँच चरणको मोडेलमा Environment Setup लाई Test Planning वा Test Execution सँग समेटिन्छ। त्यसैले कम्पनीअनुसार नाम र विभाजन केही फरक हुन सक्छ। यस नोटमा बुझ्न सजिलो होस् भनेर छवटै चरण समेटिएका छन्।

## १.३ STLC किन आवश्यक छ?

- परीक्षणलाई व्यवस्थित र दोहोर्‍याउन मिल्ने बनाउँछ।
- कुन सुविधा, कुन जोखिम र कुन उपकरण परीक्षण गर्ने भन्ने स्पष्ट गर्छ।
- आवश्यकताबाट Test Case सम्मको सम्बन्ध देखाउँछ।
- समय, बजेट र जनशक्तिको राम्रो उपयोग गर्न मद्दत गर्छ।
- दोष छिटो पत्ता लगाउन र सुधारको पुष्टि गर्न सहयोग गर्छ।
- परीक्षणको प्रगति र बाँकी जोखिमबारे Stakeholder लाई जानकारी दिन्छ।
- Release गर्ने/नगर्ने निर्णयका लागि प्रमाण उपलब्ध गराउँछ।

## १.४ STLC को सरल Flow

```text
Requirements प्राप्त
       ↓
1. Requirement Analysis
       ↓
2. Test Planning
       ↓
3. Test Case Design
       ↓
4. Test Environment Setup
       ↓
5. Test Execution ──── Defect भेटियो? ── हो → Log → Fix → Retest
       ↓                                      ↑       ↓
       └──────────────── Regression Test ←────┘
       ↓
6. Test Closure
```

यो सधैँ सीधा र एकपटक मात्र चल्ने प्रक्रिया होइन। आवश्यकता परिवर्तन, नयाँ build, defect fix वा जोखिम भेटिएमा अघिल्लो चरणमा फर्किन सकिन्छ। Agile परियोजनामा यी गतिविधि प्रत्येक Sprint वा feature अनुसार दोहोरिन्छन्।

---

# २. STLC र SDLC बीचको फरक

**SDLC (Software Development Life Cycle)** ले आवश्यकता पहिचानदेखि डिजाइन, विकास, परीक्षण, Deployment र Maintenance सम्म सफ्टवेयर निर्माण तथा सञ्चालनको समग्र जीवनचक्र समेट्छ।

**STLC** ले त्यस SDLC भित्रको Testing सम्बन्धी कामलाई व्यवस्थित गर्छ।

| आधार | SDLC | STLC |
|---|---|---|
| पूरा नाम | Software Development Life Cycle | Software Testing Life Cycle |
| मुख्य उद्देश्य | सफ्टवेयर निर्माण, वितरण र मर्मत | सफ्टवेयरको गुणस्तर जाँच र जोखिम मूल्याङ्कन |
| मुख्य गतिविधि | Requirement, Design, Coding, Testing, Deployment, Maintenance | Requirement Analysis, Planning, Test Design, Setup, Execution, Closure |
| संलग्न व्यक्ति | Product Owner, BA, Designer, Developer, Tester, Operations आदि | QA/Test Engineer, Test Lead, Developer, BA, Product Owner आदि |
| नतिजा | काम गर्ने Software/Product | Test Evidence, Defect Reports, Coverage र Quality/Risk Report |
| सम्बन्ध | व्यापक जीवनचक्र | Testing केन्द्रित जीवनचक्र; SDLC सँगै चल्न सक्छ |

### महत्त्वपूर्ण कुरा: Testing विकासपछि मात्र सुरु हुनुपर्छ भन्ने होइन

Testing सम्बन्धी काम आवश्यकता तयार हुँदै गर्दा नै सुरु गर्न सकिन्छ। उदाहरणका लागि, Requirement Analysis चरणमै अस्पष्ट requirement भेटेर स्पष्ट पार्दा पछि code बनेपछि भेटिने महँगो defect घट्न सक्छ। यसलाई **Shift Left Testing** भनिन्छ।

- Requirement चरण: आवश्यकता review र testability जाँच।
- Design चरण: architecture, API र security सम्बन्धी review।
- Coding चरण: unit test, static analysis, code review।
- Build उपलब्ध भएपछि: integration, system र UI testing।
- Release पछि: production monitoring, smoke test वा आवश्यकतानुसार post-release checks।

---

# ३. STLC का मुख्य चरणहरू — एक नजरमा

| चरण | मुख्य प्रश्न | प्रमुख गतिविधि | मुख्य Deliverables |
|---|---|---|---|
| Requirement Analysis | के परीक्षण गर्नुपर्छ? | आवश्यकता बुझ्ने, अस्पष्टता पत्ता लगाउने, testability र जोखिम पहिचान | Requirement Questions, Testable Requirements, RTM को प्रारम्भिक रूप |
| Test Planning | कसरी, कसले, कहिले र कति स्रोतमा परीक्षण गर्ने? | Scope, strategy, resource, schedule, tools, risk र exit criteria निर्धारण | Test Plan / Test Strategy |
| Test Case Design | कुन-कुन अवस्थाबाट परीक्षण गर्ने? | Test scenarios, cases, data, expected result र traceability तयार | Test Cases, Test Data, RTM |
| Test Environment Setup | कहाँ र कुन configuration मा परीक्षण गर्ने? | Build, server, database, account, device र tool तयार/जाँच | Environment Readiness / Smoke Test Result |
| Test Execution | वास्तविक नतिजा अपेक्षित नतिजासँग मिल्छ? | Test चलाउने, evidence राख्ने, defect log गर्ने, retest र regression | Execution Report, Defect Reports |
| Test Closure | परीक्षणको स्थिति र बाँकी जोखिम के छ? | मेट्रिक्स, coverage, defect status, lessons learned र sign-off | Test Summary/Closure Report |

---

# ४. उदाहरणका लागि प्रयोग गरिने परियोजना

यस नोटभरि **नगरपालिका अनलाइन सेवा पोर्टल** को उदाहरण प्रयोग गरिन्छ। नागरिकले खाता खोलेर लगइन गर्ने, “चार किल्ला प्रमाणित” जस्ता सेवाका लागि निवेदन दिने, कागजात अपलोड गर्ने र निवेदनको स्थिति हेर्ने सुविधा भएको कल्पना गरौँ।

## नमुना Requirement

**REQ-LOGIN-01:** दर्ता भएको प्रयोगकर्ताले सही इमेल/प्रयोगकर्ता नाम र पासवर्ड राखेपछि लगइन गर्न पाउनुपर्छ।

**REQ-LOGIN-02:** गलत प्रमाणिकरण विवरण राखेमा लगइन अस्वीकार गरी सुरक्षित र बुझिने सन्देश देखाउनुपर्छ।

**REQ-LOGIN-03:** पासवर्ड लुकाइएको अवस्थामा देखिनुपर्छ; प्रयोगकर्ताले चाहेको बेला मात्र देखाउन सक्ने सुविधा हुन सक्छ।

**REQ-SERVICE-01:** अनिवार्य विवरण नभरिएको निवेदन बुझाउन मिल्नु हुँदैन।

**REQ-UPLOAD-01:** प्रणालीले अनुमति दिइएका फाइल प्रकार र आकार मात्र स्वीकार गर्नुपर्छ।

यी उदाहरणहरू सिकाइका लागि हुन्; वास्तविक प्रणालीमा स्वीकृत आवश्यकता, लागू कानुन, सुरक्षा नीति र कार्यालयको कार्यविधि अनुसार नियम निश्चित गर्नुपर्छ।

---

# ५. चरण १ — Requirement Analysis

## ५.१ परिचय

Requirement Analysis STLC को पहिलो चरण हो। यसमा QA/Test Team ले Business Requirement, User Story, Acceptance Criteria, UI Design, API Specification र अन्य उपलब्ध कागजात अध्ययन गरेर **के परीक्षण गर्नुपर्छ** भन्ने बुझ्छ।

यो चरणमा मुख्य काम तुरुन्तै Test Case लेख्नु होइन; पहिले आवश्यकता सही, पूर्ण, स्पष्ट, परीक्षणयोग्य र एकअर्कासँग नमिल्ने विरोधाभासबाट मुक्त छ कि छैन भनेर जाँच्नु हो।

## ५.२ मुख्य उद्देश्य

- सबै परीक्षणयोग्य आवश्यकता पहिचान गर्ने।
- अस्पष्ट, अपूर्ण, विरोधाभासी वा असम्भव requirement पत्ता लगाउने।
- Functional र Non-functional आवश्यकता छुट्याउने।
- परीक्षणको scope र सम्भावित जोखिम बुझ्ने।
- कुन requirement कसरी परीक्षण गर्ने र कुन वातावरण/डेटा चाहिन्छ भन्ने प्रारम्भिक धारणा बनाउने।
- Product Owner, Business Analyst, Developer वा सम्बन्धित Stakeholder सँग प्रश्न स्पष्ट गर्ने।

## ५.३ Requirement का प्रकार

### A. Functional Requirements

प्रणालीले **के काम गर्नुपर्छ** भन्ने बताउँछन्।

उदाहरण:
- प्रयोगकर्ताले लगइन गर्न पाउनुपर्छ।
- नागरिकले सेवा निवेदन बुझाउन पाउनुपर्छ।
- कर्मचारीले निवेदन स्वीकृत वा अस्वीकृत गर्न पाउनुपर्छ।
- प्रयोगकर्ताले निवेदनको स्थिति हेर्न पाउनुपर्छ।

### B. Non-functional Requirements

प्रणालीले **कस्तो गुणस्तर वा सीमाभित्र काम गर्नुपर्छ** भन्ने बताउँछन्।

उदाहरण:
- Performance: सामान्य अवस्थामा पेज २ सेकेन्डभित्र देखिनुपर्छ (यो परियोजनाको स्वीकृत लक्ष्य हुनुपर्छ)।
- Security: अनुमति नभएको प्रयोगकर्ताले Admin पेज खोल्न पाउनु हुँदैन।
- Accessibility: Keyboard बाट मुख्य सुविधा प्रयोग गर्न मिल्नुपर्छ।
- Usability: त्रुटि सन्देश स्पष्ट र उपयोगी हुनुपर्छ।
- Compatibility: स्वीकृत browser/device मा काम गर्नुपर्छ।
- Reliability: असफल अनुरोध हुँदा डाटा दोहोरिएर सिर्जना हुनु हुँदैन।
- Scalability: प्रयोगकर्ता बढ्दा पनि स्वीकृत performance target कायम रहनुपर्छ।

### C. Business Rules

व्यवसाय वा सेवाको नियम बताउँछन्।

उदाहरण:
- निवेदन बुझाउनुअघि आवश्यक कागजात संलग्न हुनुपर्छ।
- वडा कर्मचारीले आफ्नो अधिकारक्षेत्रका निवेदन मात्र हेर्न पाउनुपर्छ।
- स्वीकृत निवेदनको status परिवर्तन गर्न विशेष अनुमति चाहिन सक्छ।

Business Rule लाई अनुमान गरेर लागू गर्नु हुँदैन। सम्बन्धित अधिकृत वा Product Owner बाट नियम पुष्टि गर्नुपर्छ।

## ५.४ Requirement Analysis मा गरिने काम

1. Requirement document, User Story, wireframe, API document र acceptance criteria पढ्ने।
2. Stakeholder सँग छलफल गरेर अस्पष्ट कुरा स्पष्ट गर्ने।
3. प्रत्येक requirement testable छ कि छैन जाँच्ने।
4. सकारात्मक (positive), नकारात्मक (negative) र boundary अवस्थाबारे सोच्ने।
5. भूमिका/अनुमति, डेटा, error handling र integration निर्भरता पहिचान गर्ने।
6. Functional तथा Non-functional testing आवश्यकताहरू सूची बनाउने।
7. जोखिमका आधारमा बढी ध्यान दिनुपर्ने क्षेत्र पहिचान गर्ने।
8. Testable requirement र सम्भावित test approach को प्रारम्भिक mapping बनाउने।
9. आवश्यकता परिवर्तन भएमा version/change tracking राख्ने।

## ५.५ Requirement राम्रो छ कि छैन कसरी जाँच्ने?

एउटा राम्रो requirement सामान्यतया:

- **Clear:** अर्थ स्पष्ट छ।
- **Complete:** आवश्यक विवरण पर्याप्त छ।
- **Consistent:** अन्य आवश्यकता वा नियमसँग बाझिएको छैन।
- **Testable:** पास/फेल निर्धारण गर्ने आधार छ।
- **Traceable:** ID वा अन्य तरिकाले पछ्याउन सकिन्छ।
- **Feasible:** प्राविधिक र व्यावसायिक हिसाबले सम्भव छ।
- **Unambiguous:** फरक व्यक्तिले फरक अर्थ नलगाउने गरी लेखिएको छ।

### खराब र राम्रो Requirement को उदाहरण

**खराब:** “वेबसाइट छिटो हुनुपर्छ।”

समस्या: “छिटो” को मापन छैन।

**राम्रो:** “स्वीकृत परीक्षण वातावरणमा निर्धारित load र network profile अन्तर्गत, निर्दिष्ट पेजका 95% अनुरोध 2.5 सेकेन्डभित्र पूरा हुनुपर्छ।”

यहाँ समय, वातावरण र percentile उल्लेख छन्। वास्तविक target सम्बन्धित stakeholder ले तय गर्नुपर्छ।

**खराब:** “फाइल अपलोड हुनुपर्छ।”

**राम्रो:** “प्रणालीले स्वीकृत file type र 5 MB सम्मका फाइल स्वीकार गर्नुपर्छ; 5 MB भन्दा ठूलो वा अस्वीकृत प्रकारको फाइलमा upload अस्वीकार गरी स्पष्ट सन्देश देखाउनुपर्छ।”

यहाँ 5 MB केवल उदाहरणका लागि राखिएको हो; वास्तविक सीमा परियोजनाले तय गर्नुपर्छ।

## ५.६ Requirement बाट Testability निकाल्ने उदाहरण

Requirement: “सही विवरण राखेमा प्रयोगकर्ता लगइन हुनुपर्छ।”

QA का प्रश्न:
- “सही विवरण” भन्नाले कुन login identifier र password?
- प्रयोगकर्ता निष्क्रिय छ भने के हुन्छ?
- लगातार गलत password राख्दा account lock हुन्छ?
- error message ले खाता अस्तित्वमा छ कि छैन भन्ने खुलाउँछ?
- Session कति समय सक्रिय रहन्छ?
- Login सफल भएपछि कुन पेजमा जाने?
- MFA/OTP लागू छ कि छैन?
- धेरै अनुरोध हुँदा rate limit छ?
- Password field मा paste र password manager अनुमति छ?

यी सबै प्रश्नको उत्तर हरेक परियोजनामा एउटै हुँदैन। लागू हुने प्रश्नहरू stakeholder सँग पुष्टि गर्नुपर्छ।

## ५.७ Requirement Analysis का Deliverables

- Requirement clarification questions
- Requirement review notes
- Testable requirement list
- प्रारम्भिक Requirement Traceability Matrix (RTM)
- प्रारम्भिक risk list
- Testing scope को प्रारम्भिक रूप
- आवश्यक test data, environment र dependency को सूची

## ५.८ Entry Criteria र Exit Criteria

**Entry Criteria** भनेको चरण सुरु गर्न आवश्यक अवस्था हो। Requirement Analysis सुरु गर्न प्रारम्भिक requirement, user story वा business objective उपलब्ध हुन सक्छ।

**Exit Criteria** भनेको अर्को चरणमा जान पर्याप्त तयारी भएको अवस्था हो। उदाहरण:
- महत्वपूर्ण अस्पष्टता समाधान भएको।
- आवश्यकताहरूको परीक्षणयोग्यता जाँचिएको।
- मुख्य जोखिम र dependency अभिलेख गरिएको।
- खुला प्रश्नको जिम्मेवार व्यक्ति र निर्णय मिति तोकिएको।
- Test Planning का लागि पर्याप्त जानकारी उपलब्ध भएको।

हरेक प्रश्न पूर्ण समाधान नहुँदै चरण रोकिनैपर्छ भन्ने छैन; तर बाँकी प्रश्नको जोखिम र जिम्मेवारी स्पष्ट हुनुपर्छ।

## ५.९ सामान्य गल्ती

- Requirement नबुझी सीधै test case लेख्नु।
- केवल happy path हेर्नु।
- Error, permission, boundary र security व्यवहार छुटाउनु।
- अस्पष्ट शब्द (“छिटो”, “सुरक्षित”, “सजिलो”) लाई मापनयोग्य नबनाउनु।
- Requirement परिवर्तनको version नहेर्नु।
- UI देखिएको आधारमा backend नियम अनुमान गर्नु।
- “Tester ले सबै कुरा आफैँ अनुमान गरोस्” भन्ने सोच राख्नु।

## ५.१० अभ्यास

Requirement: “नागरिकले निवेदन बुझाउन पाउनुपर्छ।”

कम्तीमा यी प्रश्न तयार गर्नुहोस्:
1. कुन विवरण अनिवार्य छन्?
2. कुन फाइल प्रकार र आकार स्वीकार हुन्छ?
3. दोहोर्‍याएर Submit गर्दा के हुन्छ?
4. Login नभएको व्यक्तिले submit गर्न सक्छ?
5. Submit सफल भएपछि कुन confirmation देखिन्छ?
6. Network बीचमै काटिएमा स्थिति कसरी थाहा हुन्छ?
7. निवेदनको status कसले परिवर्तन गर्न सक्छ?

---

# ६. चरण २ — Test Planning

## ६.१ परिचय

Test Planning मा परीक्षणको लक्ष्य, scope, strategy, स्रोत, समयतालिका, जिम्मेवारी, उपकरण, जोखिम र पास/फेलका आधारहरू निर्धारण गरिन्छ। यसले “कसले, के, कसरी, कहिले र कुन स्रोतबाट परीक्षण गर्ने?” भन्ने प्रश्नको उत्तर दिन्छ।

## ६.२ Test Plan का मुख्य उद्देश्य

- परीक्षणको सीमा (Scope) स्पष्ट बनाउने।
- परीक्षणको प्राथमिकता र विधि निर्धारण गर्ने।
- आवश्यक जनशक्ति, समय, वातावरण र tool अनुमान गर्ने।
- जोखिम तथा निर्भरता पहिचान गर्ने।
- Entry/Exit Criteria र defect workflow तय गर्ने।
- Stakeholder लाई साझा अपेक्षा र परीक्षणको रणनीति बुझाउने।

## ६.३ Test Plan मा समेटिने विषय

### 1. Test Objectives
परीक्षणबाट के प्रमाण वा जानकारी चाहिएको हो?

उदाहरण:
- Login र access control को मुख्य व्यवहार जाँच्ने।
- निवेदन बुझाउने र फाइल अपलोड गर्ने सुविधा स्वीकृत requirement अनुसार काम गर्छ कि गर्दैन जाँच्ने।
- Release अघि खुला उच्च जोखिमको defect पहिचान गर्ने।

### 2. Scope — In Scope र Out of Scope

**In Scope (परीक्षणमा समावेश):**
- Login/logout
- सेवा निवेदन फाराम
- अनिवार्य field validation
- File upload validation
- Role-based access
- Application/API integration

**Out of Scope (यस चक्रमा समावेश छैन):**
- बाह्य भुक्तानी सेवा, यदि test environment वा अनुमति उपलब्ध छैन भने
- छुट्टै स्वीकृत नभएको legacy module
- Production मा अनुमति नलिई destructive testing

Out of Scope राख्नु भनेको जोखिम छैन भन्नु होइन। कारण, प्रभाव र कसले स्वीकृति दिएको हो भन्ने कुरा अभिलेख गर्नुपर्छ।

### 3. Test Strategy / Test Approach

कुन स्तर र प्रकारका परीक्षण गरिन्छन्?

- Unit Testing: सानो function/component को परीक्षण; सामान्यतः developer ले गर्छ।
- Integration Testing: API, database वा service बीचको सम्बन्ध।
- System Testing: सम्पूर्ण प्रणालीको व्यवहार।
- End-to-End (E2E): प्रयोगकर्ताको पूरा workflow।
- Smoke Testing: build को मुख्य सुविधा चल्ने/नचल्ने प्रारम्भिक जाँच।
- Sanity Testing: सीमित परिवर्तन वा fix को लक्षित जाँच।
- Regression Testing: परिवर्तनले पुरानो सुविधा बिगारेको छ कि छैन।
- UAT: business/user ले स्वीकृत आवश्यकता अनुसार प्रयोगयोग्यता/स्वीकार्यता जाँच्ने।
- Performance, Security, Accessibility, Compatibility Testing: आवश्यकताअनुसार।

### 4. Test Resources
- Test Lead / QA Engineer
- Developer र Business Analyst को सहयोग
- Test server, database र test accounts
- Browser/device
- Test management र defect tracking tools
- Automation framework वा performance/security tools, आवश्यक भएमा

### 5. Schedule
कुन काम कहिले सुरु/समाप्त हुन्छ? अनुमानको आधार र निर्भरता पनि उल्लेख गर्नुपर्छ।

### 6. Risks and Mitigation
उदाहरण:
- Test environment ढिलो तयार हुने → वातावरण तयार गर्ने जिम्मेवार व्यक्ति र वैकल्पिक योजना तय गर्ने।
- Test data उपलब्ध नहुने → synthetic/masked data पहिले तयार गर्ने।
- Requirement बारम्बार बदलिने → change review र regression scope पुनःमूल्याङ्कन गर्ने।
- Automation unstable हुने → flaky test छुट्याउने, manual fallback राख्ने।

### 7. Entry Criteria
उदाहरण:
- Requirement र acceptance criteria review भएको।
- आवश्यक build उपलब्ध भएको (execution सुरु गर्नुअघि)।
- Test environment र test account तयार भएको।
- Test data तयार भएको।

### 8. Exit Criteria
Exit Criteria परियोजनाअनुसार तय हुन्छ। उदाहरण:
- उच्च जोखिमका आवश्यकतामा परीक्षण पूरा भएको।
- Release का लागि निर्धारित test cases को लक्ष्य coverage पूरा भएको।
- कुनै खुला Critical defect नरहेको।
- बाँकी High defect लाई स्वीकृत जोखिम, workaround र owner सहित निर्णय गरिएको।
- आवश्यक smoke/regression परीक्षण सफल भएको।
- Test Summary Report तयार भएको।

**महत्त्वपूर्ण:** “100% test case pass” मात्रै पर्याप्त release criterion होइन। परीक्षण coverage, defect को गम्भीरता, बाँकी जोखिम, performance/security आवश्यकताहरू र business approval पनि विचार गर्नुपर्छ।

### 9. Defect Management Process
Bug कहाँ log गर्ने, severity/priority कसरी तय गर्ने, कसले triage गर्ने, retest कसले गर्ने र defect पुनःखुलेमा के गर्ने भन्ने नियम।

### 10. Deliverables
Test Plan, Test Schedule, Test Data Plan, Risk Register, Environment Needs, Reporting Plan आदि।

## ६.४ Test Plan को नमुना

**Project:** नगरपालिका अनलाइन सेवा पोर्टल  
**Version:** 1.0  
**Objective:** Login, सेवा निवेदन र फाइल अपलोडको मुख्य व्यवहार तथा जोखिम जाँच्ने।

**Scope:** Login, logout, निवेदन फाराम, आवश्यक field validation, file upload, role-based access।

**Approach:** Requirement review, manual functional testing, API integration testing, चयनित browser testing, आवश्यक regression testing। Automation सम्भव र उपयोगी भएका स्थिर workflow मा मात्र प्रयोग गर्ने।

**Environment:** QA server, test database, test user roles, स्वीकृत browser/device संयोजन।

**Risks:** Requirement परिवर्तन, test data को कमी, third-party सेवा उपलब्धता, कमजोर नेटवर्क।

**Entry Criteria:** स्वीकृत acceptance criteria, उपलब्ध build, तयार test account/data।

**Exit Criteria:** Critical workflow परीक्षण सम्पन्न; critical defect खुला नरहेको; बाँकी जोखिम दस्तावेजीकृत र सम्बन्धित अधिकारप्राप्त व्यक्तिबाट निर्णय भएको; आवश्यक रिपोर्ट उपलब्ध।

**Approval:** QA Lead / Product Owner / सम्बन्धित जिम्मेवार व्यक्ति (परियोजनाको शासन प्रणालीअनुसार)।

## ६.५ Test Estimation

समय अनुमान गर्दा निम्न काम समेट्नुपर्छ:
- Requirement analysis
- Test design र review
- Test data/environment setup
- Execution
- Defect logging र triage
- Retesting
- Regression
- Reporting र closure

उदाहरणका लागि 40 test cases छन् भन्दैमा 40 × 5 मिनेट मात्र हिसाब गर्नु सही नहुन सक्छ। केही case सरल हुन्छन्, केहीमा data setup, role change, file upload, API verification वा evidence संकलन आवश्यक हुन्छ। अनुमान ऐतिहासिक डेटा, complexity, जोखिम र team capacity अनुसार गर्नुपर्छ।

## ६.६ Test Planning मा प्राथमिकता

- **Risk:** असफल भएमा प्रभाव कति ठूलो?
- **Likelihood:** असफल हुने सम्भावना कति?
- **Usage:** सुविधा कति प्रयोग हुन्छ?
- **Change impact:** हालै कति परिवर्तन भएको?
- **Dependency:** बाह्य सेवा वा जटिल integration छ?
- **Regulatory/business impact:** कानुनी वा सेवा प्रवाहमा असर पर्छ?

## ६.७ सामान्य गल्ती

- Test Plan लाई केवल औपचारिक कागजात मान्नु।
- समय/स्रोतको अवास्तविक अनुमान।
- Non-functional testing पूर्ण रूपमा बिर्सनु।
- Out of Scope को जोखिम नबताउनु।
- स्पष्ट Entry/Exit Criteria नराख्नु।
- Defect triage र stakeholder approval को प्रक्रिया नतोक्नु।
- सबै सुविधालाई समान प्राथमिकता दिनु।

---

# ७. चरण ३ — Test Case Design / Test Design

## ७.१ परिचय

Test Design चरणमा आवश्यकता र Test Plan का आधारमा परीक्षणका परिदृश्य (Test Scenarios), विस्तृत Test Cases, Test Data र Expected Results तयार गरिन्छ। आवश्यकता र परीक्षणबीच traceability कायम राखिन्छ।

**Test Scenario** ले के जाँच्ने भन्ने उच्चस्तरीय उद्देश्य बताउँछ।  
**Test Case** ले कसरी जाँच्ने, कुन input प्रयोग गर्ने र कस्तो नतिजा अपेक्षा गर्ने भन्ने स्पष्ट गर्छ।

### उदाहरण

- Test Scenario: Login को validation जाँच्ने।
- Test Case: सही इमेल र सही पासवर्ड राखेर Login थिच्दा प्रयोगकर्ता Dashboard मा पुग्छ कि पुग्दैन जाँच्ने।

## ७.२ राम्रो Test Case का विशेषता

- स्पष्ट र बुझ्न सजिलो।
- एउटै उद्देश्य केन्द्रित।
- आवश्यक पूर्वसर्त (Preconditions) स्पष्ट।
- दोहोर्‍याएर चलाउँदा समान नतिजा दिन सक्ने (जहाँ लागू हुन्छ)।
- Input/Test Data र Expected Result स्पष्ट।
- Requirement ID सँग जोडिएको।
- वास्तविक र परीक्षणयोग्य।
- आवश्यकता अनुसार Priority र Test Type उल्लेख भएको।
- नतिजा प्रमाणित गर्न सकिने।

## ७.३ Test Case का सामान्य Field

| Field | अर्थ |
|---|---|
| Test Case ID | अद्वितीय पहिचान, जस्तै TC-LOGIN-001 |
| Requirement ID | सम्बन्धित requirement, जस्तै REQ-LOGIN-01 |
| Title | के परीक्षण गर्ने |
| Preconditions | परीक्षणअघि आवश्यक अवस्था |
| Test Data | प्रयोग हुने input |
| Steps | चरणबद्ध निर्देशन |
| Expected Result | अपेक्षित व्यवहार |
| Actual Result | चलाउँदा भेटिएको वास्तविक व्यवहार |
| Status | Not Run / Pass / Fail / Blocked आदि |
| Priority | परीक्षणको प्राथमिकता |
| Type | Functional, Security, Regression आदि |
| Evidence | Screenshot, log, request/response, recording आदि |
| Tester / Date / Build | कसले, कहिले, कुन build मा परीक्षण गर्‍यो |

## ७.४ नमुना Test Cases — Login

### TC-LOGIN-001: सही विवरणबाट Login

- Requirement: REQ-LOGIN-01
- Preconditions: सक्रिय test account उपलब्ध।
- Test Data: मान्य इमेल र सही password।
- Steps:
  1. Login पेज खोल्ने।
  2. मान्य इमेल राख्ने।
  3. सही password राख्ने।
  4. Login थिच्ने।
- Expected Result: Login सफल हुन्छ र स्वीकृत landing page खुल्छ; अनधिकृत वा संवेदनशील डेटा देखिँदैन।
- Priority: High
- Type: Functional / Positive

### TC-LOGIN-002: गलत Password

- Preconditions: सक्रिय test account उपलब्ध।
- Test Data: मान्य इमेल, गलत password।
- Steps: Login पेज खोल्ने, विवरण राख्ने र Login थिच्ने।
- Expected Result: Login अस्वीकार हुन्छ; उपयुक्त त्रुटि सन्देश देखिन्छ; authenticated session सिर्जना हुँदैन।
- Type: Negative / Security

### TC-LOGIN-003: खाली अनिवार्य Field

- Test Data: इमेल र password खाली।
- Expected Result: Login सफल हुँदैन; आवश्यक field validation देखिन्छ; अनावश्यक server error हुँदैन।
- नोट: Validation client र server दुवै तहमा आवश्यक हुन सक्छ; केवल browser-side validation मा भर पर्नु हुँदैन।

### TC-LOGIN-004: निष्क्रिय Account

- Preconditions: परीक्षणका लागि निष्क्रिय account तयार।
- Expected Result: नीति अनुसार access अस्वीकार हुन्छ। सन्देशले account enumeration जोखिम बढाउँछ कि बढाउँदैन भनेर पनि मूल्याङ्कन गर्ने।

### TC-LOGIN-005: Role-based Access

- Preconditions: सामान्य नागरिक र Admin test accounts।
- Steps: नागरिक account बाट admin route/API खोल्ने प्रयास।
- Expected Result: अनुमति नभएको पहुँच server/API तहमा समेत अस्वीकार हुन्छ। UI मा link लुकाउनु मात्रै पर्याप्त सुरक्षा होइन।

## ७.५ Positive, Negative र Boundary Testing

### Positive Testing
वैध input र सामान्य प्रयोगको अवस्था जाँच्ने।

उदाहरण: मान्य विवरणसहित निवेदन submit गर्नु।

### Negative Testing
अवैध input वा अस्वीकृत व्यवहार जाँच्ने।

उदाहरण: आवश्यक विवरण नभरि submit गर्नु, अनुमति नभएको file type upload गर्नु।

### Boundary Value Testing
सीमाको नजिकका मान जाँच्ने।

यदि फाइलको स्वीकृत अधिकतम आकार 5 MB छ भने (वास्तविक नीति यही भएमा):
- सीमा भन्दा सानो फाइल
- ठीक सीमा बराबर फाइल
- सीमा भन्दा अलिकति ठूलो फाइल

सीमामा “5 MB” को अर्थ 5,000,000 bytes हो कि 5 MiB (5 × 1,048,576 bytes) हो भन्ने स्पष्ट हुनुपर्छ।

### Equivalence Partitioning
समान व्यवहार हुने input लाई समूहमा विभाजन गरेर प्रत्येक समूहबाट प्रतिनिधि मान जाँच्ने।

उदाहरण: फाइल प्रकार
- स्वीकृत PDF
- स्वीकृत image
- अस्वीकृत executable
- अज्ञात/गलत extension

### Decision Table Testing
धेरै सर्त मिलेर परिणाम तय हुँदा प्रयोग गरिन्छ।

उदाहरण: निवेदन Submit गर्न Login भएको हुनुपर्छ, अनिवार्य field भरिएको हुनुपर्छ र आवश्यक कागजात संलग्न हुनुपर्छ।

| Login छ? | विवरण पूरा? | कागजात पूरा? | अपेक्षित नतिजा |
|---|---|---|---|
| हो | हो | हो | Submit स्वीकार |
| होइन | हो | हो | Login माग्ने/अस्वीकार |
| हो | होइन | हो | Validation देखाउने |
| हो | हो | होइन | कागजात माग्ने/अस्वीकार |
| होइन | होइन | होइन | स्वीकृत नीति अनुसार रोक्ने र आवश्यक सन्देश दिने |

### State Transition Testing
प्रणालीको अवस्था परिवर्तन परीक्षण गर्ने।

उदाहरण:
Draft → Submitted → Under Review → Approved/Rejected

जाँच्नुपर्ने कुरा:
- कुन भूमिकाले कुन transition गर्न सक्छ?
- Approved भएपछि Draft मा फर्काउन मिल्छ?
- Reject गर्दा कारण अनिवार्य छ?
- दोहोर्‍याएर Approve गर्दा duplicate action हुन्छ?
- गलत transition API बाट प्रयास गर्दा रोकिन्छ?

### Use Case / End-to-End Testing
प्रयोगकर्ताको वास्तविक काम सुरुदेखि अन्त्यसम्म जाँच्ने।

उदाहरण:
Login → सेवा छनोट → फाराम भर्ने → कागजात अपलोड → Submit → Confirmation → Status हेर्ने।

## ७.६ Test Data Design

Test Data मा सामान्यतया:
- Valid data
- Invalid data
- Missing data
- Boundary data
- Duplicate data
- Different user roles
- Different language/Unicode data
- Large/small files
- Special characters
- Date/time/time-zone cases
- Privacy-sensitive data को masked वा synthetic रूप

वास्तविक नागरिकको संवेदनशील व्यक्तिगत विवरणलाई अनावश्यक रूपमा QA वातावरणमा प्रयोग नगर्नुहोस्। आवश्यक परे अनुमति, masking र access control अपनाउनुहोस्।

## ७.७ Test Case Review

Test Case review गर्दा:
- Requirement coverage छ?
- Expected Result मापनयोग्य छ?
- Steps अस्पष्ट छन्?
- Duplicate case छन्?
- Negative र boundary case छन्?
- Role/access control छ?
- Data setup र cleanup चाहिन्छ?
- Test case स्वचालित गर्न उपयुक्त छ?
- Evidence र pass/fail निर्णय स्पष्ट छन्?

## ७.८ Test Design का Deliverables

- Test Scenarios
- Test Cases / Checklist
- Test Data
- RTM अद्यावधिक
- Automation candidates (आवश्यक भए)
- Test Case Review Comments

## ७.९ सामान्य गल्ती

- केवल positive case लेख्नु।
- “Expected Result: काम गर्छ” जस्तो अस्पष्ट वाक्य लेख्नु।
- सबै test case लाई High priority दिनु।
- Requirement ID नराख्नु।
- एउटै case मा धेरै असम्बन्धित कुरा जाँच्नु।
- स्थिर test data नबनाउनु वा test पछि data cleanup नसोच्नु।
- UI test मा मात्र निर्भर भएर API/server-side validation नजाँच्नु।

---

# ८. चरण ४ — Test Environment Setup

## ८.१ परिचय

Test Environment भनेको परीक्षण चलाइने hardware/software/configuration को संयोजन हो। यसमा application build, backend service, database, network, browser/device, user role, test data र आवश्यक third-party integration पर्न सक्छन्।

केही STLC मोडेलमा यो अलग चरण हुन्छ; केहीमा Test Planning वा Execution भित्र राखिन्छ। व्यावहारिक रूपमा environment readiness स्पष्ट रूपमा जाँच्नु महत्त्वपूर्ण हुन्छ।

## ८.२ Environment का उदाहरण

- Local development
- QA / Test
- Staging / Pre-production
- Production

यी वातावरणको configuration, data र अनुमति फरक हुन सक्छ। Production मा परीक्षण गर्दा विशेष स्वीकृति, non-destructive approach र निगरानी आवश्यक हुन्छ।

## ८.३ Setup Checklist

- [ ] सही build/version deploy भएको छ।
- [ ] Frontend र backend बीच connection ठीक छ।
- [ ] Database उपलब्ध छ र आवश्यक schema/migration लागू भएको छ।
- [ ] Test accounts र roles तयार छन्।
- [ ] Test data सही र पुनःप्रयोगयोग्य छ।
- [ ] Email/SMS/payment जस्ता external integration sandbox वा mock मा छन्।
- [ ] Browser/device matrix निश्चित छ।
- [ ] आवश्यक logs र monitoring उपलब्ध छन्।
- [ ] Test environment मा production secret वा अनावश्यक वास्तविक व्यक्तिगत डेटा छैन।
- [ ] आवश्यक tool/version र access permission तयार छन्।
- [ ] Time zone, locale र language settings परीक्षणका लागि उपयुक्त छन्।
- [ ] फाइल अपलोड/storage र permission configuration सही छ।

## ८.४ Smoke Testing

Environment वा नयाँ build तयार भएपछि मुख्य सुविधा चल्छ कि चल्दैन भन्ने छोटो जाँचलाई Smoke Testing भनिन्छ।

उदाहरण:
1. Home page खुल्छ?
2. Login पेज खुल्छ?
3. Test account login हुन्छ?
4. मुख्य API ले response दिन्छ?
5. सेवा सूची खुल्छ?
6. Test निवेदन submit गर्न सकिन्छ?
7. Error log मा तुरुन्तै देखिने critical failure छ?

Smoke test असफल भएमा विस्तृत execution सुरु गर्नु अघि build/environment समस्या समाधान गर्नु राम्रो हुन्छ।

## ८.५ Environment Issue र Product Bug छुट्याउने

उदाहरण: Login test गर्दा server नै बन्द छ भने त्यसलाई तुरुन्तै “Login feature fail” भनेर निष्कर्ष निकाल्नु ठीक नहुन सक्छ। पहिले:
- Server reachable छ?
- API health ठीक छ?
- सही build छ?
- Test account सक्रिय छ?
- Configuration र network ठीक छन्?

Environment समस्या पुष्टि भएमा case लाई Blocked राख्न वा environment issue छुट्टै log गर्न सकिन्छ। तर वास्तविक product defect लाई environment समस्या भनेर ढाक्नु हुँदैन।

## ८.६ Deliverables

- Environment configuration विवरण
- Environment readiness checklist
- Build/version विवरण
- Smoke test result
- Known environment limitations
- Access र test data readiness record

---

# ९. चरण ५ — Test Execution

## ९.१ परिचय

Test Execution मा डिजाइन गरिएका test cases लाई उपयुक्त build र वातावरणमा चलाएर वास्तविक नतिजा (Actual Result) र अपेक्षित नतिजा (Expected Result) तुलना गरिन्छ। प्रमाण सुरक्षित राखिन्छ, failure को कारण छानबिन गरिन्छ र आवश्यक परे defect report तयार गरिन्छ।

## ९.२ Execution अघि जाँच

- सही build/version हो?
- Test environment उपलब्ध छ?
- आवश्यक test data तयार छ?
- Test case र expected result review भएको छ?
- हालको scope/priority स्पष्ट छ?
- Defect tracking प्रणाली उपलब्ध छ?
- Evidence राख्ने तरिका तय छ?

## ९.३ Test Case को सामान्य Status

- **Not Run:** अझै चलाइएको छैन।
- **Pass:** वास्तविक नतिजा अपेक्षित नतिजासँग मेल खान्छ।
- **Fail:** वास्तविक नतिजा अपेक्षित नतिजासँग मेल खाँदैन र परीक्षण valid छ।
- **Blocked:** आवश्यक निर्भरता/वातावरण/डेटा उपलब्ध नभएकाले परीक्षण गर्न सकिएन।
- **Not Applicable (N/A):** स्वीकृत कारणले सो build/scope मा लागू हुँदैन।
- **In Progress:** परीक्षण चलिरहेको छ (tool वा team workflow ले प्रयोग गरेमा)।

Status को परिभाषा team ले साझा रूपमा तय गर्नुपर्छ। Blocked लाई Pass वा Fail मा जबर्जस्ती बदल्नु हुँदैन।

## ९.४ Execution प्रक्रिया

1. सही build र environment पुष्टि गर्ने।
2. Test Case ID अनुसार परीक्षण चलाउने।
3. Actual Result लेख्ने।
4. Expected र Actual तुलना गर्ने।
5. Pass/Fail/Blocked status दिने।
6. Failure हुँदा reproducible steps, test data र evidence सुरक्षित गर्ने।
7. Defect tracking tool मा defect log गर्ने।
8. Defect triage र fix को स्थिति पछ्याउने।
9. Fix आएको build मा retest गर्ने।
10. प्रभावित सुविधामा regression test गर्ने।
11. परिणाम, coverage र बाँकी जोखिम रिपोर्ट गर्ने।

## ९.५ Defect Report मा के लेख्ने?

- Defect ID
- संक्षिप्त Title
- Environment / Build / Version
- Preconditions
- Reproduction Steps
- Expected Result
- Actual Result
- Severity / Priority
- Reproducibility
- Screenshot / video / logs / API evidence
- सम्बन्धित Requirement ID / Test Case ID
- Reporter, Assignee र timestamps
- Status र fix version

### नमुना Defect

**ID:** BUG-LOGIN-014  
**Title:** गलत password राख्दा Login सफल भएको देखिन्छ  
**Environment:** QA, Build 1.2.0  
**Precondition:** सक्रिय test account उपलब्ध  
**Steps:**
1. Login पेज खोल्ने।
2. मान्य इमेल र गलत password राख्ने।
3. Login थिच्ने।

**Expected:** Login अस्वीकार हुनुपर्छ र authenticated session बन्नु हुँदैन।  
**Actual:** Dashboard खुल्छ र authenticated session देखिन्छ।  
**Severity:** Critical (यदि गलत password बाट अनधिकृत प्रवेश वास्तवमै प्रमाणित भएको हो भने)  
**Priority:** तत्काल समाधानका लागि उच्च।  
**Evidence:** संवेदनशील token/password नदेखिने गरी screenshot/log संलग्न।  
**Requirement:** REQ-LOGIN-02

यो केवल उदाहरण हो; वास्तविक severity प्रभाव, reproducibility र पुष्टि भएको प्रमाणका आधारमा तय हुन्छ।

## ९.६ Retesting र Regression Testing को फरक

**Retesting:** खास defect fix भएको छ कि छैन भनेर सोही failure फेरि जाँच्ने।

उदाहरण: गलत password बाट login भएको bug fix गरेपछि सोही steps पुनः चलाउने।

**Regression Testing:** परिवर्तनले अरू पुराना सुविधा बिगारेको छ कि छैन जाँच्ने।

उदाहरण: Login code परिवर्तनपछि सही login, logout, password reset, session timeout र role-based access जाँच्ने।

Retest पास भयो भन्दैमा सम्पूर्ण प्रणालीमा regression risk छैन भन्ने हुँदैन।

## ९.७ Smoke, Sanity, Retest, Regression — तुलना

| प्रकार | उद्देश्य | सामान्य समय |
|---|---|---|
| Smoke | Build का मुख्य सुविधा चल्ने/नचल्ने जाँच | नयाँ build पछि |
| Sanity | सीमित परिवर्तन वा fix को लक्षित जाँच | सानो परिवर्तनपछि |
| Retest | पहिले fail भएको defect fix पुष्टि | Fix build आएपछि |
| Regression | परिवर्तनले अन्य सुविधा नबिगारेको पुष्टि | Code/config change पछि, जोखिमअनुसार |

## ९.८ Test Execution Report को नमुना

| Test Case | Expected | Actual | Status | टिप्पणी |
|---|---|---|---|---|
| TC-LOGIN-001 | सही विवरणबाट login सफल | Dashboard खुल्यो | Pass | Build 1.2.0 |
| TC-LOGIN-002 | गलत password अस्वीकार | Login अस्वीकार | Pass | Error message जाँचियो |
| TC-LOGIN-003 | खाली field मा validation | Validation देखियो | Pass | Client/server behavior जाँच आवश्यकताअनुसार |
| TC-UPLOAD-004 | निषेधित file type अस्वीकार | `.exe` स्वीकार भयो | Fail | BUG-UPLOAD-007 |
| TC-ROLE-002 | नागरिकले Admin API खोल्न नपाउने | 403 Forbidden | Pass | API response प्रमाण सुरक्षित |

यो तालिका सिकाइका लागि काल्पनिक नमुना हो, वास्तविक test result होइन।

## ९.९ Execution का क्रममा ध्यान दिनुपर्ने कुरा

- सही build र test data उल्लेख गर्नुहोस्।
- Failure पुनःउत्पादन गर्न मिल्ने विवरण राख्नुहोस्।
- Screenshot मात्र होइन, आवश्यक परे network/API/server logs पनि हेर्नुहोस्।
- संवेदनशील token, password वा व्यक्तिगत विवरण evidence मा नराख्नुहोस्।
- अनिश्चित नतिजालाई Pass नदिनुहोस्।
- Environment issue र product defect छुट्याउनुहोस्।
- Bug fix पछि retest र आवश्यक regression दुवै सोच्नुहोस्।
- Defect triage मा severity, priority, impact र release risk साझा रूपमा मूल्याङ्कन गर्नुहोस्।

---

# १०. चरण ६ — Test Closure

## १०.१ परिचय

Test Closure भनेको परीक्षण चक्रको अन्त्यमा सम्पन्न काम, test coverage, defect स्थिति, बाँकी जोखिम, सिकाइ र release सम्बन्धी जानकारी समेटेर औपचारिक सारांश तयार गर्ने चरण हो।

Closure को अर्थ “सबै bug हटिसके” भन्ने होइन। परीक्षण रोकिएको कारण, के परीक्षण भयो, के हुन सकेन र कुन जोखिम बाँकी छ भन्ने कुरा पारदर्शी रूपमा देखाउनु यसको उद्देश्य हो।

## १०.२ मुख्य उद्देश्य

- परीक्षणको वास्तविक स्थिति सारांश बनाउने।
- Test Plan/Exit Criteria पूरा भए/नभएको मूल्याङ्कन गर्ने।
- Defect र बाँकी जोखिम अभिलेख गर्ने।
- आवश्यक stakeholder लाई release निर्णयका लागि जानकारी दिने।
- Test artifacts र evidence सुरक्षित राख्ने।
- सिकाइ संकलन गरेर अर्को चक्र सुधार्ने।

## १०.३ Test Closure का गतिविधि

1. Test execution को स्थिति अन्तिम रूप दिने।
2. Requirement र test coverage जाँच्ने।
3. Pass, Fail, Blocked र Not Run case को संख्या/प्रतिशत निकाल्ने।
4. Defect हरूको severity, priority र status अनुसार सारांश बनाउने।
5. खुला defect को प्रभाव, workaround र owner लेख्ने।
6. Exit Criteria पूरा भएको/नभएको समीक्षा गर्ने।
7. Test Summary / Closure Report तयार गर्ने।
8. आवश्यक approval वा sign-off लिने।
9. Test cases, scripts, test data instructions र evidence version-control/repository मा राख्ने।
10. Lessons Learned / Retrospective गर्ने।
11. अर्को release वा Sprint का लागि सुधार कार्य तोक्ने।

## १०.४ Test Closure Report को नमुना

**Project:** नगरपालिका अनलाइन सेवा पोर्टल  
**Build:** 1.2.0  
**Test Period:** 2026-10-01 देखि 2026-10-10 (काल्पनिक उदाहरण)  
**Scope:** Login, निवेदन फाराम, file upload र role access

### सारांश
- कुल test cases: 100
- Pass: 82
- Fail: 8
- Blocked: 5
- Not Run: 5

**Execution coverage** (Pass + Fail + Blocked भएका case सहित executed/attempted परिभाषा team ले स्पष्ट गर्नुपर्छ) अलग रूपमा रिपोर्ट गर्नुपर्छ। यहाँ यदि “चलाइएका” भन्नाले Pass + Fail मात्र लिइयो भने 90/100 = 90% हुन्छ। Blocked लाई executed मा समेट्ने वा नसमेट्ने नीति रिपोर्टमा स्पष्ट लेख्नुपर्छ।

**Pass rate:** Pass ÷ (Pass + Fail) × 100  
= 82 ÷ (82 + 8) × 100  
≈ 91.1%

यो pass rate ले Blocked/Not Run अवस्थाको जोखिम आफैँ समेट्दैन। त्यसैले प्रतिशतसँगै counts र coverage पनि देखाउनुपर्छ।

### Defect सारांश
- Critical: 0
- High: 2
- Medium: 5
- Low: 3

यी संख्या केवल उदाहरण हुन्। Release recommendation गर्न खुला defect को वास्तविक विवरण, प्रभाव र स्वीकृति आवश्यक हुन्छ।

### बाँकी जोखिम
- केही browser/device संयोजनमा परीक्षण बाँकी।
- बाह्य SMS सेवा QA environment मा उपलब्ध नभएकाले पूर्ण integration प्रमाणित नभएको।
- दुई High defect workaround सहित खुला छन्; निर्णय अधिकारप्राप्त stakeholder बाट आवश्यक।

### Recommendation
उपलब्ध प्रमाण, exit criteria र बाँकी जोखिमका आधारमा Release / Conditional Release / No-Go मध्ये सिफारिस लेख्ने। QA ले गुणस्तरसम्बन्धी प्रमाण दिन्छ; अन्तिम release निर्णय परियोजनाको अधिकारप्राप्त निर्णयकर्ताले गर्छ।

## १०.५ Sign-off भनेको के हो?

Sign-off भनेको निर्धारित परीक्षण कार्य र रिपोर्ट समीक्षा गरिएको तथा नतिजा/बाँकी जोखिम स्वीकार वा निर्णय गरिएको औपचारिक अभिलेख हो। Sign-off ले “सफ्टवेयरमा कुनै bug छैन” भन्ने ग्यारेन्टी दिँदैन।

## १०.६ Lessons Learned

Closure meeting मा यस्ता प्रश्न सोध्न सकिन्छ:
- कुन defect requirement चरणमै भेट्न सकिन्थ्यो?
- कुन test case अनावश्यक वा दोहोरिएको थियो?
- Environment कति पटक असफल भयो?
- Test data तयार गर्न कति समय लाग्यो?
- Automation ले कहाँ मद्दत गर्‍यो र कहाँ flaky भयो?
- Regression coverage पर्याप्त थियो?
- अर्को Sprint मा कुन प्रक्रिया सुधार्ने?

प्रत्येक सुधारका लागि action, owner र target date राख्नु उपयोगी हुन्छ।

## १०.७ Closure का Deliverables

- Test Summary / Closure Report
- Final Test Metrics
- Defect Summary
- RTM / Coverage Report
- Known Issues and Residual Risks
- Sign-off / Release Recommendation
- Lessons Learned
- Archive गरिएका test artifacts

---

# ११. STLC मा प्रयोग हुने मुख्य कागजात

| कागजात | उद्देश्य | सामान्यतया कहिले |
|---|---|---|
| Requirement Specification / User Story | प्रणालीले के गर्नुपर्छ भन्ने आधार | Requirement Analysis |
| Test Plan | Scope, approach, schedule, risk र criteria | Test Planning |
| Test Scenario | उच्चस्तरीय परीक्षण क्षेत्र | Test Design |
| Test Case | चरण, data र expected result | Test Design |
| Test Data Sheet | परीक्षणका लागि input र setup | Test Design/Execution |
| RTM | Requirement र test case बीचको mapping | Requirement देखि Closure सम्म |
| Defect/Bug Report | पत्ता लागेको समस्या र प्रमाण | Execution |
| Test Execution Report | case को वास्तविक status | Execution |
| Environment Readiness Checklist | परीक्षण वातावरण तयार भएको प्रमाण | Setup |
| Test Summary Report | coverage, result, defects र residual risk | Closure |

कागजातको नामभन्दा त्यसमा रहेको जानकारी, version control र team ले प्रयोग गर्ने तरिका महत्त्वपूर्ण हुन्छ। सानो Agile team ले यी जानकारी ticket, wiki र automated pipeline मा राख्न सक्छ।

---

# १२. Bug / Defect Life Cycle

Defect को अवस्था प्रत्येक संस्थामा केही फरक हुन सक्छ। एउटा सामान्य workflow:

```text
New / Open
   ↓
Triage
   ↓
Assigned
   ↓
In Progress
   ↓
Fixed
   ↓
Ready for Retest
   ↓
Retest
  ↙   ↘
Pass   Fail
 ↓      ↓
Closed  Reopened → Assigned / In Progress
```

अन्य सम्भावित status:
- **Rejected / Not a Bug:** जाँचपछि requirement अनुसार काम गरेको वा defect नभएको निष्कर्ष।
- **Duplicate:** पहिले नै log भएको defect।
- **Deferred:** अर्को release मा सारिएको; कारण र जोखिम स्पष्ट हुनुपर्छ।
- **Cannot Reproduce:** उपलब्ध प्रमाणबाट पुनःउत्पादन हुन सकेन; थप logs/data माग्न सकिन्छ।
- **Blocked:** आवश्यक निर्भरता नहुँदा fix वा retest अघि बढ्न नसकेको।

**महत्त्वपूर्ण:** “Developer ले Fixed भनेको” र “QA ले Retest गरेर Pass गरेको” फरक कुरा हुन्। Fix build मा पुष्टि नभएसम्म defect स्वतः Closed हुँदैन, जबसम्म team को स्वीकृत प्रक्रिया फरक छैन।

---

# १३. Severity र Priority

## १३.१ Severity भनेको के हो?

Severity ले defect को प्राविधिक वा व्यावसायिक प्रभाव कति गम्भीर छ भन्ने जनाउँछ।

- **Critical:** प्रणाली/मुख्य सेवा ठप्प, गम्भीर data loss वा पुष्टि भएको गम्भीर security compromise।
- **High:** मुख्य workflow बिग्रिएको वा ठूलो प्रयोगकर्ता समूह प्रभावित।
- **Medium:** सीमित workaround सहित सुविधा आंशिक रूपमा बिग्रिएको।
- **Low:** सानो visual/content समस्या वा कम प्रभावको defect।

यी स्तरका परिभाषा संगठनअनुसार फरक हुन सक्छन्।

## १३.२ Priority भनेको के हो?

Priority ले defect कति चाँडो समाधान गर्नुपर्छ भन्ने व्यावसायिक प्राथमिकता जनाउँछ।

- P0 / Immediate
- P1 / High
- P2 / Normal
- P3 / Low

Priority का नाम र संख्या team ले परिभाषित गर्नुपर्छ।

## १३.३ Severity र Priority बीचको फरक

| उदाहरण | सम्भावित Severity | सम्भावित Priority |
|---|---|---|
| सबै नागरिकले निवेदन बुझाउन नसक्ने | High/Critical | P0/P1 |
| Login बाट अनधिकृत Admin पहुँच | Critical | P0 |
| मुख्य पेजमा महत्त्वपूर्ण सूचना गलत | Medium/High, प्रभावअनुसार | उच्च हुन सक्छ |
| कम प्रयोग हुने पेजमा सानो icon alignment समस्या | Low | Low |
| आगामी कार्यक्रमको मिति गलत, कार्यक्रम भोलि छ | प्रभावअनुसार Medium | तत्काल उच्च हुन सक्छ |

Severity र Priority सधैँ समान हुँदैनन्। अन्तिम निर्णय प्रमाण, जोखिम र business impact अनुसार गरिन्छ।

---

# १४. Test Metrics र Reporting

Metrics ले प्रगति र जोखिम बुझ्न मद्दत गर्छन्; तिनलाई कर्मचारीको प्रदर्शन मापन गर्ने एक मात्र आधार वा “जति धेरै bug, उति राम्रो tester” भन्ने निष्कर्षका लागि प्रयोग गर्नु हुँदैन।

## १४.१ Test Execution Coverage

उदाहरणको एउटा परिभाषा:

\[
\text{Execution Coverage} =
\frac{\text{चलाइएका Test Cases}}{\text{योजनाबद्ध Test Cases}} \times 100
\]

“चलाइएका” मा Blocked समावेश गर्ने/नगर्ने स्पष्ट रूपमा उल्लेख गर्नुपर्छ। व्यवहारमा Pass/Fail मात्र होइन, Blocked र Not Run अलग देखाउनु राम्रो हुन्छ।

## १४.२ Pass Rate

\[
\text{Pass Rate} =
\frac{\text{Pass}}{\text{Pass + Fail}} \times 100
\]

Pass Rate ले Blocked र Not Run लाई समेट्दैन। त्यसैले यसलाई एक्लै release readiness को प्रमाण मान्नु हुँदैन।

## १४.३ Requirement Coverage

\[
\text{Requirement Coverage} =
\frac{\text{कम्तीमा एउटा Test Case भएका Requirements}}{\text{कुल लागू Requirements}} \times 100
\]

Requirement मा test case हुनु र पर्याप्त रूपमा परीक्षण हुनु फरक कुरा हो। Coverage सँगै test quality, risk र execution status पनि हेर्नुपर्छ।

## १४.४ Defect Metrics

- Defect Count by Severity
- Open vs Closed Defects
- Defect Reopen Rate
- Defect Aging (कति समयदेखि खुला)
- Defect Leakage (परीक्षणबाट छुटेर पछिल्लो चरण/Production मा भेटिएका defect)
- Defect Density (उपयुक्त र तुलनायोग्य आकारको आधारमा)
- Escaped Defect Rate

Metrics को denominator र समयावधि स्पष्ट नराखे तुलना भ्रमपूर्ण हुन सक्छ।

## १४.५ उदाहरण

कुल test cases = 120  
Pass = 90  
Fail = 10  
Blocked = 10  
Not Run = 10

यदि कुल planned 120 हो र “attempted” मा Pass + Fail मात्र गनिन्छ भने attempted = 100; त्यसैले attempted coverage = 100/120 × 100 = 83.3%। Blocked छुट्टै 10 छन्। Pass rate = 90/(90+10) × 100 = 90%।

यसको अर्थ 90% pass rate भए पनि 10 case blocked र 10 not run भएकाले बाँकी जोखिम छ। रिपोर्टमा सबै संख्या देखाउनुपर्छ।

---

# १५. Risk-Based Testing

Risk-Based Testing मा सबै कुरा समान रूपमा परीक्षण गर्नुको सट्टा असफल हुँदा प्रभाव र असफल हुने सम्भावना बढी भएका क्षेत्रमा प्राथमिकता दिइन्छ।

## १५.१ सरल Risk Score

सिकाइका लागि एउटा सामान्य विधि:

\[
\text{Risk Score} = \text{Impact} \times \text{Likelihood}
\]

यदि दुवैलाई 1 देखि 5 सम्म अंक दिइयो भने score 1–25 हुन्छ। यो कुनै सार्वभौमिक मानक होइन; team ले परिभाषित र consistent रूपमा प्रयोग गर्नुपर्छ।

| सुविधा | Impact (1–5) | Likelihood (1–5) | Score | प्राथमिकता |
|---|---:|---:|---:|---|
| Login / Access Control | 5 | 4 | 20 | अति उच्च |
| निवेदन Submit | 5 | 3 | 15 | उच्च |
| File Upload | 4 | 4 | 16 | उच्च |
| Footer icon alignment | 1 | 2 | 2 | न्यून |

## १५.२ उच्च जोखिम क्षेत्रमा के जाँच्ने?

- Authentication र authorization
- Data loss / duplicate submission
- File upload validation
- व्यक्तिगत डेटा सुरक्षा
- Payment वा वित्तीय गणना, यदि लागू हुन्छ
- Audit log र approval workflow
- API validation र rate limiting
- Backup/restore तथा recovery, आवश्यकताअनुसार

जोखिम स्कोर प्राथमिकता निर्धारणको सहयोगी हो, स्वतः release निर्णय गर्ने यन्त्र होइन।

---

# १६. Requirement Traceability Matrix (RTM)

RTM ले requirement, test scenario/test case र execution result बीचको सम्बन्ध देखाउँछ। यसले आवश्यकता छुटेको छ कि छैन, कुन test ले कुन requirement जाँच्छ र परिवर्तन हुँदा कुन test पुनः चलाउनुपर्छ भन्ने पत्ता लगाउन मद्दत गर्छ।

## १६.१ नमुना RTM

| Requirement ID | Requirement | Test Case IDs | Execution Status | Defect |
|---|---|---|---|---|
| REQ-LOGIN-01 | सही विवरणबाट login | TC-LOGIN-001 | Pass | — |
| REQ-LOGIN-02 | गलत विवरण अस्वीकार | TC-LOGIN-002 | Pass | — |
| REQ-UPLOAD-01 | स्वीकृत file type/size | TC-UPLOAD-001, 002, 003 | Fail | BUG-UPLOAD-007 |
| REQ-ROLE-01 | नागरिकले Admin access नपाउने | TC-ROLE-002 | Pass | — |

## १६.२ RTM किन उपयोगी छ?

- Requirement coverage देखाउँछ।
- अनावश्यक duplicate testing पत्ता लगाउन मद्दत गर्छ।
- Requirement परिवर्तनको प्रभाव विश्लेषण गर्न सजिलो हुन्छ।
- Audit वा औपचारिक approval चाहिने परियोजनामा प्रमाण दिन्छ।
- Test Closure मा coverage रिपोर्ट बनाउन सहयोग गर्छ।

---

# १७. Automation Testing र STLC

Automation Testing भनेको test execution वा जाँचका केही काम tool/script मार्फत स्वचालित गर्नु हो। Automation ले सबै manual testing हटाउँदैन। exploratory testing, usability judgment, नयाँ feature को अनिश्चित व्यवहार र धेरै दृश्य/मानवीय मूल्याङ्कन आवश्यक हुने ठाउँमा manual testing अझै महत्त्वपूर्ण हुन्छ।

## १७.१ कुन test automate गर्ने?

उपयुक्त उम्मेदवार:
- बारम्बार चलाइने regression test
- स्थिर र स्पष्ट expected result भएका workflow
- धेरै data combination परीक्षण
- API contract/validation test
- प्रत्येक build मा चलाउनुपर्ने smoke test
- दोहोरिने browser compatibility checks

सुरुमा automate नगर्न उपयुक्त हुन सक्ने:
- बारम्बार बदलिने UI
- अस्पष्ट requirement
- एकपटक मात्र चलाइने सानो परीक्षण
- automation बनाउन/मर्मत गर्न लाग्ने खर्चभन्दा कम लाभ हुने test
- परीक्षण गर्न सुरक्षित, स्थिर test data वा environment नै नभएको workflow

## १७.२ Automation STLC मा कहाँ पर्छ?

- Requirement Analysis: automation का लागि testability र जोखिम बुझ्ने।
- Test Planning: tool, framework, CI/CD र maintenance cost तय गर्ने।
- Test Design: reusable test case र data design गर्ने।
- Environment Setup: browser driver, API endpoint, secrets र test accounts सुरक्षित रूपमा तयार गर्ने।
- Execution: automated suite चलाउने; failure triage गर्ने।
- Closure: pass/fail, flaky test, coverage र maintenance debt रिपोर्ट गर्ने।

## १७.३ Flaky Test भनेको के हो?

एउटै code/build र समान अवस्थामै कहिले pass, कहिले fail हुने अस्थिर test लाई flaky test भनिन्छ। कारणमा timing, asynchronous behavior, shared data, environment instability वा कमजोर locator हुन सक्छन्।

Flaky test लाई बारम्बार rerun गरेर हराएको जस्तो देखाउनु ठीक होइन; मूल कारण खोजेर स्थिर बनाउनु आवश्यक हुन्छ।

---

# १८. Agile/Scrum मा STLC

Agile/Scrum मा testing प्रायः छुट्टै ठूलो चरणको अन्त्यमा मात्र हुँदैन। Requirement, development, testing र feedback एउटै Sprint भित्र निरन्तर हुन सक्छन्।

## १८.१ Sprint मा STLC को उदाहरण

1. **Backlog Refinement:** User Story, acceptance criteria र testability review।
2. **Sprint Planning:** Scope, risk, testing approach र capacity अनुमान।
3. **Development का क्रममा:** Code review, unit test, API test, test case तयार।
4. **Build उपलब्ध हुँदा:** Smoke test, functional/integration test।
5. **Bug fix पछि:** Retest र risk-based regression।
6. **Sprint Review:** कामको demo र stakeholder feedback।
7. **Retrospective:** प्रक्रिया सुधारका काम तय गर्ने।

## १८.२ Definition of Ready (DoR) र Definition of Done (DoD)

- **Definition of Ready:** Story काम सुरु गर्न पर्याप्त स्पष्ट छ कि छैन भन्ने team को साझा मापदण्ड।
- **Definition of Done:** Story लाई पूरा भन्न आवश्यक मापदण्ड, जस्तै acceptance criteria पूरा, review, आवश्यक tests pass, documentation र defect status को सहमति।

DoR/DoD को ठ्याक्कै सूची प्रत्येक team ले आफ्नो उत्पादन र जोखिमअनुसार तय गर्छ।

## १८.३ QA विकासपछि मात्र सुरु हुन्छ?

हुँदैन। QA ले refinement मा प्रश्न उठाउन, acceptance criteria स्पष्ट पार्न, test design तयार गर्न र जोखिम पहिचान गर्न सक्छ। Developer ले coding कै क्रममा unit test लेख्न सक्छ; API र integration test service तयार भएपछि चलाउन सकिन्छ। त्यसैले परीक्षण र गुणस्तर सुनिश्चित गर्ने गतिविधि SDLC भरि चल्छन्।

---

# १९. Beginner देखि Advanced सम्म अभ्यास योजना

## Level 1 — Beginner

लक्ष्य: मुख्य अवधारणा र सरल functional test बुझ्ने।

- STLC का चरण नाम र उद्देश्य सम्झने।
- Requirement र Test Case बीचको फरक बुझ्ने।
- Login का 10 वटा positive/negative test case लेख्ने।
- Expected र Actual Result छुट्याउने।
- Pass/Fail/Blocked status प्रयोग गर्ने।
- एउटा defect report तयार गर्ने।

**अभ्यास:** Login form का लागि valid email, invalid email, blank field, wrong password, inactive account, password visibility र logout परीक्षणको checklist बनाउनुहोस्।

## Level 2 — Intermediate

लक्ष्य: systematic test design र reporting गर्न सक्ने।

- Equivalence Partitioning
- Boundary Value Analysis
- Decision Table
- State Transition
- RTM
- Severity/Priority
- Retest/Regression
- Test Summary Report

**अभ्यास:** “Нागरिक सेवा निवेदन” workflow का 20–30 test cases तयार गरी Requirement ID सँग map गर्नुहोस्। अनिवार्य field, duplicate submit, invalid file, role access र status transition समेट्नुहोस्।

## Level 3 — Advanced

लक्ष्य: जोखिम, गुणस्तर र release readiness को विश्लेषण गर्न सक्ने।

- Risk-based test prioritization
- API integration/security validation
- Performance test planning
- Accessibility and cross-browser strategy
- Automation selection and flaky test analysis
- Defect trend र leakage analysis
- Test estimation र coverage reporting
- Change impact analysis
- Residual risk र release recommendation

**अभ्यास:** काल्पनिक release का लागि Test Plan, RTM, defect dashboard र closure report बनाउनुहोस्। 5 वटा खुला defect मध्ये कुन release रोक्ने, कुन workaround सहित स्वीकार गर्न सकिने र कसले निर्णय गर्नुपर्छ भन्ने कारणसहित लेख्नुहोस्।

## १९.१ Portfolio अभ्यास परियोजना

एउटा सानो Login + Service Request web application छान्नुहोस्। निम्न artifact तयार गर्नुहोस्:

1. `REQUIREMENT_ANALYSIS.md`
2. `TEST_PLAN.md`
3. `TEST_CASES.md`
4. `RTM.csv` वा Markdown table
5. `DEFECT_REPORTS.md`
6. `TEST_EXECUTION_REPORT.md`
7. `TEST_CLOSURE_REPORT.md`

यसले interview वा QA portfolio मा प्रक्रिया बुझाइ देखाउन सहयोग गर्छ। वास्तविक नतिजा नभएको test लाई “Pass” भनेर नलेख्नुहोस्; नमुना/काल्पनिक हो भने स्पष्ट लेबल लगाउनुहोस्।

---

# २०. अभ्यास प्रश्न तथा उत्तर

## प्रश्न १: STLC के हो?
**उत्तर:** Software Testing Life Cycle भनेको परीक्षणलाई चरणबद्ध, व्यवस्थित र मापनयोग्य रूपमा सम्पन्न गर्ने प्रक्रिया हो।

## प्रश्न २: STLC का मुख्य चरण के-के हुन्?
**उत्तर:** Requirement Analysis, Test Planning, Test Case Design, Test Environment Setup, Test Execution र Test Closure। केही मोडेलमा Setup लाई अन्य चरणमा समेटिन्छ।

## प्रश्न ३: Requirement Analysis किन आवश्यक छ?
**उत्तर:** आवश्यकताहरू स्पष्ट, पूर्ण, एकरूप र परीक्षणयोग्य छन् कि छैनन् जाँच्न तथा अस्पष्टता/जोखिम समयमै पत्ता लगाउन।

## प्रश्न ४: Test Scenario र Test Case बीच के फरक छ?
**उत्तर:** Scenario ले के जाँच्ने भन्ने उच्चस्तरीय क्षेत्र बताउँछ; Test Case ले precondition, steps, data र expected result सहित कसरी जाँच्ने भन्ने बताउँछ।

## प्रश्न ५: Retesting र Regression Testing बीच के फरक छ?
**उत्तर:** Retesting ले विशेष defect fix भएको पुष्टि गर्छ; Regression ले परिवर्तनले अन्य सुविधा नबिगारेको जाँच गर्छ।

## प्रश्न ६: Test Closure मा सबै defect बन्द हुनैपर्छ?
**उत्तर:** आवश्यक छैन। खुला defect र बाँकी जोखिम स्पष्ट अभिलेख, मूल्याङ्कन र अधिकारप्राप्त व्यक्तिबाट निर्णय गरिएको हुनुपर्छ। परियोजनाको exit criteria ले के स्वीकार्य छ भन्ने निर्धारण गर्छ।

## प्रश्न ७: 100% test cases Pass भए software पूर्ण रूपमा bug-free हुन्छ?
**उत्तर:** हुँदैन। Test case ले जाँचेका अवस्थाहरूमा मात्र प्रमाण दिन्छ। Coverage बाहिरका अवस्था, नयाँ वातावरण, अप्रत्याशित प्रयोग र अज्ञात जोखिम बाँकी हुन सक्छन्।

## प्रश्न ८: QA कहिले सुरु हुनुपर्छ?
**उत्तर:** आवश्यकता र डिजाइन चरणदेखि नै QA गतिविधि सुरु हुन सक्छ। सबै परीक्षण code बनेपछि मात्र सुरु गर्नुपर्छ भन्ने होइन।

## प्रश्न ९: Blocked test case लाई Fail मान्ने?
**उत्तर:** सामान्यतया होइन। आवश्यक वातावरण/डेटा/निर्भरता नभएकाले परीक्षण गर्न नसकिएको हो भने Blocked भनेर स्पष्ट रिपोर्ट गर्नुपर्छ।

## प्रश्न १०: Severity र Priority फरक के हो?
**उत्तर:** Severity ले प्रभावको गम्भीरता जनाउँछ; Priority ले समाधानको समय/व्यावसायिक प्राथमिकता जनाउँछ।

## प्रश्न ११: RTM किन चाहिन्छ?
**उत्तर:** Requirement देखि test case र execution result सम्म traceability राख्न, coverage जाँच्न र requirement परिवर्तनको प्रभाव पत्ता लगाउन।

## प्रश्न १२: Smoke Testing र Sanity Testing बीच फरक?
**उत्तर:** Smoke ले build को मुख्य कार्यक्षमता प्रारम्भिक रूपमा जाँच्छ; Sanity ले सीमित परिवर्तन वा fix को लक्षित व्यवहार जाँच्छ। व्यवहारमा परिभाषा team अनुसार फरक हुन सक्छ।

---

# २१. Glossary — महत्त्वपूर्ण शब्दावली

| शब्द | सरल नेपाली अर्थ |
|---|---|
| QA (Quality Assurance) | गुणस्तर सुनिश्चित गर्न प्रक्रिया सुधार र रोकथाममा केन्द्रित गतिविधि |
| QC (Quality Control) | उत्पादन/नतिजा जाँचेर त्रुटि पत्ता लगाउने गतिविधि |
| Testing | अपेक्षित र वास्तविक व्यवहार जाँच्ने प्रक्रिया |
| Requirement | प्रणालीले पूरा गर्नुपर्ने आवश्यकता |
| Acceptance Criteria | आवश्यकता स्वीकार गर्न पूरा हुनुपर्ने मापदण्ड |
| Test Scenario | उच्चस्तरीय परीक्षण अवस्था/क्षेत्र |
| Test Case | परीक्षण चरण, input र expected result सहितको विवरण |
| Test Data | परीक्षणमा प्रयोग हुने डेटा |
| Expected Result | अपेक्षित नतिजा |
| Actual Result | परीक्षण गर्दा देखिएको वास्तविक नतिजा |
| Defect / Bug | आवश्यकता वा अपेक्षित व्यवहारसँग नमिलेको समस्या |
| Severity | defect को प्रभावको गम्भीरता |
| Priority | समाधानको प्राथमिकता |
| Retesting | defect fix को पुनःपुष्टि |
| Regression Testing | परिवर्तनले पुरानो व्यवहार नबिगारेको जाँच |
| Smoke Testing | build का मुख्य सुविधा चल्ने प्रारम्भिक जाँच |
| Sanity Testing | सानो परिवर्तनको लक्षित जाँच |
| RTM | Requirement र test case बीचको mapping |
| Test Coverage | आवश्यकता वा परीक्षण क्षेत्र कति समेटियो भन्ने मापन |
| Test Environment | परीक्षण चलाइने configuration र प्रणाली |
| Test Oracle | नतिजा सही/गलत ठहर गर्ने आधार |
| Entry Criteria | चरण सुरु गर्न आवश्यक सर्त |
| Exit Criteria | चरण पूरा भएको मान्न आवश्यक सर्त |
| Test Closure | परीक्षण नतिजा, जोखिम र सिकाइको औपचारिक समापन |
| UAT | User Acceptance Testing |
| E2E | End-to-End Testing |
| CI/CD | Continuous Integration / Continuous Delivery वा Deployment |
| Flaky Test | समान अवस्थामा पनि अस्थिर नतिजा दिने test |
| Shift Left | विकासको प्रारम्भिक चरणमै testing/quality गतिविधि सुरु गर्ने दृष्टिकोण |
| Residual Risk | परीक्षणपछि पनि बाँकी रहेको जोखिम |
| Sign-off | समीक्षा/स्वीकृति भएको औपचारिक अभिलेख |

---

# २२. अन्तिम पुनरावलोकन चेकलिस्ट

## Requirement Analysis
- [ ] आवश्यकता पढिएको र अस्पष्टता उठाइएको छ।
- [ ] Functional/Non-functional आवश्यकता पहिचान छन्।
- [ ] Testability र risk जाँचिएको छ।
- [ ] आवश्यक stakeholder प्रश्नको जिम्मेवारी तोकिएको छ।

## Test Planning
- [ ] Objective र scope स्पष्ट छन्।
- [ ] In Scope / Out of Scope लेखिएको छ।
- [ ] Test approach, resources र schedule तय छन्।
- [ ] Risk, dependency र defect workflow लेखिएका छन्।
- [ ] Entry/Exit Criteria स्पष्ट छन्।

## Test Case Design
- [ ] Test scenarios र test cases तयार छन्।
- [ ] Positive, negative र boundary अवस्थाहरू समेटिएका छन्।
- [ ] Expected result स्पष्ट र परीक्षणयोग्य छ।
- [ ] Test data र preconditions छन्।
- [ ] RTM अद्यावधिक छ र review गरिएको छ।

## Environment Setup
- [ ] सही build/version छ।
- [ ] Backend/API/database connection जाँचिएको छ।
- [ ] Test account, roles र data तयार छन्।
- [ ] Smoke test सफल वा failure स्पष्ट रूपमा रिपोर्ट गरिएको छ।
- [ ] सुरक्षा र data privacy को व्यवस्था छ।

## Test Execution
- [ ] Case अनुसार नतिजा अभिलेख गरिएको छ।
- [ ] Fail भएका case मा पुनःउत्पादन गर्न मिल्ने प्रमाण छ।
- [ ] Defect सही severity/priority सहित log गरिएको छ।
- [ ] Fix पछि retest गरिएको छ।
- [ ] जोखिमअनुसार regression test गरिएको छ।
- [ ] Blocked/Not Run अवस्था लुकाइएको छैन।

## Test Closure
- [ ] Execution, coverage र defect सारांश तयार छ।
- [ ] बाँकी जोखिम र known issues स्पष्ट छन्।
- [ ] Exit Criteria मूल्याङ्कन गरिएको छ।
- [ ] आवश्यक stakeholder बाट निर्णय/sign-off लिइएको छ।
- [ ] Test artifacts सुरक्षित गरिएको छ।
- [ ] Lessons Learned र सुधार कार्य तोकिएका छन्।

---

# निष्कर्ष

STLC को मूल विचार भनेको परीक्षणलाई अन्तिम समयमा गरिने एकपटकको गतिविधि नबनाई, आवश्यकता बुझ्ने चरणदेखि नै योजना, डिजाइन, वातावरण, execution र closure सम्म व्यवस्थित रूपमा चलाउनु हो।

याद राख्नुपर्ने मुख्य कुरा:

1. **Requirement Analysis:** के परीक्षण गर्ने र requirement परीक्षणयोग्य छ कि छैन बुझ्ने।
2. **Test Planning:** कसरी, कसले, कहिले र कुन जोखिमलाई प्राथमिकता दिएर परीक्षण गर्ने तय गर्ने।
3. **Test Case Design:** स्पष्ट steps, data र expected result सहित परीक्षण तयार गर्ने।
4. **Test Environment Setup:** परीक्षणका लागि सही build, configuration, account र data तयार गर्ने।
5. **Test Execution:** वास्तविक नतिजा जाँच्ने, प्रमाण राख्ने, defect log गर्ने, retest र regression गर्ने।
6. **Test Closure:** coverage, परिणाम, defect, बाँकी जोखिम र सिकाइको सारांश तयार गर्ने।

**सबैभन्दा महत्त्वपूर्ण सिद्धान्त:** परीक्षणको उद्देश्य केवल “Pass” संख्या बढाउनु होइन; उत्पादनको गुणस्तर र जोखिमबारे सही, प्रमाणमा आधारित जानकारी दिनु हो।
"""
