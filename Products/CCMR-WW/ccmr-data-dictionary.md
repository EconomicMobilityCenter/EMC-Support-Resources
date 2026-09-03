---
title: "CCMR Weekly Workbook - Data Dictionary"
orgs: ["all"]
product: "ccmr-weekly-workbook"
category: "Reference"
group: "CCMR Weekly Workbook"
order: 1
type: "article"
link: ""
published: false
---

This dictionary explains every column in the CCMR Weekly Workbook: the workbook column you see, the underlying data field, what it means in plain terms, where the data comes from, and whether it is available today.

**Status key:** 🟢 Live means the column is populated from a confirmed source. 🟡 / 🔴 Not yet available means the column exists but its data is not connected yet.

*Last updated: September 2026.*


## Student identifiers

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| Student ID | `student_id` | Student's local ID. | Roster (District) | 🟢 Live |
| FirstName | `first_name` | Student's first name. | Roster (District) | 🟢 Live |
| Last Name | `last_name` | Student's last name. | Roster (District) | 🟢 Live |

## Student Profile

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| Grade | `cohort_year` | Student's current grade level. | Roster (District) | 🟢 Live |
| Cohort Year | `ADD COLUMN NAME` | the year they are expected to graduate, not necessarily the year they actually do. Students stay tied to their cohort for tracking even if they graduate early or late.  | Roster (District) | 🟢 Live |
| Eco Dis | `eco_dis` | Whether the student is economically disadvantaged. | Roster (District) | 🟢 Live |
| Sped | `sped` | Whether the student is in special education. | Roster (District) | 🟢 Live |
| 504 | `504` | Whether the student is 504. | Roster (District) | 🔴 Not yet available |
| Emergent Bilingual | `emergent_bilingual` | Whether the student is an emergent bilingual / limited English proficiency student. | Roster (District) | 🟢 Live |

## HS Academic Standing

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| A-F CCMR | `ccmr_af` | CCMR A-F accountability indicator (whether the student is CCMR-met). | Early Warning file (District) | 🟢 Live |
| Attendance (%) | `attendance_pct` | Student's attendance percentage. | Not yet sourced | 🔴 Not yet available |
| Algebra I EOC | `algebra_i_eoc` | Algebra I STAAR EOC result. | STAAR EOC (District) | 🟡 Not yet available |
| English I EOC | `english_i_eoc` | English I STAAR EOC result. | STAAR EOC (District) | 🟡 Not yet available |
| English II EOC | `english_ii_eoc` | English II STAAR EOC result. | STAAR EOC (District) | 🟡 Not yet available |
| Biology EOC | `biology_eoc` | Biology STAAR EOC result. | STAAR EOC (District) | 🟡 Not yet available |
| U.S. History EOC | `us_history_eoc` | U.S. History STAAR EOC result. | STAAR EOC (District) | 🟡 Not yet available |
| On Track to Graduate | `on_track_to_graduate` | Whether the student is on track to graduate. | Not yet sourced | 🔴 Not yet available |
| # of credits | `total_hs_credits` | Total high school credits earned. | Transcript (District) | 🟢 Live |
| Unweighted GPA | `gpa` | Student's high school grade point average. | Roster (District) | 🟢 Live |
| Weighted GPA | `weighted_gpa` | Student's high school grade point average on a weighted scale. | Roster (District) | 🔴 Not yet available |
| Work Ready | `work_ready` | Whether the student is designated work-ready. | Roster (District) | 🟢 Live |
| Counselor | `counselor_name` | Name of the student's assigned counselor. | Roster (District) | 🟢 Live |
| Advisor | `advisor_name` | Name of the student's assigned advisor. | Roster (District) | 🟢 Live |

