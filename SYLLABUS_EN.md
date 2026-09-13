# NS5119-* Independent Study: Institutional Research and Big Data Analytics

## Fall 2026 Syllabus — Academic Year 115, Semester 1

| Course Information | Details |
| --- | --- |
| Class time | Thursdays, 13:00–16:00 |
| Location | S5-601 |
| Teaching period | September 10–December 24, 2026; 16 weeks |
| Instructor | Erik Chang |
| Credits | 3 |
| Contact and office hours | By appointment |
| Course format | Independent study, project work, literature discussions, and oral defenses |
| Course website | <https://github.com/audachang/2026-Fall-IR-competition> |
| Source version | September 10, 2026; the teaching schedule and grading weights will be announced after confirmation by the instructor |

*English translation of [the Chinese syllabus](SYLLABUS.md), prepared September 13, 2026. Course requirements, dates, and source-check dates are retained from that version. English translations of competition categories and Chinese source titles are descriptive, not verified official English names.*

[English course information and supporting documents](README.md#english)

## 1. Course Overview

This course investigates institutional issues at National Central University (NCU) through data analysis and artificial intelligence. Students will complete a research project with a clearly defined question, traceable evidence, and actionable recommendations. Starting with the existing institutional research (IR) data catalog and past competition cases, students will select a topic, apply for data access, design a study, prepare data, conduct analyses, and evaluate an application. The “2026 AI Applications for University Governance Competition” (2026 AI校務治理實務競賽) serves as an intermediate venue for presenting project outcomes.

In line with the 2026 competition themes, the course connects data analysis to practical AI applications for university operations: report checking, interdisciplinary learning navigation, research expertise matching, teaching resource scenario analysis, and IR data discovery. Each team must select a specific task, support its design with research evidence, and evaluate the prototype’s accuracy and usefulness against a baseline. Governance recommendations must explain the conditions for adoption and the procedures for human review.

Students may work individually or in teams, with supervision tailored to their progress. Every student must make an identifiable contribution and be able to explain the research methods and findings independently.

## 2. Learning Objectives

By the end of the course, students should be able to:

1. Turn an institutional issue into a researchable question and identify the intended decision-makers, study population, unit of analysis, and outcome indicators.
2. Distinguish between data catalogs, fields listed for data requests, and actual datasets; plan data access, permitted uses, and alternatives.
3. Build reproducible workflows for data cleaning, linkage, analysis, and visualization, checking missing values, duplicates, time definitions, and classification definitions.
4. Select appropriate statistical or machine learning methods and distinguish description, association, prediction, and causal inference.
5. Implement an AI application relevant to an institutional issue and evaluate its benefits using baselines, held-out test cases, and error analysis.
6. Present evidence in reports, slides, and posters, and make recommendations that specify implementation conditions, human review, and outcome monitoring.

## 3. Research Data and Project Selection

### Data Foundation

The course data inventory reviewed 60 data catalog entries and their request-field pages on September 9, 2026: 38 datasets transferred from university administrative systems and 22 Ministry of Education university database reports. **These are confirmed items for which access may be requested, not datasets already obtained for analysis.** Record counts, complete year coverage, field definitions, anonymous linkage identifiers, and actual usage permissions must be confirmed after approval and delivery.[1][2]

Areas with relatively stronger catalog and field coverage include course offerings, course registration allocation, individual course grades, semester grades, student affiliations, UCAN career interests and competencies, and aggregate records of programming and interdisciplinary course participation. Core data such as individual salary follow-up, employer satisfaction, and course classrooms and scheduled periods were not confirmed in this inventory and must not be assumed to be available.

### Competition Themes and Topic Selection Principles

The 2026 competition focuses on practical AI applications for university governance. Its seven official categories are **AI Transformation of University Operations (校務ＡＩ轉型), Resilient and Sustainable Governance (韌性永續治理), Intelligent Learning Guidance (智慧學習引導), Intelligent Research and Development Support (智慧研發支持), Intelligent Institutional Research (智慧校務研究), NCU Brand Management (中大品牌經營), and Borderless Campus Services (無國界校園服務)**. Submissions should focus on implementable AI applications.[5]

The course offers five candidate directions that connect research questions to specific users and workflows, based on the data conditions documented in the inventory. The category mappings below are course suggestions, not additional subtopics designated by the organizers. Each team should register under the category that best matches its primary purpose. Students may propose other questions if they also provide a data acquisition and evaluation plan.

### Five Suggested Research Directions

#### 1. AI Assistant for Checking and Summarizing Institutional Reports

**Primary category: AI Transformation of University Operations.** Help administrative staff turn approved aggregate university database data into traceable reports and explanations, reducing confusion between years, denominators, unique headcounts, and counts of occurrences. The deliverable is a working process for reading tables, checking them, generating charts and summaries, and conducting human review.

Start with one report series—學1, 學9, or 學29—and establish checking rules after obtaining its exact definitions. AI identifies table headers and textual claims and explains potential problems; reproducible code performs numerical calculations. Historical anomalies should be flagged for confirmation, without automatically correcting source data.

**Evaluation and limitations:** Compare the tool with manual spreadsheet work on error detection rate, false positive rate, numerical consistency, and task completion time. Separately labeled cases with deliberately inserted errors may be used to test the system. Before obtaining real data, teams must not claim to have improved NCU’s reporting quality. The minimum deliverable should cover one table and one common task. All reports intended for external use require human confirmation.

#### 2. AI Navigation for Interdisciplinary Learning and Course Progression

**Primary category: Intelligent Learning Guidance.** Help students and advisors explore interdisciplinary courses and identify prerequisite knowledge, using learning goals, completed courses, and approved course requirements. The deliverable is a navigation prototype in which every recommendation includes its course sources, conditions of applicability, and missing information.

Begin with course offering data, public program regulations, and manually entered course-taking scenarios. Reports 學29 and 學9 may help identify differences in participation across university units. Once authorized anonymous linkage is available, teams may add UCAN Holland interest measures, individual course grades, and semester grades to study how career interests or course-taking experience relate to performance. The earlier topics of “career interests and grades” and “course progression and subsequent performance” may serve as research modules; the project does not need to include all of them.

**Evaluation and limitations:** Compare existing course search, general AI question answering, and the prototype on compliance with course rules, the proportion of fabricated courses, and time needed to find courses. Limit the minimum deliverable to one program or one sequence of related courses. Separately verify the applicable academic year, prerequisites, and credit transfer or exemption rules. Career interests are not equivalent to ability, and associations do not establish course effects. Without follow-up evidence, teams must not claim improved grades or continuation rates.

#### 3. AI Matching for Research Expertise Discovery and Interdisciplinary Collaboration

**Primary category: Intelligent Research and Development Support.** Help researchers and research administration staff find relevant expertise, research outputs, and potential collaborating units within NCU based on a research question. The deliverable is semantic search and a recommendation list, with supporting papers, keywords, and years for every recommendation.

Use journal publication titles, abstracts, keywords, authors, and affiliations as the core data, optionally supplemented by National Science and Technology Council disciplinary fields or project attributes. Initially restrict the scope to one research issue and a clearly defined period. Resolve authors with identical names, remove duplicate publications, and verify affiliation mappings before generating recommendations. AI supports topic identification, semantic ranking, and evidence organization.

**Evaluation and limitations:** Have people with relevant domain knowledge review test queries. Compare the tool with keyword search on the relevance of top-ranked recommendations, citation accuracy, and exploration time. The minimum deliverable supports discovery of relevant outputs and expertise; it does not establish that collaborations have occurred. Complementarity across disciplines, willingness to collaborate, and personnel availability require separate confirmation. Research funding amounts were not identified in the catalog, so the project cannot also infer returns on investment.

#### 4. AI Support for Teaching Resource Resilience and Cross-Department Course Allocation

**Primary category: Resilient and Sustainable Governance.** Focus on the continuity and adaptability of course provision. Help course-offering units identify concentrated cross-department demand, persistently unmet registration demand, and possible adjustments to course offerings. The deliverable is a tool for examining demand and comparing scenarios. The final category fit should still be checked against the proposal’s content and the organizers’ guidance.

Build a demand baseline from course registration allocation histories and course offering data, initially focusing on one type of general education or interdisciplinary course. Confirm how repeated applications by the same student across allocation rounds are handled, what result codes mean, and how the success-rate denominator is defined before comparing semesters. If sufficient data are available, machine learning may be used to estimate demand. Otherwise, use observed demand as the basis, with AI translating user-proposed scenarios into parameters for confirmation before code compares the options.

**Evaluation and limitations:** Where comparable historical data are available, evaluate demand estimates using later-period data. For scenario tools, check parameter translation accuracy, constraint violations, and the interpretability of results. Additional seats, teaching staff, and funding may only be treated as explicit assumptions if the relevant data have not been obtained. Teams must not claim that additional classes are feasible, costs have been reduced, or carbon emissions have been lowered without evidence.

#### 5. AI Assistant for IR Data Discovery and Research Design

**Primary category: Intelligent Institutional Research.** Help faculty, students, and IR staff map research questions to data that can be requested, identify the level of analysis and overlapping time coverage, and recognize evidence gaps. The aim is to reduce unsuitable data choices and research questions that the available data cannot answer.

Use the 60 catalog entries, request fields, and public research summaries within the approved scope to build a data search tool with citations. Given a research question, the tool should list suggested datasets, fields, periods, linkage conditions requiring confirmation, and claims the data cannot support. It should produce a draft data requirements list for human review. The first version supports data discovery only and does not automatically submit requests.

**Evaluation and limitations:** Use manually checked test questions and compare the tool with keyword search, evaluating dataset recommendations, source citations, gap identification, and whether it appropriately declines to answer. Tests must include questions that currently lack core data, such as “interdisciplinary course participation and individual salary.” Without original records, the tool must not generate institutional statistics or research findings. Permission to index internal catalogs and the permitted scope of external AI use still require confirmation.

### Alternative Topics: NCU Brand Management and Borderless Campus Services

To retain five manageable candidate projects, the remaining two official categories are offered as alternative application contexts. Teams are not required to cover all seven categories:

| Official category | Possible research question and deliverable | Additional requirements and evaluation |
| --- | --- | --- |
| NCU Brand Management | Extend Direction 3 into an “AI Evidence Guide to NCU Research Strengths,” producing source-supported introductions to research strengths for potential partners or incoming students. | Use only research information that may be made public, and confirm permissions and wording for external communication. Check factual accuracy, citation completeness, and target users’ understanding. Page views or fluent writing do not establish branding outcomes. |
| Borderless Campus Services | Extend Direction 2 into “Multilingual Course and Program Navigation for Overseas Students,” addressing language-related difficulties in understanding rules and finding courses. | Add the course regulations applicable to overseas students and translations checked by people. Compare answer consistency across languages, understanding of rules, and task completion rates. Do not assume that every rule for local students also applies to overseas students. |

### Shared Competition Requirements

Every proposal must explain who will use the application and in what situation, which step AI performs, who reviews the output, and how it will be evaluated against the current approach. The prototype should complete one clearly bounded task and retain records of failure cases and usage limitations. The following course requirements reflect the official judging dimensions:[5]

- **Significance:** Explain the need through a specific institutional problem and the users affected.
- **Innovation:** Identify a substantive change from the current workflow or comparison tool, and explain why AI is needed.
- **Empirical support:** Provide held-out test data, standards checked by people, and baseline comparisons; do not show only successful cases.
- **Feasibility:** Explain data access, costs, maintenance, human review, and procedures for handling failure.

These are proposed research directions awaiting implementation and evaluation. They do not imply that data have been obtained, systems completed, or governance outcomes demonstrated. Past competition cases are used to examine research questions and evidence needs; submissions for 2026 must still follow this year’s focus on AI applications.[3][5]

### Data Acquisition and Contingency Plans

Complete the data requirements list in Week 2. The instructor will submit requests through the applicable procedures, and students and other personnel handling the data must work within the approved scope. Requests should specify the required fields, time coverage, level of analysis, personnel handling the data, computing environment, and how results will be presented.

**October 1 is the course’s data feasibility checkpoint.** If essential data have not been delivered, consult the instructor about narrowing the scope, using aggregate or public data already obtained, or adopting a data discovery or checking tool as the project. While awaiting approval, complete the literature review, method selection, and workflow design. Synthetic data may be used only for development and demonstration, must be labeled, and cannot be presented as empirical findings about NCU.

## 4. Weekly Schedule

Classes meet on Thursdays, 13:00–16:00. The schedule follows NCU’s calendar for Academic Year 115, Semester 1. The midterm review is on October 29, and the final assessment is on December 24.[4] All dates below are in 2026.

| Week | Date | Topic and research focus | Milestone or deliverable |
| --- | --- | --- | --- |
| 1 | 09/10 | Institutional research questions, competition requirements, and past cases; read the data inventory. | One-page research idea identifying users, the problem, and data needs. |
| 2 | 09/17 | Topic selection, literature, and research design; confirm data requests and division of work. | Research proposal, data requirements list, and contingency plan; complete the registration materials check by 09/21. |
| 3 | 09/24 | Define units of analysis, indicators, and time periods; plan data linkage. | Draft data dictionary, analysis plan, and source records. |
| 4 | 10/01 | Check data availability; conduct cleaning and exploratory analysis. | Data quality records and preliminary figures; activate the contingency plan if needed. |
| 5 | 10/08 | Baselines, research design, and evaluation metrics. | Baseline analysis and a data splitting or tool testing plan. |
| 6 | 10/15 | Implement analytical models and an AI application suited to the topic. | First demonstrable prototype and operating instructions. |
| 7 | 10/22 | Performance comparisons, data leakage, and error analysis. | Evaluation results, failure cases, and a revision list. |
| 8 | 10/29 | Midterm research review and individual oral defenses. | Midterm report; confirm the research scope achievable before the competition. |
| 9 | 11/05 | Strengthen evidence; examine alternative explanations and governance recommendations. | Complete first draft of the report and a table linking claims to evidence. |
| 10 | 11/12 | Review the project report, verify numbers, and prepare the submission. | Submission-ready report; complete the official submission by 11/16 at 23:59. |
| 11 | 11/19 | Slides, posters, and prototype demonstrations. | Draft slides and A0 poster; a set of anticipated questions and answers. |
| 12 | 11/26 | Competition rehearsal and demonstration checks. | Slides and demonstration files; attend the competition separately on Friday, 11/27. |
| 13 | 12/03 | Organize judges’ or peers’ feedback and examine unresolved questions. | Revision tracking table and a plan for further analysis. |
| 14 | 12/10 | Robustness, group differences, and scope of applicability. | Supplementary analyses and revised conclusions. |
| 15 | 12/17 | Governance proposal, maintenance costs, and research handover. | Revised report, reproduction instructions, and a two-page summary of governance recommendations. |
| 16 | 12/24 | Final presentations and individual oral examinations. | Complete research package, individual contribution statement, and research reflection. |

The instructor will announce adjustments if the academic calendar, competition arrangements, or data delivery changes. Methods instruction will follow each team’s research question; teams are not required to use every statistical and AI technique.

## 5. Assignments and Assessment

| Component | Weight | Requirements and assessment focus |
| --- | --- | --- |
| Individual research journal, discussions, and peer review | 20% | Record weekly work, evidence, research decisions, and next steps. Assessment considers engagement, problem identification, and the quality of responses to feedback. |
| Research proposal and data feasibility | 10% | A 2–3-page proposal covering the question, data, methods, baseline, outcome indicators, division of work, and contingency plan. Submit on 09/17 and complete revisions by 09/21. |
| Data processing, reproducible analysis, and prototype evaluation | 20% | Data dictionary, cleaning and analysis workflows, environment versions, and test records. Assessment considers methodological suitability, reproducibility, and error checking. |
| Midterm report and oral defense | 15% | On 10/29, explain the question, data, baseline, preliminary results, and remaining risks. Each student answers questions about their own work. |
| Competition report, slides, and poster | 20% | Assessment considers the argument, empirical support, feasibility of recommendations, and communication. Finalize the report for the course on 11/12; complete slides and the poster ahead of the official submission deadlines. |
| Revised final project and individual oral examination | 15% | Submit the research package on 12/24. Assessment considers new evidence, reasons for revisions, handover materials, and the ability to explain the work independently. |
| **Total** | **100%** | |

Midterm and final assessments consist of project reports and oral defenses; there are no separate written examinations. Individual grades for shared work are determined using research records, actual contributions, and oral defense performance. Every student must understand the main data processing steps and conclusions. Formatting or preparing slides alone does not substitute for research participation.

**Grades do not depend on reaching the final round or winning an award.** Students who do not reach the final round, or who are excused from participation for an approved reason, must still complete an equivalent project package and in-class presentation. A lack of significant differences, AI failing to outperform the baseline, or an unsupported original hypothesis can all constitute valid research outcomes. Assessment is based on the quality of methods and evidence.

If data delivery, physical or mental health, or other factors affect progress, discuss adjustments to the scope and deadlines with the instructor as early as possible. Students who take leave or miss class must submit the research records and deliverables required for that week.

## 6. Competition and Deliverable Requirements

An intermediate course goal is to complete a project that meets the competition requirements. The official process consists of registration, preliminary review of the project report, and final-round presentations and poster displays. Each team has 1–5 members.[5]

| Date | Type | Task |
| --- | --- | --- |
| 09/21 (Mon) | Course checkpoint | Complete checks of the topic, team, and registration materials. |
| 09/23 (Wed) | Official deadline | Complete online registration. |
| 11/12 (Thu) | Course checkpoint | Complete the submission-ready report. |
| 11/16 (Mon), 23:59 | Official deadline | Submit the project report. |
| 11/26 (Thu) | Course checkpoint | Rehearse for the final round and check the demonstration. |
| 11/27 (Fri) | Official event | Final round; outside the regularly scheduled Thursday class. |

The official judging weights are 25% each for significance, innovation, empirical support, and feasibility. These weights support project self-assessment and differ from the course grading scheme. Submission times for slides and posters, and the presentation duration, will follow subsequent announcements; the November 26 rehearsal does not replace an official deadline. Discuss attendance at the Friday event and any conflicts with other courses with the instructor in advance.

The project report should follow the official template and cover the topic, abstract, motivation and problem, methods, analytical results, institutional unit response strategies and recommendations, and conclusions. Slides and the A0 poster (841 × 1189 mm) must be consistent with the report and include team and advisor information as required by the announcement.[5]

The **final research package** includes the revised report, code and environment documentation, data dictionary, data that may be reviewed within the approved scope or instructions for obtaining access, main figures, slides, poster, a two-page summary of governance recommendations, and an individual contribution statement. It must explain the evidence added and revisions made since the competition version; simply resubmitting the original report is not sufficient.

## 7. Research and AI Use Policies

- **Data and permissions:** Use only public or approved data. Identify all personnel handling the data, the computing environment, and the period of use as required. Access to a catalog does not authorize unrestricted redistribution. Do not send internal university data or metadata to external AI services without permission. At the end of the approved period, close the project and handle the data according to the approval requirements.
- **Analytical responsibility:** Verify definitions across periods, data levels, and linkage methods. Counts of occurrences must not be treated as unique headcounts, and departmental averages must not be treated as individual observations. UCAN self-reported competencies and interests are not equivalent to objective ability. Associations involving course participation or grades do not directly establish course effects.
- **AI collaboration:** AI may assist with coding, searching, and writing, but its uses must be disclosed. Retain the model or service name, dates of use, important prompts, and records of human checks. Students remain responsible for citations, numbers, code, and conclusions.
- **Evaluation and reporting:** Both research-oriented and tool-oriented projects require appropriate baselines. Separate findings from inferences and document failure cases. A prototype that has not been evaluated in a real setting must not be described as having improved institutional performance.
- **Integrity and research participation:** Do not fabricate data, citations, interviews, or test results. Before conducting surveys, interviews, or user testing, confirm the applicable consent and review procedures with the instructor. Presentations of results should avoid identifying individuals or small groups.

## 8. Learning Materials and References

No textbook purchase is required. During the first two weeks, read the course data inventory and the comparison of past competition cases. Subsequently, select research methods materials and relevant literature according to the project topic. Build an annotated bibliography explaining how each source supports the question, methods, or interpretation. Data request catalogs and field information in the course analysis documents are available to enrolled students within the approved scope. Course documents and subsequent updates are maintained on the course website: <https://github.com/audachang/2026-Fall-IR-competition>.

[1] [NCU IR Data Inventory and NS5119 Topic Assessment — English](NCU_IR_Data_Inventory_and_Topic_Assessment_2026-09-09_EN.md), September 9, 2026. Prioritize the sections on data limitations, topic assessment, and application requirements. [Chinese source](https://github.com/audachang/2026-Fall-IR-competition/blob/main/NCU_IR_資料盤點與選題評估_2026-09-09.md).

[2] [NCU IR Catalog of 60 Data Items — English](NCU_IR_60_Item_Data_Catalog_2026-09-09_EN.md), September 9, 2026. Use it to locate data and fields; it does not replace the data dictionary provided after approval. [Chinese source](https://github.com/audachang/2026-Fall-IR-competition/blob/main/NCU_IR_60項資料目錄_2026-09-09.md).

[3] [Past Award-Winning Institutional Research Competition Topics and Corresponding NCU Data — English](IR_Competition_Past_Awards_and_NCU_Data_Mapping_2026-09-09_EN.md), September 9, 2026. Read selected cases on course participation, learning performance, and career interests to examine their data requirements. [Chinese source](https://github.com/audachang/2026-Fall-IR-competition/blob/main/校務研究競賽歷年得獎題目與NCU資料對照_2026-09-09.md).

[4] National Central University, Academic Year 115 Calendar, page 1. For course planning details, see the course plan retained by the instructor.

[5] Office of Institutional Research, [2026 AI Applications for University Governance Competition Announcement](https://ir.ncu.edu.tw/p/406-1034-216,r11.php?Lang=zh-tw). Checked on September 10, 2026, as recorded in the Chinese syllabus. Schedules, formats, and event details remain subject to the organizers’ final announcements.
