# NCU IR Data Inventory and NS5119 Topic Assessment

Inspection date: September 9, 2026, Asia/Taipei. Compilation and verification completed at 2026-09-09 14:44:03 +08:00. Method: authenticated, read-only inspection through the Codex built-in browser of the catalog, request-field pages for 60 datasets, application and download pages, and public IR Office instructions. This report describes the pages visible during that inspection. No analytical datasets were obtained.

*Translated September 13, 2026 from [the Chinese report](NCU_IR_資料盤點與選題評估_2026-09-09.md). Inspection results and recommendations describe the original September 9 work, not a new verification or the final course topic list. Platform labels and raw codes are retained where useful; English source titles are descriptive translations.*

[English course information](README.md#english) · [Student-facing syllabus](SYLLABUS_EN.md)

## 1. What Was Confirmed

**The platform was accessible; the information obtained consisted of the catalog and request-field lists, not data ready for analysis.** The authenticated page header displayed the name “張智宏” and a logout option, and the home page showed a welcome message. This state was verified in the browser during the inspection rather than inferred from the earlier task’s login statement.

The working directory was confirmed as `C:/Users/audachang/Documents/Codex/2026-09-09/ncu-ir-data-exploration`. The browser startup error encountered in the earlier Dropbox task did not occur. A read-only attempt to access the original course plan returned access denied, so the original course files were not read or modified during that inspection. This report assessed the five candidate topics listed in the handoff and did not add time-by-time activities for individual classes.

| Evidence status | Inspection result | Supported conclusion |
| --- | --- | --- |
| Readable: catalog and metadata | 38 administrative-system datasets and 22 Ministry of Education reports; all 60 field pages were opened. | Dataset names, requestable fields, time options, and some descriptions were confirmed. |
| Readable: data values / analytical tables | None obtained. | Record counts, distributions, missingness, quality, and analytical findings cannot be confirmed. |
| Catalog visible but field page not opened | 0 among the 60 included datasets. | This does not establish coverage of all data available under every account or permission level. |
| Application required | All 60 field pages offered “Add dataset of interest” (加入有興趣資料集). | An application route exists; permission to use the data has not been granted. |
| Download availability | The Data Download / Amendment / Closure page was readable; its default date range returned no records. | No downloadable dataset was verified and no raw data were downloaded. |
| Not verified | Approved file formats, delivery times, linkage keys, student access arrangements, and annual completeness. | These require information from the application outcome or data administrators. |

The administrative category pages displayed 70 rows, including duplicate dataset names and view URLs. Deduplication by view URL yielded 38 datasets; the 70 rows must not be counted as 70 distinct datasets. Unique counts were 18 academic affairs, 5 student affairs, 2 personnel, 10 research and development, and 3 integrated data. The Ministry of Education tab had another 22 links. See the [60-item catalog](NCU_IR_60_Item_Data_Catalog_2026-09-09_EN.md) for the complete list and item-level sources.

Source: [Integrated Query Platform](https://cis.ncu.edu.tw/IRSys/dataMarket/dataPlatform).

## 2. Interpreting Fields and Time Information

The pages display checklists of fields available for requests. Most dataset descriptions are brief or blank. **These are not complete data dictionaries:** they generally omit data types, code values, missing-value definitions, unique keys, row definitions, historical field changes, and calculation formulas.

Time selectors use semesters, academic years, ROC years, Gregorian years, or ministry reporting periods. This report preserves the raw codes: for example, `1141` and `11403` must not be treated as the same time unit. An option’s presence does not prove that complete data exist for that period. An “updated on” date also does not establish data coverage. The latest available period differs across datasets; a course in 115-1 cannot assume that complete course-taking records for 115-1 are already available.

The following issues were observed at the metadata or interface level; underlying records had not been checked:

- UCAN Common Workplace Competencies listed academic years 109, 110, 111, 112, and 114, but not 113.
- The Student Basic Data semester selector included `7701`; the Teaching and Research Personnel Basic Data ROC-year selector included `011`. The field pages did not establish whether these were special values, entry errors, or consequences of different time fields.
- 學9 included period `11120`; it must not be silently corrected to `11110` or another period.
- The scholarship selector mixed three- and four-digit codes, such as `110`, `1101`, and `1030`. The Student Dual-Degree Data selector also included a blank option.
- Project Data included years 116 and 117 and the value `-`. Future project years may be reasonable, but their meaning still requires confirmation.
- The personnel awards year selector was not numerically ordered. Its first and last options cannot be used to infer the coverage range.
- 學14 (student counts by age) and 學22 (new entrant origins) listed only 10710, 11210, and 11310, which is insufficient for a continuous annual trend without additional data.

## 3. Data Most Relevant to Topic Selection

The levels below are inferred from fields, not verified row definitions. Confirm them again when data are delivered.

| Dataset | Key fields actually visible | Selectable periods | Inferred level and main limitations |
| --- | --- | --- | --- |
| Course Offerings | Course name/code/serial number, academic year and semester, offering department, objectives, materials, teaching language, year level, credit program name/code, jointly offered professional program, programming implementation/application/logic and computational thinking flags. | 0851–1142; 60 options. | Course offering records. Explicit prerequisites and AI-specific flags were not identified; complete AI program rules are not assured. |
| Course Registration Allocation History | Preference rank, lottery number, registration result, allocation code, allocation end time, course number, semester, student department/year level/gender. | 1011–1141; 27 options. | Allocation events. Rounds, duplicate events, and success-rate denominators require confirmation. |
| Student Course Grades | Credits, course name/code/serial number, academic year and semester, grade, allocation result, student department, course and registration attributes. | 0922–1141; 44 options. | Student–course records. A usable cross-table student linkage key was not confirmed. |
| 學29 Programming Course Participation | Department category, formally enrolled students, students who have taken programming courses, students in digital technology interdisciplinary programs, and gender breakdowns. | 10710–11403; 14 periods. | Unit/program type/period aggregates. “Have taken” does not mean current-period enrollment; programming participation is not AI literacy. |
| 學9 Interdisciplinary Course Participation | Unit, program type, inter-university course enrollment, minors, double majors, teacher education programs, other credit programs, and gender breakdowns. | 10303–11410; 25 periods, including 11120. | Aggregates. Some fields count occurrences, not distinct people. |
| Teaching and Research Personnel Basic Data | Birth year, college/department, position, staff type, arrival year/month, educational qualifications, and other fields. | ROC-year options 011, 054, 057–114. | Personnel records. The field filtered by year, employment reference date, and full-time scope were unclear. |
| Teaching and Research Personnel Experience | Experience type, job title, unit, starting year, start date, and end date. | ROC years 055, 063–115. | Employment histories. Cross-table linkage and valid current headcounts were not verified; these cannot directly produce retirement lists. |
| UCAN Common Workplace Competencies | Raw scores/PR values for information technology application, problem solving, innovation, and other areas; pre/post assessment, assessment semester/year, competency development plan. | Academic years 109, 110, 111, 112, 114. | The official field page explicitly described student self-assessment. This is not an AI scenario performance test; pre/post pairing was not confirmed. |
| Graduate Employment Analysis Results | Unit, program type, graduation academic year, salary observation year, graduate/available-for-work counts, mean monthly salary/standard deviation, workforce participation rate, differences from national discipline/field benchmarks. | Academic years 102–111; 10 options. | Unit/program type/graduating cohort/salary-year aggregates. Distinguish graduation year from salary observation year. |
| Graduate Employment by Industry | Unit, program type, graduation academic year, salary observation year, industry counts, and total. | Academic years 102–111; 10 options. | Aggregates. Common keys with the employment results table and small-cell suppression rules require confirmation. |
| Journal Evaluation Data | ISSN/EISSN, journal, field, database, year, IF/CiteScore, ranking numerator/denominator, percentile. | Gregorian years 2018–2025. | Journal-level indicators, not university rankings. |
| Journal Publications | Paper title, journal, publication year, abstract, keywords, unit, FWCI, database, author order, international collaboration, SDGs. | Gregorian years 1985–2025. | Publication/author relationships. FWCI provenance and observation window, and publication deduplication rules, were unclear. |

Each dataset’s clickable field-page source appears in the [complete catalog](NCU_IR_60_Item_Data_Catalog_2026-09-09_EN.md). The table above selects fields rather than listing them all. It does not establish that every field has values in every period.

## 4. Application Rights, Workflow, and Download Limits

The IR Office’s [data application instructions](https://ir.ncu.edu.tw/p/412-1034-2329.php?Lang=zh-tw) state that faculty may apply directly, staff must ask the office to enable access, and students must apply through their supervising faculty member. Faculty eligibility to apply does not imply automatic approval. Whether course students may jointly handle data, which environments they may use, and what may be made public still require confirmation in the application.

The following interface route was verified during the inspection:

1. Select a dataset in the Integrated Query Platform and read its request fields. Fields and start/end periods can be selected; some tables also allow restrictions by unit (限縮申請單位).
2. The “Add dataset of interest” button and [Cart](https://cis.ncu.edu.tw/IRSys/dataMarket/dataCart) page were present. No fields were checked and no datasets were added during the inspection. The cart displayed no records.
3. The [Data Use Applications](https://cis.ncu.edu.tw/IRSys/dataMarket/dataApply) page supported status queries: Data Preparation in Progress, Under Review, Not Approved, Application Completed, Withdrawal in Progress, and Withdrawn by Applicant. The default modification-date range was 2025-09-09 to 2026-09-09, and no records appeared. A “Teaching Practice Research Program Data Application” entry was also visible, but this does not establish that this course qualifies for that application type.
4. The [Data Download / Amendment / Closure](https://cis.ncu.edu.tw/IRSys/dataMarket/dataHistory) page used the same default range, 2025-09-09 to 2026-09-09, for the data use period and displayed no records. This was not a review of all historical applications and does not prove that the account permanently lacks download rights.
5. The download page stated that projects must be closed and data destroyed at the end of the use period, otherwise further applications are blocked. The empty case list did not allow verification of delivery formats, post-approval download steps, or deadlines.

The page structure supports the interpretation “select data and scope → cart → application review → download and closure.” However, no application was completed or submitted, and the complete set of mandatory fields for a standard application was not verified.

An official paper application is also available, including a confidentiality agreement and usage declaration. The instructions require the unit head’s signature or seal and documentation from everyone jointly participating in or handling the data. During this inspection, only the public webpage instructions were read; the attached guidelines were not opened in full, and no paper form was completed. No email, registration, application, or transfer of individual-level data occurred.

## 5. Reassessment of the Five Original Candidate Topics

These are research design judgments based on the field inventory, not empirical findings from datasets that had not been obtained.

| Candidate topic | Feasibility judgment | Minimum initial deliverable | Missing key evidence |
| --- | --- | --- | --- |
| 1. AI evidence assistant for institutional research | **A prototype can be built first; empirical analysis functions require data approval.** The 60 catalog entries and field lists can support an initial data discovery and suitability Q&A tool. | Each answer identifies datasets, fields, periods, sources, and reasons a question can or cannot be answered. Test citation accuracy and appropriate refusal using questions written and checked by the instructor. | Permission for students and external models to use the catalog; approved data and indicator definitions for institutional statistics. |
| 2. AI program course navigation for students without computing backgrounds | **The strongest direct data foundation, but scope should be narrowed.** Course offerings provide content and program affiliation; 學29 and 學9 support participation analysis. | Begin with programming/digital interdisciplinary course discovery and navigation for students in non-computing departments. Attach course objectives and rule sources to recommendations. | Official AI program course lists, prerequisites/credit exemptions/graduation rules, actual 115-1 offerings, and timetable clashes. Do not promise AI program completion or course eligibility before checking these. |
| 3. Scenario-based AI literacy diagnosis and feedback | **Existing IR data are insufficient for direct completion.** UCAN can provide background or self-reported competency reference measures, not AI literacy outcomes. | Design scenario tasks, scoring rubrics, and a small pilot; have people check feedback, with IR data as supplementary information. | Scenario items, objective performance, scoring agreement, and validity evidence. Linking to IR records also requires permission and linkage keys. |
| 4. Faculty age structure and replacement hiring scenarios | **Conditionally feasible; restrict initial work to unit-level aggregate scenarios.** Birth year and employment history fields exist. | Compare 3–5-year scenarios using college/department age bands and assumed hiring counts, making all assumptions explicit. | Employment reference date, full-time staff selection, age-band counts, definitions of departures and hires, staffing limits, funding, and teaching demand. Birth year alone cannot establish retirement dates, individual intentions, or replacement needs. |
| 5. AI evidence checking for university rankings and institutional indicators | **Ranking data are insufficient; institutional/research indicator checking is more feasible.** Journal evaluations, publications, and ministry reports are listed, but no QS/THE university ranking dataset was identified. | Narrow the task to checking research indicator definitions or verifying numbers and sources in institutional reporting claims. | Current-year methods from the relevant ranking organization, original institutional component values, and year/unit mappings. IF, CiteScore, and FWCI are not interchangeable or substitutes for university ranking scores. |

An advanced search for `AI`, with both data sources selected and union mode enabled, returned no results. This establishes only that the particular query found no match; it does not establish that every course is unrelated to AI. The ranking-data judgment is limited to the 60 catalog entries and does not imply that other university systems lack such data.

## 6. Topics with Stronger Data Foundations and Suggested Priorities

**First choice: Gaps in programming and digital interdisciplinary participation among students in non-computing departments, combined with traceable course recommendations.** Use 學29 as the core because it contains both enrolled-student and prior-participation counts. Use 學9 separately to describe interdisciplinary participation, and course offerings to identify possible courses. This design is more likely to yield checkable results from aggregate data than a project that begins by linking individual grades.

First verify consistency of units, program types, and periods, then calculate “students who have taken programming courses / total formally enrolled students.” Confirm whether the numerator counts distinct currently enrolled students and whether numerator and denominator use the same scope. Until confirmed, call it a proposed indicator awaiting definition approval. Define “non-computing departments” through the university’s classification or an explicit mapping; departmental affiliation does not establish every student’s actual programming background. AI explains differences, provides checkable course evidence, and answers follow-up questions; reproducible calculations produce proportions and charts. Evaluate the assistant by comparing course-finding and evidence-checking accuracy, time, and erroneous recommendations with and without it.

**Alternative: An AI evidence presentation assistant for graduate employment and industry destinations.** Employment results and industry destinations share similar unit, program type, graduation year, and salary-year fields. Begin with aggregate comparisons across observation years and have the assistant attach baselines and reasons why particular conclusions cannot be drawn. Administrators must explain the population available for work, salary sample, and national comparison definitions. Departmental means cannot establish individual graduates’ salaries, and associations cannot be described as course effects.

**Another feasible direction: Cross-department course demand and allocation bottlenecks.** Allocation records include preference ranks and results; combining them with offerings may identify unmet course demand. First confirm how to deduplicate students across allocation rounds, interpret rejection/unsuccessful lottery codes, and define the applicant denominator. This topic is closer to resource allocation than course recommendation alone, but requires more work on access and event processing.

If approval cannot be obtained in time, narrow Topic 1 to an “IR Data Discovery and Evidence Suitability Assistant,” using only authorized catalog/public information and manually established reference answers. Do not imply that internal data have been analyzed. Synthetic demonstration data must be prominently labeled and cannot count as institutional findings or empirical results.

## 7. Concrete Draft Requirements for a Future Application — Not Submitted

Concentrate initially on the first-choice topic rather than requesting every dataset:

| Priority dataset | Suggested fields and scope | Purpose |
| --- | --- | --- |
| 學29 | Request valid recent periods actually visible in the platform, for example those within 11003–11403; period, academic year/semester, college/unit/program type and department category, enrolled counts, counts who have taken programming, digital interdisciplinary program counts, and supplementary notes. | Establish denominators and comparable units without requesting individual student records. |
| Course Offerings | Valid offerings in 1101–1142; course and unit codes/names, semester, objectives, year level, language, program affiliation, programming flags, and status. | Explain course options and link recommendations to the supporting data. |
| 學9 (secondary) | Periods that can be aligned with 學29; unit/program type, interdisciplinary participation categories, and supplementary notes. | Describe minor, double-major, and program participation, keeping occurrences and distinct headcounts separate. |

Focus questions to the IR Office on three areas:

1. **Definitions and completeness:** Which field does each time option filter? Are the periods complete, and when did definitions change? Request data types, codebooks, missing-value and suppression rules, and explanations of special periods such as 11120. Recent periods could be delivered first, with older data later.
2. **Comparability and linkage:** Is there a mapping for renamed or merged units? How is “have taken” calculated in 學29, and is it limited to currently enrolled students? If course registration events are later added, could administrators first produce unit × course × period aggregates to avoid unnecessary individual records and linkage keys?
3. **Course use and delivery:** May NS5119 students be joint data handlers? Is use in specified AI tools, indexing of the catalog, and competition display of aggregate findings permitted? What are the format, expected delivery date, approved use period, and closure requirements? A document’s absence from the visible interface does not establish that it is unnecessary.

## 8. Competition Schedule and Scope of This Inspection

The [2026 AI Applications for University Governance Competition announcement](https://ir.ncu.edu.tw/p/406-1034-216,r11.php?Lang=zh-tw) was reread during the original inspection. It still listed registration by 2026-09-23, the project report by 2026-11-16 at 23:59, and the final round on 2026-11-27. Teams consist of 1–5 people. Significance, innovation, empirical support, and feasibility each carry 25%. The organizers state that the detailed schedule is subject to the final announcement.

Topic selection should therefore consider more than the number of AI functions. Allow time to confirm definitions, obtain approval and delivery, conduct reproducible analysis, and evaluate with users. These are course topic recommendations from the original exploration. That work did not modify the original course plan, choose the user’s competition topic, or submit external data or applications.