## Assessments (TSIA2/SAT/ACT)

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| TSI Met By Assessment | `tsi_met_by_assessment` | Overall TSI status: Met only if both math and ELAR are met, otherwise Not Met. | Calculated | 🟢 Live |
| TSI Math Met | `tsi_math_met` | Whether the student met the TSI math bar (1 = met, 0 = not met). | Calculated | 🟢 Live |
| TSI Math Met by | `computed` | Which assessment the student met the TSI math bar with (TSIA2, SAT, or ACT). | Calculated | 🟢 Live |
| SAT Math `AD` | `sat_math` | SAT math score. | Assessment files (District) | 🟢 Live |
| ACT Math `AE` | `act_math` | ACT math score. | Assessment files (District) | 🟢 Live |
| TSIA Math Score  | `tsia2_math_crc` | TSIA2 math college-readiness score. | Assessment files (District) | 🟢 Live |
| TSIA Math Diagnostic  | `tsia2_math_diag_level` | TSIA2 math diagnostic level. | Assessment files (District) | 🟢 Live |
| TSI ELAR Met  | `tsi_elar_met` | Whether the student met the TSI ELAR bar (1 = met, 0 = not met). | Calculated | 🟢 Live |
| TSI ELAR Met by | `computed` | Which assessment the student met the TSI ELAR bar with (TSIA2, SAT, or ACT). | Calculated | 🟢 Live |
| SAT Reading and Writing | `sat_ebrw` | SAT Evidence-Based Reading & Writing score (also reads satela). | Assessment files (District) | 🟢 Live |
| ACT English | `act_english` | ACT English score. | Assessment files (District) | 🟢 Live |
| TSIA ELAR Score | `tsia2_elar_crc` | TSIA2 ELAR college-readiness score. | Assessment files (District) | 🟢 Live |
| TSIA ELAR Essay  | `tsia2_essay_score` | TSIA2 essay score. | Assessment files (District) | 🟢 Live |
| TSIA ELAR Diagnostic | `tsia2_elar_diag_level` | TSIA2 ELAR diagnostic level. | Assessment files (District) | 🟢 Live |

## Dual credit (Dallas College)

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| Dual Credit Program | `dual_credit_path` | Student's dual-credit pathway. | Not yet sourced | 🟡 Not yet available |
| DC College Credits Earned | `dual_credit_earned` | Dual-credit hours/credit the student has earned. | Enrollment File (Dallas College) | 🟢 Live |
| Academic College Standing | `dual_credit_standing` | Student's current academic standing in dual credit. | Enrollment File (Dallas College) | 🟢 Live |
| Dual Credit GPA | `dual_credit_gpa` | Student's cumulative dual-credit GPA. | Enrollment File (Dallas College) | 🟢 Live |
| College Credits Enrolled | `dual_credit_enrolled` | Dual-credit hours the student is currently or upcoming enrolled in. | Courses file (Dallas College) | 🟢 Live |
| Associate Degree Earned | `associate_degree` | Whether the student earned an associate degree (AA or AS). | Credential files (District + Dallas College) | 🟢 Live |

## Career readiness & CTE

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| IBC Completed | `ibc_latest_aligned` | The student's most recent aligned Industry-Based Certification. | Certifications file (District) | 🟢 Live |
| Program of Study (name) | `pos_name` | Name of the student's aligned CTE Program of Study. | CTE files (District) | 🟢 Live |
| Program of Study Status | `pos_status` | Student's CTE Program of Study status. | CTE files (District) | 🟢 Live |
| Level I Certification Earned | `credential_level_1` | Whether the student earned a Level 1 certificate (C1). | Credential files (District + Dallas College) | 🟢 Live |
| Level II Certification Earned | `credential_level_2` | Whether the student earned a Level 2 certificate (C2). | Credential files (District + Dallas College) | 🟢 Live |

