# विषयसूची (Table of Contents)

- [१. SDLC र STLC को परिचय तथा आपसी सम्बन्ध](#१-sdlc-र-stlc-को-परिचय-तथा-आपसी-सम्बन्ध)
  - [१.१ SDLC भनेको के हो?](#११-sdlc-भनेको-के-हो)
  - [१.२ STLC भनेको के हो?](#१२-stlc-भनेको-के-हो)
  - [१.३ दुवैबीचको मुख्य सम्बन्ध](#१३-दुवैबीचको-मुख्य-सम्बन्ध)
- [२. SDLC र STLC बीचको विस्तृत तुलना](#२-sdlc-र-stlc-बीचको-विस्तृत-तुलना)
- [३. SDLC र STLC का चरणहरू कसरी सम्बन्धित हुन्छन्?](#३-sdlc-र-stlc-का-चरणहरू-कसरी-सम्बन्धित-हुन्छन्)
- [४. QA ले Development सुरु हुनुअघि नै किन काम सुरु गर्छ?](#४-qa-ले-development-सुरु-हुनुअघि-नै-किन-काम-सुरु-गर्छ)
  - [४.१ परम्परागत सोच र आधुनिक QA](#४१-परम्परागत-सोच-र-आधुनिक-qa)
  - [४.२ QA ले चाँडै काम सुरु गर्नुका कारण](#४२-qa-ले-चाँडै-काम-सुरु-गर्नुका-कारण)
  - [४.३ वास्तविक उदाहरण](#४३-वास्तविक-उदाहरण)
  - [४.४ Defect पत्ता लाग्ने चरणअनुसार सुधारको प्रभाव](#४४-defect-पत्ता-लाग्ने-चरणअनुसार-सुधारको-प्रभाव)
- [५. V-Model मा Development र Testing को सम्बन्ध](#५-v-model-मा-development-र-testing-को-सम्बन्ध)
  - [५.१ V-Model का मुख्य Testing स्तरहरू](#५१-v-model-का-मुख्य-testing-स्तरहरू)
  - [५.२ Verification र Validation बीचको सम्बन्ध](#५२-verification-र-validation-बीचको-सम्बन्ध)
- [६. Agile/Scrum मा SDLC र STLC कसरी दोहोरिन्छन्?](#६-agilescrum-मा-sdlc-र-stlc-कसरी-दोहोरिन्छन्)
  - [६.१ Agile मा SDLC का गतिविधि](#६१-agile-मा-sdlc-का-गतिविधि)
  - [६.२ Agile मा STLC का गतिविधि](#६२-agile-मा-stlc-का-गतिविधि)
  - [६.३ Definition of Done (DoD) भनेको के हो?](#६३-definition-of-done-dod-भनेको-के-हो)
  - [६.४ Agile र Waterfall बीच Testing को मुख्य भिन्नता](#६४-agile-र-waterfall-बीच-testing-को-मुख्य-भिन्नता)
- [७. Login System को उदाहरणबाट SDLC र STLC बुझ्ने](#७-login-system-को-उदाहरणबाट-sdlc-र-stlc-बुझ्ने)
  - [७.१ SDLC अनुसार Login System विकास](#७१-sdlc-अनुसार-login-system-विकास)
  - [७.२ STLC अनुसार Login System परीक्षण](#७२-stlc-अनुसार-login-system-परीक्षण)
  - [७.३ Login System का नमुना Test Cases](#७३-login-system-का-नमुना-test-cases)
  - [७.४ एउटा Test Case को विस्तृत नमुना](#७४-एउटा-test-case-को-विस्तृत-नमुना)
  - [७.५ Defect भेटिएपछि के हुन्छ?](#७५-defect-भेटिएपछि-के-हुन्छ)
- [८. SDLC र STLC मा थप बुझ्नुपर्ने महत्त्वपूर्ण विषयहरू](#८-sdlc-र-stlc-मा-थप-बुझ्नुपर्ने-महत्त्वपूर्ण-विषयहरू)
  - [८.१ Entry Criteria र Exit Criteria](#८१-entry-criteria-र-exit-criteria)
  - [८.२ Requirement Traceability Matrix (RTM)](#८२-requirement-traceability-matrix-rtm)
  - [८.३ Test Coverage र Test Metrics](#८३-test-coverage-र-test-metrics)
  - [८.४ Defect Life Cycle](#८४-defect-life-cycle)
  - [८.५ Severity र Priority](#८५-severity-र-priority)
  - [८.६ Testing र Quality Assurance बीचको भिन्नता](#८६-testing-र-quality-assurance-बीचको-भिन्नता)
  - [८.७ Release Readiness र Test Closure](#८७-release-readiness-र-test-closure)
- [९. SDLC र STLC सम्बन्धी महत्त्वपूर्ण Interview Questions and Answers](#९-sdlc-र-stlc-सम्बन्धी-महत्त्वपूर्ण-interview-questions-and-answers)
- [१०. परीक्षाका लागि Short Notes](#१०-परीक्षाका-लागि-short-notes)
- [११. SDLC र STLC को Quick Revision](#११-sdlc-र-stlc-को-quick-revision)
- [१२. SDLC र STLC सम्झिने सजिलो तरिका](#१२-sdlc-र-stlc-सम्झिने-सजिलो-तरिका)
- [१३. निष्कर्ष](#१३-निष्कर्ष)

---

## १. SDLC र STLC को परिचय तथा आपसी सम्बन्ध

### १.१ SDLC भनेको के हो?

**SDLC (Software Development Life Cycle)** सफ्टवेयरको योजना बनाउने, आवश्यकता विश्लेषण गर्ने, डिजाइन गर्ने, विकास गर्ने, परीक्षण गर्ने, Deploy गर्ने र Maintenance गर्ने समग्र प्रक्रिया हो।

### १.२ STLC भनेको के हो?

**STLC (Software Testing Life Cycle)** सफ्टवेयरको गुणस्तर जाँच्न आवश्यकताहरू विश्लेषण गर्ने, Testing Plan बनाउने, Test Cases तयार गर्ने, Test Environment सेटअप गर्ने, परीक्षण गर्ने, Defects व्यवस्थापन गर्ने र Testing Closure गर्ने व्यवस्थित प्रक्रिया हो।

### १.३ दुवैबीचको मुख्य सम्बन्ध

SDLC ले सफ्टवेयर कसरी निर्माण र सञ्चालन गर्ने भन्ने समग्र प्रक्रिया समेट्छ भने STLC ले त्यस सफ्टवेयरले आवश्यकताहरू पूरा गर्छ कि गर्दैन भनेर परीक्षण गर्ने प्रक्रिया व्यवस्थित गर्छ।

```text
SDLC — Overall Software Development
Planning → Requirements → Design → Coding → Testing → Deployment → Maintenance
                              ↕
                    समन्वय र Feedback
                              ↕
STLC — Software Testing Process
Requirement Analysis → Test Planning → Test Design → Environment Setup
                 → Test Execution → Defect Management → Test Closure
```

**नोट:** STLC, SDLC को Testing चरणमा मात्र सीमित हुँदैन। Testing सम्बन्धी योजना र गतिविधिहरू Requirements तथा Design चरणदेखि नै सुरु हुन सक्छन्।

**उदाहरण:** नगरपालिका पोर्टल बनाउँदा SDLC ले Login, नागरिक आवेदन, कर्मचारी Dashboard र प्रमाणपत्रसम्बन्धी सुविधा निर्माण गर्न समन्वय गर्छ। STLC ले ती सुविधाहरू सही, सुरक्षित र आवश्यकताअनुसार चलेका छन् कि छैनन् जाँच्छ।

---

## २. SDLC र STLC बीचको विस्तृत तुलना

| तुलना गर्ने आधार | SDLC | STLC |
|---|---|---|
| पूरा रूप | Software Development Life Cycle | Software Testing Life Cycle |
| मुख्य उद्देश्य | सफ्टवेयर निर्माण तथा सञ्चालन | सफ्टवेयरको गुणस्तर परीक्षण |
| मुख्य प्रश्न | सफ्टवेयर कसरी बनाउने? | सफ्टवेयर सही रूपमा काम गर्छ? |
| Scope | योजना, विकास, Testing, Deployment र Maintenance | परीक्षण योजना, डिजाइन, Execution, Defect Management र Closure |
| सुरुवात | परियोजना तथा आवश्यकताको पहिचानबाट | Testing का लागि आवश्यकता विश्लेषणबाट; QA गतिविधि यसअघि पनि सुरु हुन सक्छ |
| प्रमुख कार्य | Requirement, Design, Coding, Integration, Release | Test Analysis, Planning, Test Design, Execution |
| प्रमुख जिम्मेवारी | Business Analyst, Developer, Architect, QA सहितको टोली | QA Engineer, Test Analyst, Tester तथा Automation Engineer |
| प्रमुख Input | Business Needs, Requirements, Project Scope | Requirements, Acceptance Criteria, Design र Testable Artifacts |
| प्रमुख Output | कार्यशील सफ्टवेयर तथा Release | Test Results, Defect Reports, Coverage र Test Summary |
| गुणस्तरमा भूमिका | गुणस्तर निर्माण गर्ने सम्पूर्ण प्रक्रिया | गुणस्तर मूल्याङ्कन गर्ने र त्रुटि पहिचान गर्ने प्रक्रिया |
| Coding | सामान्यतया मुख्य भाग | Testing Code वा Automation Script लेख्न सकिन्छ; Application Coding मुख्य काम होइन |
| Defect Handling | त्रुटिको कारण पत्ता लगाई Code वा Design सुधार गर्ने | Defect पहिचान, रिपोर्ट, Retest र Regression Test गर्ने |
| सफलता मापन | आवश्यकता पूरा भएको, उपयोगी र सञ्चालनयोग्य Software | पर्याप्त Testing, अपेक्षित Results, जोखिम र Defect को मूल्याङ्कन |
| अन्तिम परिणाम | प्रयोग गर्न सकिने सफ्टवेयर | परीक्षणको नतिजा तथा Release सम्बन्धी निर्णयमा सहयोग |

**ध्यान दिनुहोस्:** SDLC र STLC का जिम्मेवारीहरू पूर्ण रूपमा अलग हुँदैनन्। Developer ले Unit Test गर्न सक्छन्, QA ले Requirement Review गर्न सक्छन् र Business User ले Acceptance Testing मा भाग लिन सक्छन्।

---

## ३. SDLC र STLC का चरणहरू कसरी सम्बन्धित हुन्छन्?

| SDLC चरण | सम्बन्धित STLC गतिविधि | उदाहरण |
|---|---|---|
| Planning | Testing को प्रारम्भिक Scope र जोखिम पहिचान | Login, आवेदन र Payment मध्ये कुन-कुन परीक्षण गर्ने? |
| Requirement Analysis | Requirement Review, Testability Analysis | गलत Password हुँदा के देखिनुपर्छ? |
| System Design | Test Strategy, Test Scenarios तथा Design Review | Login API, Session र Role Access कसरी परीक्षण गर्ने? |
| Development | Unit Testing, Test Case Preparation, Automation Development | Password Validation का Test Cases तयार गर्ने |
| Testing | Test Execution, Defect Reporting, Retesting, Regression | सही र गलत Login परीक्षण गर्ने |
| Deployment | Smoke Test, Release Verification | Production मा Login र मुख्य API चल्छन् कि चल्दैनन्? |
| Maintenance | Regression Testing, Change Testing | Password Reset परिवर्तनपछि Login फेरि परीक्षण गर्ने |

### यस सम्बन्धका महत्त्वपूर्ण पक्षहरू

- **Shift-left Testing:** विकासको प्रारम्भिक चरणमै Testing सम्बन्धी काम सुरु गर्नु।
- **Continuous Testing:** विकाससँगै उपयुक्त समयमा बारम्बार परीक्षण गर्नु।
- **Feedback Loop:** परीक्षणबाट भेटिएका Defects विकास टोलीलाई पठाएर सुधारपछि पुनः परीक्षण गर्नु।
- **Traceability:** Requirement देखि Test Case र Defect सम्मको सम्बन्ध कायम राख्नु।
- **Risk-based Testing:** उच्च जोखिम भएका सुविधालाई प्राथमिकता दिनु।

माथिका गतिविधिहरू प्रत्येक परियोजनामा एउटै क्रम र समयमा हुँदैनन्। Waterfall, V-Model र Agile जस्ता Development Model अनुसार Testing को व्यवस्था फरक हुन सक्छ।

---

## ४. QA ले Development सुरु हुनुअघि नै किन काम सुरु गर्छ?

यो SDLC र STLC सम्बन्धी सबैभन्दा महत्त्वपूर्ण विषयमध्ये एक हो।

### ४.१ परम्परागत सोच र आधुनिक QA

परम्परागत सोचमा पहिले सम्पूर्ण Coding सकिन्छ र त्यसपछि Testing सुरु गरिन्छ। तर आधुनिक Software Development मा QA ले Requirements तथा Design चरणदेखि नै सहभागिता जनाउन सक्छ।

यसलाई **Shift-left Testing** भनिन्छ।

### ४.२ QA ले चाँडै काम सुरु गर्नुका कारण

1. **Requirement मा अस्पष्टता पत्ता लगाउन:** उदाहरणका लागि, गलत Password, निष्क्रिय Account, Password Reset र धेरै असफल Login प्रयासमा के हुन्छ भन्ने कुरा स्पष्ट पार्न।
2. **सुरक्षा तथा जोखिम पहिल्यै पहिचान गर्न:** Password सुरक्षित भण्डारण, Role-based Access Control, Session Management र Sensitive Data Protection जस्ता आवश्यकताहरू Design मै विचार गर्न।
3. **Test Cases पहिल्यै तयार गर्न:** Developer ले Coding गरिरहँदा QA ले Test Scenarios, Test Cases, Test Data र अपेक्षित नतिजा तयार गर्न सक्छ।
4. **समय र लागत बचत गर्न:** Design वा Requirement मै भेटिएको समस्या सुधार्न प्रायः Coding सकिएपछि भेटिएको उही समस्याभन्दा कम प्रयास लाग्न सक्छ।
5. **Acceptance Criteria स्पष्ट बनाउन:** सुविधा कहिले सही मानिने भन्ने कुरा पहिले नै तय गरी Developer, Tester र ग्राहकबीचको गलत बुझाइ घटाउन।

### ४.३ वास्तविक उदाहरण

Requirement: “प्रयोगकर्ताले Login गर्न सक्नुपर्छ।”

यो Requirement अस्पष्ट छ। QA ले निम्न प्रश्नहरू उठाउन सक्छ:

- Username गलत भए के हुन्छ?
- Password गलत भए के हुन्छ?
- दुवै Field खाली भए के हुन्छ?
- Account निष्क्रिय भए Login गर्न मिल्छ?
- कर्मचारीले नागरिकको Admin Dashboard खोल्न सक्छ?
- धेरै पटक गलत Password हालेमा के हुन्छ?
- Password Reset गरेपछि पुरानो Session को व्यवहार के हुन्छ?

यी प्रश्नहरूको उत्तर Requirement मा समावेश भएपछि Developer र Tester दुवैले एउटै अपेक्षाअनुसार काम गर्न सक्छन्।

### ४.४ Defect पत्ता लाग्ने चरणअनुसार सुधारको प्रभाव

| Defect भेटिएको चरण | सम्भावित प्रभाव |
|---|---|
| Requirement | Requirement स्पष्ट पारेर सुधार |
| Design | Architecture वा Design परिवर्तन |
| Development | Code परिवर्तन र Unit Testing |
| System Testing | Code Fix, Retesting र Regression |
| Production | वास्तविक प्रयोगकर्तामा असर, Incident Response, Hotfix वा Rollback |

सबै Early Defects सधैँ सस्ता हुन्छन् भन्ने होइन। तर समस्या फैलिनुअघि पत्ता लगाउँदा पुनःकाम तथा जोखिम कम गर्ने अवसर बढी हुन्छ।

**निष्कर्ष:** QA को काम केवल Bug खोज्नु होइन; आवश्यकता स्पष्ट पार्न, जोखिम घटाउन र सुरुदेखि नै गुणस्तर निर्माण गर्न सहयोग गर्नु पनि हो।

---

## ५. V-Model मा Development र Testing को सम्बन्ध

V-Model (Verification and Validation Model) SDLC को यस्तो मोडेल हो जसमा Development का चरणहरूसँग सम्बन्धित Testing चरणहरूलाई योजनाबद्ध रूपमा जोडिन्छ।

```text
Requirement Analysis  <----------------> Acceptance Testing
       System Design  <----------------> System Testing
 Architecture Design  <----------------> Integration Testing
 Module/Detailed Design <---------------> Unit Testing
                    \                    /
                     \     Coding       /
```

यो सरलीकृत अवधारणात्मक चित्र हो। बायाँतर्फ Verification का विकास चरणहरू र दायाँतर्फ तिनसँग सम्बन्धित Validation Testing चरणहरू छन्।

### ५.१ V-Model का मुख्य Testing स्तरहरू

| Development चरण | सम्बन्धित Testing स्तर | के जाँचिन्छ? |
|---|---|---|
| Requirement Analysis | Acceptance Testing | प्रयोगकर्ताको आवश्यकता पूरा भयो? |
| System Design | System Testing | सम्पूर्ण प्रणालीले अपेक्षाअनुसार काम गर्छ? |
| Architecture / High-Level Design | Integration Testing | Module हरूबीचको सम्बन्ध सही छ? |
| Module / Low-Level Design | Unit Testing | सानो Function वा Component सही छ? |
| Coding | Implementation | डिजाइनअनुसार कोड निर्माण |

### ५.२ Verification र Validation बीचको सम्बन्ध

**Verification:** उत्पादन सही तरिकाले निर्माण हुँदै छ कि छैन भनेर Requirement, Design, Review र अन्य Work Products जाँच्ने प्रक्रिया।

उदाहरण: Login Requirement मा Password अनिवार्य हुनुपर्ने लेखिएको छ कि छैन भनेर Requirement Document Review गर्नु।

**Validation:** वास्तविक सफ्टवेयरले प्रयोगकर्ताको आवश्यकता पूरा गर्छ कि गर्दैन भनेर मूल्याङ्कन गर्ने प्रक्रिया।

उदाहरण: Login Page मा खाली Password दिएर परीक्षण गर्दा प्रणालीले Login रोक्छ कि रोक्दैन भनेर जाँच्नु।

याद राख्ने सूत्र:

- Verification — *Are we building the product right?*
- Validation — *Are we building the right product?*

V-Model मा Testing को योजना सम्बन्धित Development चरणसँगै बनाइन्छ। तर सबै वास्तविक Testing Coding सुरु हुनुअघि नै गर्न सकिन्छ भन्ने होइन।

---

## ६. Agile/Scrum मा SDLC र STLC कसरी दोहोरिन्छन्?

Agile मा सफ्टवेयरलाई साना-साना Iteration वा Increment मा विकास गरिन्छ। Scrum मा यी कार्यहरू सामान्यतया Sprint भित्र सञ्चालन हुन्छन्।

उदाहरण: एउटा परियोजनामा पहिलो Sprint मा Login, दोस्रोमा User Profile र तेस्रोमा Online Application विकास गर्न सकिन्छ।

```text
Product Backlog
      ↓
Sprint Planning
      ↓
┌────────────────────────┬────────────────────────┐
│ SDLC                   │ STLC                   │
│ Design, Coding,        │ Test Design, Execution, │
│ Integration            │ Defect Fix, Regression  │
└────────────────────────┴────────────────────────┘
      ↓
Working Increment
      ↓
Review → Feedback → Backlog Update → अर्को Sprint
```

### ६.१ Agile मा SDLC का गतिविधि

- User Story तथा Acceptance Criteria तयार गर्ने।
- Sprint Planning गर्ने।
- UI तथा System Design गर्ने।
- Coding र Code Review गर्ने।
- Integration र आवश्यक Documentation गर्ने।
- Increment तयार गरी Review गर्ने।

### ६.२ Agile मा STLC का गतिविधि

- User Story र Acceptance Criteria Review गर्ने।
- Test Scenarios तथा Test Cases बनाउने।
- आवश्यक Test Data तथा Environment तयार गर्ने।
- Unit, Integration र Functional Tests सञ्चालन गर्ने।
- Regression तथा Automation Tests चलाउने।
- Defects समाधानपछि Retest गर्ने।
- Definition of Done पूरा भए/नभएको जाँच गर्ने।

### ६.३ Definition of Done (DoD) भनेको के हो?

Definition of Done भनेको कुनै User Story वा Increment लाई पूरा भएको मान्न आवश्यक सहमत मापदण्डहरूको सूची हो।

उदाहरण:

- आवश्यक Functionality पूरा भएको।
- Code Review सम्पन्न भएको।
- आवश्यक Automated Tests पास भएको।
- स्वीकृत Acceptance Criteria पूरा भएको।
- गम्भीर Defect बाँकी नभएको, वा सहमत नीतिअनुसार व्यवस्थापन भएको।
- आवश्यक Documentation अद्यावधिक भएको।

DoD प्रत्येक टोलीको परियोजना र गुणस्तर नीतिअनुसार फरक हुन सक्छ।

### ६.४ Agile र Waterfall बीच Testing को मुख्य भिन्नता

| Waterfall | Agile/Scrum |
|---|---|
| चरणहरू प्रायः क्रमिक हुन्छन् | काम Iteration/Sprint मा दोहोरिन्छ |
| Testing को मुख्य Execution पछिल्लो चरणमा केन्द्रित हुन सक्छ | Testing प्रत्येक Increment सँगै हुन्छ |
| परिवर्तनले धेरै चरण प्रभावित पार्न सक्छ | Feedback अनुसार साना परिवर्तन समावेश गर्न सकिन्छ |
| Documentation र चरणगत Approval मा जोड हुन सक्छ | Working Software र निरन्तर Feedback मा जोड हुन्छ |
| Regression Testing Release अनुसार हुन सक्छ | Regression Tests बारम्बार चलाइन्छ |

Agile मा पनि Documentation, Planning र Approval आवश्यक पर्न सक्छन्; ती हटाइन्छन् भन्ने होइन।

---

## ७. Login System को उदाहरणबाट SDLC र STLC बुझ्ने

अब एउटा वास्तविक Web Application को Login System बनाएर दुवै जीवनचक्र कसरी प्रयोग हुन्छन् हेरौँ।

### ७.१ SDLC अनुसार Login System विकास

| SDLC चरण | गरिने काम |
|---|---|
| Planning | Login सुविधा किन चाहिन्छ र यसको Scope के हो तय गर्ने |
| Requirement Analysis | Username, Password, Account Status र Role सम्बन्धी नियम निर्धारण गर्ने |
| Design | Login UI, API, Database, Session तथा Authorization Design गर्ने |
| Development | Frontend Form, Backend API र Database Logic बनाउने |
| Testing | Login का सबै आवश्यक व्यवहार परीक्षण गर्ने |
| Deployment | Login System Production मा उपलब्ध गराउने |
| Maintenance | Login सम्बन्धी Bug Fix, Security Update र नयाँ सुविधा थप्ने |

### ७.२ STLC अनुसार Login System परीक्षण

**Requirement Analysis:** Login का नियमहरू अध्ययन गर्ने।

उदाहरण:
- सही Credentials भए Login सफल हुनुपर्छ।
- गलत Password भए Login असफल हुनुपर्छ।
- निष्क्रिय Account ले Login गर्न पाउनु हुँदैन।
- प्रयोगकर्ताले आफ्नो अधिकार नभएको Dashboard खोल्न पाउनु हुँदैन।

**Test Planning:** कुन प्रकारको परीक्षण गर्ने, कसले गर्ने, कुन Environment प्रयोग गर्ने र कुन जोखिमलाई प्राथमिकता दिने भन्ने तय गर्ने।

**Test Case Design:** प्रत्येक Requirement का लागि परीक्षण अवस्था र अपेक्षित नतिजा तयार गर्ने।

**Test Environment Setup:** Application, Database, Test Accounts र आवश्यक Configuration तयार गर्ने।

**Test Execution:** Test Cases चलाएर Actual Result र Expected Result तुलना गर्ने।

**Defect Management:** त्रुटि भेटिएमा रिपोर्ट गर्ने, Developer बाट Fix भएपछि Retest गर्ने र Regression Testing गर्ने।

**Test Closure:** परीक्षणको नतिजा, बाँकी Defects, जोखिम र Coverage को सारांश तयार गर्ने।

### ७.३ Login System का नमुना Test Cases

| Test ID | Test Scenario | Input | Expected Result |
|---|---|---|---|
| TC-01 | सही Credentials | सही Username र Password | Login सफल |
| TC-02 | गलत Password | सही Username, गलत Password | Login असफल |
| TC-03 | गलत Username | गलत Username, सही Password | Login असफल |
| TC-04 | खाली Field | Username वा Password खाली | Validation Message |
| TC-05 | निष्क्रिय Account | निष्क्रिय प्रयोगकर्ताको Credentials | Login अस्वीकार |
| TC-06 | Role Access | सामान्य User बाट Admin Dashboard खोल्ने प्रयास | Access अस्वीकार |
| TC-07 | Session Handling | Logout पछि सुरक्षित पृष्ठ खोल्ने प्रयास | पुनः प्रमाणीकरण आवश्यक |
| TC-08 | SQL Injection प्रयास | Input मा SQL-जस्तो Malicious Payload | सुरक्षित रूपमा अस्वीकार; अनधिकृत Access नहुने |

यी नमुना Test Cases हुन्। वास्तविक Expected Result भने स्वीकृत Requirements र Security Policy अनुसार परिभाषित गर्नुपर्छ।

### ७.४ एउटा Test Case को विस्तृत नमुना

**Test Case ID:** TC-01 — Valid Login

- **Test Objective:** सही Credentials प्रयोग गर्दा प्रयोगकर्ता Login हुन सक्छ कि सक्दैन जाँच्ने।
- **Precondition:** प्रयोगकर्ताको Account सक्रिय छ र Test Environment उपलब्ध छ।
- **Test Steps:**
  1. Login Page खोल्ने।
  2. मान्य Username प्रविष्ट गर्ने।
  3. मान्य Password प्रविष्ट गर्ने।
  4. Login Button थिच्ने।
- **Expected Result:** प्रयोगकर्ता प्रमाणित हुन्छ, उपयुक्त Dashboard खुल्छ र सुरक्षित Session स्थापित हुन्छ।
- **Actual Result:** Testing चलाएपछि वास्तविक परिणाम लेख्ने।
- **Status:** Actual Result अपेक्षित नतिजासँग मिलेमा PASS, नमिलेमा FAIL।

### ७.५ Defect भेटिएपछि के हुन्छ?

उदाहरण: TC-06 मा सामान्य User ले Admin Dashboard खोल्न सकेको छ।

1. Tester ले Defect Report गर्छ।
2. Defect मा Steps to Reproduce, Expected Result, Actual Result, Environment र आवश्यक प्रमाण समावेश गर्छ।
3. Developer ले कारण पत्ता लगाएर Authorization Logic सुधार्छ।
4. Tester ले सोही Test Case पुनः चलाउँछ — यसलाई **Retesting** भनिन्छ।
5. सुधारले अन्य सुविधामा असर पारेको छ कि छैन जाँचिन्छ — यसलाई **Regression Testing** भनिन्छ।
6. आवश्यक परीक्षण पूरा भएपछि मात्र सम्बन्धित Defect बन्द गरिन्छ।

यही Feedback Loop ले SDLC र STLC लाई जोड्छ।

---

## ८. SDLC र STLC मा थप बुझ्नुपर्ने महत्त्वपूर्ण विषयहरू

### ८.१ Entry Criteria र Exit Criteria

**Entry Criteria:** कुनै चरण वा Testing Activity सुरु गर्न आवश्यक न्यूनतम सर्तहरू।

उदाहरण:
- Test Environment उपलब्ध हुनु।
- परीक्षण गर्नुपर्ने Build Deploy भएको हुनु।
- आवश्यक Test Data उपलब्ध हुनु।
- आवश्यकताहरू पर्याप्त रूपमा स्पष्ट हुनु।

**Exit Criteria:** कुनै चरण पूरा भएको मान्न आवश्यक सर्तहरू।

उदाहरण:
- निर्धारित Test Cases को Execution पूरा हुनु।
- महत्त्वपूर्ण Defects को अवस्था मूल्याङ्कन हुनु।
- आवश्यक Regression Tests चलाइनु।
- बाँकी जोखिम र सीमाहरू अभिलेख हुनु।

सबै परियोजनामा शतप्रतिशत Test Cases पास हुनैपर्छ भन्ने सार्वभौमिक नियम हुँदैन। Release Criteria परियोजनाको जोखिम, आवश्यकताहरू र स्वीकृत नीतिअनुसार तय गरिन्छ।

### ८.२ Requirement Traceability Matrix (RTM)

RTM ले Requirements र तिनलाई परीक्षण गर्ने Test Cases बीचको सम्बन्ध देखाउँछ।

| Requirement ID | Requirement | Test Case ID | Status |
|---|---|---|---|
| REQ-01 | Valid Login | TC-01 | Pass |
| REQ-02 | Invalid Password रोक्ने | TC-02 | Pass |
| REQ-03 | Inactive Account रोक्ने | TC-05 | Fail |
| REQ-04 | Role-based Access | TC-06 | Not Run |

यसको उपयोग:
- कुन Requirement परीक्षण भयो भनेर बुझ्न।
- छुटेका Requirements पत्ता लगाउन।
- परिवर्तन हुँदा प्रभावित Test Cases पहिचान गर्न।
- Requirement Coverage मूल्याङ्कन गर्न।

### ८.३ Test Coverage र Test Metrics

**Test Coverage** ले परिभाषित Scope भित्रका आवश्यकताहरू, Statements, Branches वा अन्य परीक्षणयोग्य पक्षमध्ये कति समेटिए भन्ने देखाउँछ।

Requirement Coverage को सरल उदाहरण:

\[
\text{Requirement Coverage}=
\frac{\text{Test गरिएका Requirements}}{\text{कुल Testable Requirements}}\times100
\]

यदि ५० वटा Requirements मध्ये ४५ वटाको परीक्षण भएको छ भने Requirement Coverage ९०% हुन्छ।

तर **९०% Coverage हुनुको अर्थ सफ्टवेयर ९०% Bug-free छ भन्ने होइन।** Coverage ले परीक्षणको दायरा देखाउँछ; परीक्षणको गहिराइ वा बाँकी सबै जोखिमको पूर्ण मापन गर्दैन।

अन्य उपयोगी Metrics:
- Test Execution Rate
- Test Pass Rate
- Defect Density
- Defect Leakage
- Defect Reopen Rate
- Automation Coverage
- Mean Time to Resolve Defects

### ८.४ Defect Life Cycle

Defect Report भएपछि त्यसको अवस्था परिवर्तन हुँदै जान्छ।

```text
New / Open
     ↓
Assigned / In Progress
     ↓
Fixed / Ready for Retest
     ↓
Retest
  ↙     ↘
Pass     Fail
 ↓        ↓
Closed   Reopen
```

यो एउटा सामान्य Workflow हो। वास्तविक Defect Tracking System मा Rejected, Duplicate, Deferred, Cannot Reproduce जस्ता थप Status हुन सक्छन्।

### ८.५ Severity र Priority

- **Severity:** Defect ले प्रणालीमा कति गम्भीर असर पार्छ?
- **Priority:** Defect लाई कति छिटो समाधान गर्नुपर्छ?

उदाहरण: सबै प्रयोगकर्ताले Login गर्न नसक्ने समस्या उच्च Severity र उच्च Priority हुन सक्छ। तर सानो पृष्ठमा देखिएको Logo Alignment समस्या सामान्यतया कम Severity को हुन सक्छ, यद्यपि कुनै महत्त्वपूर्ण सरकारी वा कानुनी पृष्ठमा गलत Logo हुनु उच्च Priority हुन सक्छ।

### ८.६ Testing र Quality Assurance बीचको भिन्नता

**QA (Quality Assurance):** प्रक्रिया सुधार र Defects रोक्न केन्द्रित गतिविधिहरू।

**QC (Quality Control):** उत्पादनको गुणस्तर जाँच्ने गतिविधिहरू।

**Testing:** सफ्टवेयरको व्यवहार मूल्याङ्कन गरी Defects वा असंगतिहरू पत्ता लगाउने प्रमुख गतिविधि।

त्यसैले QA केवल Testing मात्र होइन। Requirement Review, Process Improvement, Test Planning, Test Execution र Defect Analysis सबैले गुणस्तर सुधारमा योगदान दिन सक्छन्।

### ८.७ Release Readiness र Test Closure

Testing समाप्त भएपछि Release गर्ने वा नगर्ने निर्णय गर्दा निम्न पक्ष हेर्नुपर्छ:

- स्वीकृत Release Criteria पूरा भए/नभएको।
- Critical र High Severity Defects को अवस्था।
- मुख्य Business Flows को परीक्षण परिणाम।
- Security र Performance सम्बन्धी जोखिम।
- बाँकी Defects का Workarounds तथा प्रभाव।
- Regression तथा Smoke Testing को नतिजा।
- आवश्यक Stakeholder Approval।

Test Closure ले परीक्षणको निष्कर्ष अभिलेख गर्छ; यसले आफैँमा Release Approval को ग्यारेन्टी दिँदैन।

---

## ९. SDLC र STLC सम्बन्धी महत्त्वपूर्ण Interview Questions and Answers

### Q1. What is SDLC?

**Answer:** SDLC stands for Software Development Life Cycle. It is a structured process used to plan, analyze, design, develop, test, deploy, and maintain software.

नेपालीमा: सफ्टवेयरलाई योजनादेखि Maintenance सम्म व्यवस्थित रूपमा विकास र सञ्चालन गर्ने प्रक्रिया SDLC हो।

### Q2. What is STLC?

**Answer:** STLC stands for Software Testing Life Cycle. It is a systematic process of analyzing requirements, planning tests, designing test cases, preparing the test environment, executing tests, managing defects, and closing testing activities.

### Q3. What is the main difference between SDLC and STLC?

**Answer:** SDLC covers the overall software lifecycle, whereas STLC focuses on systematic software testing activities within that lifecycle.

### Q4. Does STLC start only after coding is completed?

**Answer:** No. Testing-related activities can begin during the requirement analysis and design phases. Test execution that requires a working build may occur later.

### Q5. What is Shift-left Testing?

**Answer:** Shift-left Testing means introducing testing activities earlier in the software development process to identify defects sooner and reduce rework and risk.

### Q6. What is the relationship between SDLC and STLC?

**Answer:** STLC works in coordination with SDLC. Requirements, design, coding, testing and maintenance activities provide inputs for corresponding testing activities and feedback.

### Q7. What is the V-Model?

**Answer:** The V-Model is an SDLC model that associates development stages with corresponding testing levels, such as requirements with acceptance testing and detailed design with unit testing.

### Q8. How does testing work in Agile?

**Answer:** In Agile, development and testing activities are performed iteratively. Testing, feedback, defect fixing and regression testing occur throughout successive iterations or Sprints.

### Q9. What is the difference between Retesting and Regression Testing?

**Answer:**
- **Retesting:** Re-executing a failed test after the relevant defect has been fixed.
- **Regression Testing:** Checking whether a change has adversely affected previously working functionality.

### Q10. What are Entry and Exit Criteria?

**Answer:** Entry Criteria define the conditions required to begin a phase or activity. Exit Criteria define the conditions required to consider that phase or activity complete.

### Q11. What is RTM?

**Answer:** RTM stands for Requirement Traceability Matrix. It maps requirements to corresponding test cases and helps identify missing test coverage.

### Q12. Can 100% testing guarantee bug-free software?

**Answer:** No. Exhaustive testing is generally impractical for complex software. Testing reduces uncertainty and risk but cannot guarantee that every defect has been found.

### Q13. What is the difference between Verification and Validation?

**Answer:** Verification checks whether work products conform to specified requirements and design. Validation evaluates whether the resulting software meets user needs and intended use.

### Q14. What is Test Closure?

**Answer:** Test Closure is the activity of reviewing and documenting testing results, coverage, defect status, unresolved risks, lessons learned and relevant metrics.

### Q15. Who is responsible for software quality?

**Answer:** Software quality is a shared responsibility involving developers, QA professionals, analysts, product owners and other stakeholders. QA does not own quality alone.

---

## १०. परीक्षाका लागि Short Notes

### SDLC (Software Development Life Cycle)

सफ्टवेयरको योजना, Requirement Analysis, Design, Development, Testing, Deployment र Maintenance समेट्ने समग्र प्रक्रिया।

### STLC (Software Testing Life Cycle)

Requirement Analysis, Test Planning, Test Design, Environment Setup, Test Execution, Defect Management र Test Closure समेट्ने परीक्षण प्रक्रिया।

### Shift-left Testing

विकासको प्रारम्भिक चरणमै Testing गतिविधि सुरु गरी Defects छिटो पत्ता लगाउने दृष्टिकोण।

### V-Model

Development का चरण र तिनसँग सम्बन्धित Testing Levels लाई जोडी विकास तथा परीक्षण योजना बनाउने मोडेल।

### Agile Testing

प्रत्येक Iteration वा Sprint मा विकाससँगै परीक्षण, Feedback र सुधार दोहोरिने दृष्टिकोण।

### RTM

Requirements र Test Cases बीचको सम्बन्ध अभिलेख गर्ने Matrix।

### Retesting

Fix गरिएको Defect सम्बन्धित Test Case पुनः चलाएर सुधार पुष्टि गर्ने प्रक्रिया।

### Regression Testing

Code परिवर्तनपछि पहिले काम गरिरहेका सुविधाहरूमा नयाँ समस्या आएको छ कि छैन जाँच्ने प्रक्रिया।

### Test Closure

परीक्षणको नतिजा, Defects, Coverage र बाँकी जोखिमको समीक्षा गरी अभिलेख तयार गर्ने चरण।

---

## ११. SDLC र STLC को Quick Revision

| प्रश्न | उत्तर |
|---|---|
| SDLC को पूरा रूप के हो? | Software Development Life Cycle |
| STLC को पूरा रूप के हो? | Software Testing Life Cycle |
| SDLC को मुख्य उद्देश्य के हो? | सफ्टवेयरको योजना, विकास, Deployment र Maintenance व्यवस्थित गर्नु। |
| STLC को मुख्य उद्देश्य के हो? | Testing गतिविधिहरू व्यवस्थित गरी गुणस्तर मूल्याङ्कन र Defects पहिचान गर्नु। |
| QA ले कहिलेदेखि काम सुरु गर्न सक्छ? | Requirement Analysis तथा Design चरणदेखि नै। |
| V-Model को विशेषता के हो? | Development चरणलाई सम्बन्धित Testing Levels सँग जोड्नु। |
| Agile मा Testing कहिले हुन्छ? | हरेक Iteration वा Sprint मा आवश्यकतानुसार निरन्तर हुन्छ। |
| RTM को काम के हो? | Requirements र Test Cases बीच Traceability कायम गर्नु। |
| Retesting र Regression Testing मा के फरक छ? | Retesting ले Fix पुष्टि गर्छ; Regression ले परिवर्तनबाट अन्य सुविधा बिग्रिएको छ कि छैन जाँच्छ। |
| Testing ले सबै Bug हटेको ग्यारेन्टी दिन्छ? | दिँदैन; Testing ले Defects र जोखिम पहिचान गर्न मद्दत गर्छ। |

---

## १२. SDLC र STLC सम्झिने सजिलो तरिका

### SDLC — Software बनाउने प्रक्रिया

**Plan → Requirements → Design → Code → Test → Deploy → Maintain**

मुख्य ध्यान: सफ्टवेयर निर्माण र सञ्चालन।

### STLC — Software परीक्षण प्रक्रिया

**Analyze → Plan → Design Tests → Setup → Execute → Close**

मुख्य ध्यान: परीक्षण योजना, परीक्षणको कार्यान्वयन र परिणाम।

### दुवैको सम्बन्ध

**Develop + Test + Feedback + Improve**

Testing ले समस्या पत्ता लगाउँछ, Development ले सुधार गर्छ र पुनः परीक्षणले सुधारको प्रभाव जाँच्छ।

---

## १३. निष्कर्ष

SDLC र STLC सफ्टवेयर विकास तथा गुणस्तर व्यवस्थापनका परस्पर सम्बन्धित प्रक्रिया हुन्। SDLC ले सफ्टवेयरको समग्र जीवनचक्र समेट्छ भने STLC ले Testing गतिविधिहरूलाई व्यवस्थित बनाउँछ।

गुणस्तरीय सफ्टवेयर बनाउन Testing लाई Coding पछिको अन्तिम कामका रूपमा मात्र हेर्नु हुँदैन। Requirement Analysis देखि Design, Development, Deployment र Maintenance सम्म QA तथा Testing को उपयुक्त सहभागिता आवश्यक हुन्छ।
