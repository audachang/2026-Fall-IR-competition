# Eight field-based topics for the 2026 AI 校務治理實務競賽

[中文版](2026_AI_IR_Competition_Topics_ZH.md) · [Course home](../README.md#english)

Prepared: 2026-09-15. English explanations with proposed Chinese competition titles. English topic titles are descriptive translations.

## Recommendation

Prioritize **unmet course demand** for a quantitative IR project, **SDG-label evidence checking** for a bounded text-analysis project, or **multilingual course discovery** for a student-facing application. **Research-to-classroom matching** offers a more exploratory alternative. Keep **IR research-design checking** as the fallback if analytical data are delayed.

These are design judgments based on the supplied field catalog, not findings about NCU or predictions of competition success. Creativity here means a specific improvement to a university decision or task; it is not a claim that no similar tool exists elsewhere.

### Evidence and timing

- The supplied workbook contains **36 worksheets: a cover, an index, and 34 dataset field lists containing 626 field entries**. All populated cells were read. This differs in scope from the older 60-item platform inventory; this brief uses the workbook as its primary data boundary.
- The workbook lists fields, not analytical records. It does not establish delivered records, usable sample sizes, year coverage, completeness, definitions, or permission for cross-table linkage. Feasibility below is conditional on these checks.
- The current [official announcement](https://ir.ncu.edu.tw/p/406-1034-216,r11.php?Lang=zh-tw) and [guidelines revised September 10, 2026](https://ir.ncu.edu.tw/static/file/34/1034/img/429/602589443.pdf), checked September 15, list registration by **September 23** and submission by **November 11 at 23:59**. The guidelines require the report, a demo video of no more than four minutes, slides, and an A0 poster. The final is November 27. The older local syllabus lists November 16 for the report; use the currently verified November 11 deadline for project planning.
- The guidelines evaluate importance, innovation, empirical evidence, and feasibility at 25% each. Category assignments below are recommendations, not organizer-approved classifications.

## Shortlist

| No. | Proposed topic | Concrete decision or task | Field-based feasibility | Suggested category |
| --- | --- | --- | --- | --- |
| 1 | Unmet course demand and allocation bottlenecks | Which courses warrant closer capacity or allocation review? | Moderate; allocation-event definitions are essential | Resilient and sustainable governance (韌性永續治理) |
| 2 | Checking the evidence behind course SDG labels | Which course labels have textual support, and which need clarification? | Strong if course-goal text is populated; one core dataset | Resilient and sustainable governance (韌性永續治理) |
| 3 | Multilingual course discovery with explicit limitations | Can students find relevant courses and understand what is still unconfirmed? | Strong if usable course descriptions are delivered | Borderless campus services (無國界校園服務) |
| 4 | From UCAN development goals to course evidence | Which courses contain evidence relevant to a student's chosen development goal? | Moderate; competency definitions and mapping need human review | Smart learning guidance (智慧學習引導) |
| 5 | Bringing NCU research into the classroom | Which local research examples could enrich an existing course? | Moderate; needs usable abstracts and course goals | Smart research and development support (智慧研發支持) |
| 6 | Comparing graduate outcomes responsibly | Which graduate-outcome comparisons are meaningful and which are misleading? | Moderate; aggregate definitions and comparison keys are essential | Smart institutional research (智慧校務研究) |
| 7 | Supporting the first semester after return from leave | What academic support may returning students need? | Conditional; longitudinal version needs approved student linkage | Smart learning guidance (智慧學習引導) |
| 8 | Checking whether an IR research proposal is feasible | Does a proposed research question have the necessary fields and linkage? | Lowest dependence on new records; catalog use still must be permitted | Smart institutional research (智慧校務研究) |

“Strong” means comparatively few missing data dependencies, not that access or successful implementation has been confirmed. Keep each team to one topic and one primary workflow.

## 1. Unmet course demand and allocation bottlenecks

**Proposed Chinese title:** 想修卻修不到：跨系選課需求與分發瓶頸 AI 助理

**Question.** Which courses show persistent unmet high-priority demand, and does access differ between students inside and outside the offering department?

**User and prototype.** An opening-unit or curriculum committee member selects a course group and semester. The tool shows distinct applicants, preference ranks, allocation outcomes, and repeated unsuccessful attempts. AI turns a natural-language question into a supported query and explains the computed result with its denominator. It can prepare a review brief comparing “retain current provision” and explicitly assumed capacity changes.

**Workbook evidence.** `選課分發歷程!B2:B14`: 分發代碼、學期別、課號、學號、志願序、選課的結果、學生所屬系所、學生年級、結束的分發時間. `開課資料!B9:B21` and `B35:B36`: course identity, opening department, status, level, and term.

**Minimum study.** One course group over two comparable completed semesters, if available. Start with descriptive demand and allocation analysis. A possible indicator is the proportion of distinct first-choice applicants with no successful allocation after the defined rounds; use it only after confirming how preferences and results operate. This measures allocation outcomes, not final enrollment or hidden demand from students who never applied.

**Distinctive contribution.** Separates repeated applications from distinct unmet demand and lets administrators trace a bottleneck claim back to its events. The AI interaction makes an auditable analysis easier to use.

**Validation.** Compare manual spreadsheet answers, a fixed dashboard, and the AI interface on the same held-out administrative questions. Check numerical agreement, denominator selection, unsupported claims, and task time. If multiple historical semesters support forecasting, compare against the previous comparable semester before adding a complex model.

**Critical gaps and fallback.** Confirm whether 分發代碼 identifies a round, result-code meaning, stable pseudonymous student IDs, and the mapping from 課號 to course-offering keys. The workbook does not list seats, priority rules, actual timetable constraints, or budget. Do not claim an optimal allocation or feasible extra class without them. A fallback is a data-custodian-produced table of deduplicated demand and outcomes by course, term, and student department.

## 2. Checking the evidence behind course SDG labels

**Proposed Chinese title:** SDGs 標籤有根據嗎？課程永續證據檢核 AI

**Question.** Can AI identify the passages supporting a course's assigned SDG labels and distinguish insufficient description from a potentially questionable label?

**User and prototype.** A curriculum reviewer sees the recorded label, the supporting course-goal passage, and an explanation. The system returns “text supports review,” “text insufficient,” or “possible mismatch for human review.” It proposes a clarification request when the description is too thin.

**Workbook evidence.** `開課資料!B9:B16`: course name, department, evaluation weighting, teaching language, course code, and goals. `B31:B35`: grading description, SDG goals/codes, and term. The core is 課程目標 plus SDGs目標／代碼; evaluation descriptions are supplementary only if their delivered values are informative.

**Minimum study.** One faculty and a proposed sample of 60–100 course offerings, adjusted to the actual population. Use an authoritative SDG definition set, document the rubric, and have two reviewers independently label a subset. Split repeated versions of the same course together to avoid nearly identical descriptions appearing in training and testing.

**Distinctive contribution.** Tests the evidence for administrative labels instead of merely assigning more labels. Separating missing evidence from incorrect labeling makes the output actionable without treating short descriptions as proof of poor teaching.

**Validation.** Compare a keyword baseline, an unconstrained AI classifier, and evidence-required classification. Measure per-label precision/recall, agreement with adjudicated reviewers, quoted-passage accuracy, abstention behavior, and review time. Existing SDG labels are comparison data, not automatic ground truth.

**Critical gaps and fallback.** Need populated goal text, SDG definitions, and reviewers. Restrict the project to catalog-description quality: course text does not establish actual SDG learning, behavior change, or carbon reduction. If descriptions are unavailable, a small authorized public course-description collection can test the workflow; disclose the narrower coverage.

## 3. Multilingual course discovery with explicit limitations

**Proposed Chinese title:** 找得到，也讀得懂：多語課程探索與限制說明 AI

**Question.** Can Chinese and English queries retrieve relevant course options while accurately preserving teaching-language, term, and program information?

**User and prototype.** A student describes a learning goal in either language. The tool returns a short list with translated goal excerpts, teaching language, program association, and opening status. It separately identifies unresolved eligibility, prerequisites, scheduling, and credit-recognition questions.

**Workbook evidence.** `開課資料!B9:B21`, `B35:B44`: 課程名稱、授課語言、課程目標、開課狀態、開課學程名稱、開課年級、學年學期、課程流水號、學分學程名稱／代碼、合開專業學程、所屬學制名稱.

**Minimum study.** One program or faculty; Chinese and English only. Prepare approximately 30 paired search tasks, including requests for unavailable courses or unsupported eligibility claims. A historical catalog can validate retrieval, but current enrollment advice requires a current offering list and applicable rules.

**Distinctive contribution.** Tests whether the same intent produces comparably useful results across languages, including accurate explanations of missing information. It goes beyond translating course names.

**Validation.** Compare keyword/filter search, ordinary AI answers, and the grounded tool. Score relevant results in the top five, teaching-language accuracy, unsupported eligibility claims, translation fidelity, completion rate, and task time. Use bilingual reviewers and counterbalance task order in user testing.

**Critical gaps and fallback.** The workbook has no explicit prerequisite, quota, weekday/period, classroom, or degree-rule fields. Add verified rules only for a narrowly defined program; until then call this course discovery, not an enrollment-ready schedule or degree audit. Public authorized course descriptions can support a smaller fallback dataset.

## 4. From UCAN development goals to course evidence

**Proposed Chinese title:** 從能力養成計畫到選課：UCAN 課程證據導航

**Question.** Can a student turn a selected competency-development goal into course options whose stated goals provide relevant evidence?

**User and prototype.** A student or career adviser selects a goal such as problem solving or communication. AI retrieves course-goal passages and explains the match and its limits. Suggestions include adjacent interests rather than forcing the student into one occupational profile.

**Workbook evidence.** `_x0009_UCAN職場共通職能診斷資料!B2:B25`: raw scores, PR values, 前測/後測、勾選的能力養成計畫、診斷學期年. `UCAN專業職能診斷!B7:B14`: 是否列入養成計畫、就業途徑分數、能力面向分數、就業途徑、能力面向、職涯類型. `開課資料!B9:B16` and `B35:B44` supply course text and program context. The unusual `_x0009_` prefix is part of the actual worksheet name.

**Minimum study.** Three competency areas and one course collection. Start with participant-entered goals and reviewed competency definitions; historical UCAN-to-course linkage is unnecessary for the retrieval prototype. If aggregate UCAN data arrive, use them to prioritize which competency goals to support, not to infer individual deficits.

**Distinctive contribution.** Connects an existing development-plan step to specific course evidence. Every recommendation answers “what in this course supports the match?”

**Validation.** Compare department-only recommendations and keyword matching with AI semantic matching. Have advisers rate relevance and unsupported promises; test whether students can explain why an option was suggested. Hold out reviewed matches from development.

**Critical gaps and fallback.** Need authoritative competency definitions and the meaning of the UCAN measures. A listed 前測/後測 field does not prove paired observations. Claims about competency growth require matched observations, comparable measurement, and a suitable design. Do not treat PR values as interval-scale growth or claim the courses cause better employment. The participant-entered-goal version is the fallback.

## 5. Bringing NCU research into the classroom

**Proposed Chinese title:** 研究走進課堂：中大研究成果與課程 AI 配對

**Question.** Which NCU publications provide useful local examples for a course's stated learning goals?

**User and prototype.** An instructor selects a course. AI retrieves relevant publication abstracts, explains the conceptual connection, and drafts a short teaching-case outline with source excerpts and questions for the instructor to review.

**Workbook evidence.** `期刊論文著述!B4:B7` and `B13:B21`: affiliation, abstract, keywords, language, paper title, publication year, and SDG tags. `開課資料!B9:B16`, `B21`, `B35:B36`: course identity, goal, level, and term. These datasets can be compared semantically without linking individual students or faculty.

**Minimum study.** A proposed 20 courses and 50–100 usable abstracts within one or two related domains. Keep publication records deduplicated and preserve field-level provenance. Do not invent methods or findings that the abstract does not report.

**Distinctive contribution.** Gives research discovery a specific downstream use: helping teachers find local examples for existing learning goals. It can surface useful cross-department connections without asserting that people are available or willing to collaborate.

**Validation.** Compare same-department retrieval, keyword retrieval, and semantic matching. Instructors rate top-five relevance, level suitability, and factual accuracy of case outlines. Measure useful accepted matches and preparation time. Hold out course-publication matches from tuning.

**Critical gaps and fallback.** The publication sheet lists author order/count, not author names or a verified person ID. Do not turn this into named-expert matching without additional identity data. Abstracts may support discovery but not a complete teaching case; full text and reuse rights may be needed. Use an authorized public abstract collection if internal text is unavailable. Do not claim improved student learning without a separate classroom study.

## 6. Comparing graduate outcomes responsibly

**Proposed Chinese title:** 系所就業數字，怎麼比才合理？AI 比較與解讀助理

**Question.** Can AI help users compare graduate outcomes while detecting incompatible cohorts, salary years, denominators, and unsupported explanations?

**User and prototype.** A department reviewer asks a question such as “Did the employment picture improve?” The tool checks the comparison dimensions, runs deterministic calculations, and returns an evidence-linked explanation or requests the missing definition. It can display industry distribution alongside outcomes when the two tables align.

**Workbook evidence.** `中央大學畢業生就業相關情形分析結果!B2:B21`: 平均月薪、畢業生人數、畢業學年、有薪資所得、相對於全國學類平均差異比率、已投入職場比率、占可工作人口比率、月薪標準差、薪資年、學制別、可工作人數. `_x0009_中央大學畢業生就業流向人數統計!B2:B28` provides industries, unit identifiers, graduation year, salary year, degree type, 等級, and totals.

**Minimum study.** One unit and degree type, using only comparable delivered graduation cohorts and observation horizons. For trends, align years since graduation after confirming year definitions. Join candidate dimensions only after checking uniqueness and the meaning of 等級; resolve renamed units and suppressed cells.

**Distinctive contribution.** Makes “this comparison cannot support that conclusion” an observable tool capability. It can prevent an attractive chart from implying that a degree or course caused a salary difference.

**Validation.** Use analyst-adjudicated questions with valid and deliberately invalid comparisons. Compare manual analysis and ordinary AI with the constrained tool on numeric accuracy, valid-comparison decisions, unsupported causal statements, and task time.

**Critical gaps and fallback.** These fields suggest aggregate tables, not individual salaries. Confirm the salary population, the unit of 有薪資所得, and each ratio's denominator. Do not recompute salary standard errors from all graduates unless the actual salary-sample size is supplied. Do not infer individual outcomes or a course's salary return. If only one compatible table is delivered, build a single-table interpretation tool. Mock tables can test code but cannot establish NCU outcomes.

## 7. Supporting the first semester after return from leave

**Proposed Chinese title:** 重返校園的第一學期：復學支持需求與 AI 課程規劃

**Question.** What academic patterns occur in the first semester after return from leave, and can a bounded planning tool help returning students identify questions to discuss with an adviser?

**User and prototype.** A returning student and adviser review current course options and a checklist of curriculum changes or unresolved requirements. The research component describes return-to-study patterns; the tool helps prepare a conversation rather than assign a risk label.

**Workbook evidence.** `學生休學紀錄!B2:B9`: actual return term, actual leave duration, reasons, requested duration, leave term. `學生復學紀錄!B2:B8`: return term, approval result, application term. `學生學期平均成績!B2:B36`: semester and cumulative results, term, and result-completeness flags. `學生不及格警示資料!B2:B7`: failed credits, total attempted credits, warning category, and term. Course fields support the planning component.

**Minimum study.** A narrowly defined returning cohort with an observable post-return semester, plus a small adviser-reviewed planning prototype. Compare descriptive pre/post patterns and matched observation windows; keep planned return, actual return, approved application, leave, and deferred enrollment distinct.

**Distinctive contribution.** Studies a concrete transition and a support workflow. The meaningful outcome is the quality of the planning conversation and identification of missing information.

**Validation.** First audit event reconstruction and linkage. Evaluate the planning tool against a static checklist on factual accuracy, useful issues identified, and adviser/student task completion. Academic outcomes are exploratory unless a suitable intervention evaluation is added.

**Critical gaps and fallback.** Student IDs are not explicitly listed in several required sheets. This version requires approved, consistent pseudonymous linkage and historical records; do not match people from demographics. Need current curriculum rules and adequate cohort size. Exclude free-text leave reasons unless essential and authorized. If linkage is unavailable, reduce to aggregate return patterns and a participant-entered planning scenario; if even aggregates are delayed, choose another primary topic.

## 8. Checking whether an IR research proposal is feasible

**Proposed Chinese title:** 題目做不做得出來？IR 資料與研究設計 AI 檢核

**Question.** Can an AI assistant distinguish a supported research question from one missing essential variables, valid comparison units, or linkage?

**User and prototype.** A student enters a proposed project. The tool returns relevant dataset/field/cell references, an analysis unit, a conditional data-request draft, and a specific missing-data explanation. It separates “the field is listed” from “the records are available” and “the tables can be joined.”

**Workbook evidence.** All 34 field lists and `校務資料內容一覽!A1:D35`. The workbook's missing keys, inconsistent index/worksheet naming for student-status datasets, and lack of classroom/timetable fields provide useful real test cases.

**Minimum study.** A proposed 40–60 instructor-authored questions, with a held-out set that includes both feasible and infeasible proposals. Examples: course-language discovery; course-to-SDG text checking; individual course-to-salary effects; classroom walking distance versus grades; named-faculty matching from publications. Review the answer key independently of the model's generated responses.

**Distinctive contribution.** Evaluates research-design validity rather than only retrieving a dataset name. Success includes recognizing a missing linkage key, ecological inference, an outcome observed too late for prediction, or an absent core variable.

**Validation.** Compare manual Excel search, keyword retrieval, and the AI checker on field-citation accuracy, necessary-dataset coverage, correct gap identification, erroneous rejection of feasible questions, and review time. The answer key must not interpret absence from this workbook as proof of absence from the entire university.

**Critical gaps and fallback.** Catalog reuse and the model-processing environment must fit the permitted scope. No analytical records are needed to test catalog interpretation, but a catalog-only prototype cannot report actual NCU trends or numerical outcomes. This is the most robust fallback when record delivery is uncertain.

## What changes from the earlier broad directions

| Earlier direction or tempting claim | Field-based revision |
| --- | --- |
| General AI course navigation | Separate multilingual discovery (#3) from competency-goal matching (#4), with distinct users and tests. |
| Teaching-resource resilience | Focus #1 on observed allocation bottlenecks. Capacity, staffing cost, and timetable optimization remain additional-data extensions. |
| Research-expert matching | Use #5 for publication-to-course matching. Named-person matching is not established by the publication fields in this workbook. |
| Generic report summarization | Use #6 for a concrete reporting risk: invalid graduate-outcome comparisons. Aggregate salary fields do exist, but individual salary linkage is not established. |
| Broad IR data assistant | Make #8 demonstrate correct missing-data and research-design judgments, including deliberate failure cases. |
| Classroom walking distance and grades | Do not select as a primary project from this workbook: classroom, weekday/period, and route data are absent. |
| AI literacy improvement from programming courses | Programming flags and UCAN measures do not establish a validated AI-literacy outcome or a causal improvement. |

## Data request and delivery gates

For whichever topic is selected, request the smallest usable slice first. Dates below are proposed course milestones, not promises by the data custodian.

1. **By September 21:** settle the user, main question, one primary workflow, required fields, and fallback. Request actual period coverage and representative de-identified or aggregate records. Complete registration preparation for September 23.
2. **By October 1:** verify records, text completeness, code definitions, permitted processing, unique row meaning, linkage where needed, and displayable results. If a critical dependency fails, reduce scope or use #8.
3. **By October 15:** complete the baseline and a usable prototype. Freeze a held-out evaluation set before further tuning.
4. **By October 29:** complete the main comparison and error analysis. Small user studies should report participant/task counts and uncertainty; proposed sample sizes in this brief are practical starting points, not power calculations.
5. **By November 5:** freeze the evidence and prepare all four submission artifacts, allowing time before the November 11 deadline.

For text tools, numerical claims must come from verified calculations or stored source values. Compare the AI component against a simpler method that could solve the same task. For longitudinal analyses, keep the same person out of incompatible train/test splits and use only information available before any prediction date. An impressive interface does not substitute for these tests.

## Source register and completion boundary

Primary local source: `校務研究管理平台-各資料欄位名稱一覽表.xlsx` (course-provided workbook; not included in this repository). Worksheet names and cell ranges above were checked against the original workbook. Leading spaces in field labels are omitted for readability; unusual worksheet-name prefixes are retained where needed for lookup. The cover contains no populated cells in the extracted cell grid; graphical content was not used as evidence. Course participants can consult the [English field guide, which requires the course password](https://audachang.github.io/ir-competition/University_IR_Field_Catalog_EN.html).

The older [topic assessment](NCU_IR_Data_Inventory_and_Topic_Assessment_2026-09-09_EN.md) and current local [syllabus](../course-materials/SYLLABUS_EN.md) were read for continuity. Their historical portal observations are not treated as current access verification. No specific historical year range is assumed available in these proposals.

This brief provides eight research designs, not analyses of student, staff, publication, or employment records. No analytical records were obtained, no application was submitted, and no model or intervention was evaluated. The Chinese and English editions retain the same topics, evidence boundaries, and validation requirements. Publication of these proposals does not make the underlying records publicly available or authorize their redistribution.