## College application & enrollment (Promise)

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| Path Form Submitted | `path_form_submitted` | Whether the student submitted the PathForm / pledge (pledge status not ineligible). | Promise Data | 🟢 Live |
| Interest (from Path form) | `path_form_interest` | Career pathway the student is most interested in. | Promise Data | 🟢 Live |
| Senior Survey Submitted | `senior_survey` | Whether the student submitted the senior survey. | Promise Data | 🟢 Live |
| Applied | `applied` | Whether the student applied to any partner college. | Promise Data | 🟢 Live |
| Applied to 3 | `applied_three` | Whether the student applied to at least 3 partner colleges. | Promise Data | 🟢 Live |
| Financial Aid | `financial_aid_status` | Whether the student submitted FAFSA or TASFA. | Promise Data | 🟢 Live |
| Accepted | `accepted` | Whether the student was admitted to a partner college. | Promise Data | 🟢 Live |
| Enrolled | `postsecondary_enrolled` | Whether the student is enrolled at a partner college (status = Enrolled). | Promise Data | 🟢 Live |
| Advanced Diploma  | `advanced_diploma` | Whether the student has an advanced diploma designation (based on graduation code plus program). | Roster (District) | 🟢 Live |

## Class Schedule

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| Class,Teacher | `class_teacher_1` | Teacher for class period 1. | Student Schedule (District) | 🟢 Live |
| Class,Teacher 2 | `class_teacher_2` | Teacher for class period 2. | Student Schedule (District) | 🟢 Live |
| Class,Teacher 3 | `class_teacher_3` | Teacher for class period 3. | Student Schedule (District) | 🟡 Not yet available |
| Class,Teacher 4 | `class_teacher_4` | Teacher for class period 4. | Student Schedule (District) | 🟡 Not yet available |
| Class,Teacher 5 | `class_teacher_5` | Teacher for class period 5. | Student Schedule (District) | 🟡 Not yet available |
| Class,Teacher 6 | `class_teacher_6` | Teacher for class period 6. | Student Schedule (District) | 🟡 Not yet available |
| Class,Teacher 7 | `class_teacher_7` | Teacher for class period 7. | Student Schedule (District) | 🟡 Not yet available |
| Class,Teacher 8 | `class_teacher_8` | Teacher for class period 8. | Student Schedule (District) | 🟡 Not yet available |
| Extra Curricular | `extracurricular` | Student's extracurricular participation. | Not yet sourced | 🔴 Not yet available |

## Advanced coursework and Prep

| Column Name | Data field | What it means | Source | Status |
|---|---|---|---|---|
| Highest AP Score | `highest_ap_score` | Student's highest AP exam score across all AP subjects. | Advanced Placement file (District) | 🟢 Live |
| Highest IB Score | `highest_ib_score` | Student's highest IB score. | Not yet sourced | 🔴 Not yet available |
| Highest OnRamps College Grade | `highest_onramps_grade` | Student's highest OnRamps letter grade. | OnRamps file (District) | 🟢 Live |
| College Prep Type | `college_Prep` | The college prep course pathway the student is enrolled in through Texas College Bridge. |Texas College Bridge (District) | 🟡 Not yet availabl |
| College Prep Type 2 | `college_prep2` | A second college prep pathway, if the student is enrolled in more than one. | Texas College Bridge (District) | 🟡 Not yet availabl |
| College Prep Math Status | ` ` | The student's status in the college prep math course (Texas College Bridge), used toward TSI math readiness. | Texas College Bridge (District) | 🟡 Not yet availabl |
| College Prep ELAR Status | `` | The student's status in the college prep ELAR course (Texas College Bridge), used toward TSI ELAR readiness. | Texas College Bridge (District) | 🟡 Not yet availabl |
| HB3 CCMR | `ccmr_hb3` | CCMR indicator under HB3 (met both ELA and math, excluding certain cases). | Early Warning file (District) | 🟢 Live |
| HB3 IBC Status | `ibc_hb3` | Whether the student earned at least one Industry-Based Certification (HB3 indicator). | Early Warning file (District) | 🟢 Live |
| A-F Career Status  | `career_af` | Career A-F accountability indicator. | Early Warning file (District) | 🟢 Live |




