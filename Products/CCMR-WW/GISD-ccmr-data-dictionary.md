---
title: "Data Dictionary"
orgs: ["garland-isd"]
product: "ccmr-weekly-workbook"
category: "Training"
group: "CCMR Weekly Workbook"
order: 5
type: "article"
published: true
---

This dictionary explains every column in the CCMR Weekly Workbook: the workbook column you see, the underlying data field, what it means in plain terms, where the data comes from, and whether it is available today.

**Status key:** 🟢 Live means the column is populated from a confirmed source. 🟡 / 🔴 Not yet available means the column exists but its data is not connected yet.

*Last updated: October 2026.*
 
 
## Student identifiers
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| Student ID | `student_id` | Student's local ID. | Garland - Roster | Skyward | 🟢 Live |
| FirstName | `first_name` | Student's first name. | Garland - Roster | Skyward | 🟢 Live |
| Last Name | `last_name` | Student's last name. | Garland - Roster | Skyward | 🟢 Live |
 
## Student Profile
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| Grade | `grade_level` | Student's current grade level. | Garland - Roster | Skyward | 🟢 Live |
| Cohort Year | Calculated | The year the student is expected to graduate, calculated from the year they started high school (from the Roster). Students stay tied to their cohort for tracking even if they graduate early or late. | Garland - Roster | Skyward | 🟢 Live |
| Eco Dis | `eco_dis` | Whether the student is economically disadvantaged. | Garland - Roster | Skyward | 🟢 Live |
| Sped | `sped` | Whether the student is in special education. | Garland - Roster | Skyward | 🟢 Live |
| 504 | `504` | Whether the student is 504. | Not provided by district | n/a | 🔴 Not yet available |
| Emergent Bilingual | `emergent_bilingual` | Whether the student is an emergent bilingual / limited English proficiency student. | Garland - Roster | Skyward | 🟢 Live |
 
## HS Academic Standing
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| A-F CCMR | `ccmr_af` | CCMR A-F accountability indicator (whether the student is CCMR-met). | Garland - Early Warning | TEA CCMR Early Warning System | 🟢 Live |
| Attendance (%) | `attendance_pct` | Student's attendance percentage. | Not provided by district | n/a | 🔴 Not yet available |
| Algebra I EOC | `algebra_i_eoc` | Algebra I STAAR EOC result. | Not provided by district | n/a | 🔴 Not yet available |
| English I EOC | `english_i_eoc` | English I STAAR EOC result. | Not provided by district | n/a | 🔴 Not yet available |
| English II EOC | `english_ii_eoc` | English II STAAR EOC result. | Not provided by district | n/a | 🔴 Not yet available |
| Biology EOC | `biology_eoc` | Biology STAAR EOC result. | Not provided by district | n/a | 🔴 Not yet available |
| U.S. History EOC | `us_history_eoc` | U.S. History STAAR EOC result. | Not provided by district | n/a | 🔴 Not yet available |
| On Track to Graduate | `on_track_to_graduate` | Whether the student is on track to graduate. | Not provided by district | n/a | 🔴 Not yet available |
| # of credits | `total_hs_credits` | Total high school credits earned. | Garland - Transcripts | Skyward | 🟢 Live |
| Unweighted GPA | `gpa` | Student's high school grade point average on an unweighted scale. | Garland - Roster | Skyward | 🟢 Live |
| Weighted GPA | `weighted_gpa` | Student's high school grade point average on a weighted scale. | Not provided by district | n/a | 🔴 Not yet available |
| Work Ready | `work_ready` | Whether the student is designated work-ready. | Garland - Roster | Skyward | 🟢 Live |
| Counselor | `counselor_name` | Name of the student's assigned counselor. | Garland - Roster | Skyward | 🟢 Live |
| Advisor | `advisor_name` | Name of the student's assigned advisor. | Garland - Roster | Skyward | 🟢 Live |
 
## Assessments (TSIA2/SAT/ACT)
 
Test score columns can draw on more than one file: the current test file, the Early Warning file, and historical assessment files. If a student has more than one result, the workbook shows the highest.
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| TSI Met By Assessment | `tsi_met_by_assessment` | Overall TSI status: Met only if both math and ELAR are met, otherwise Not Met. | Calculated from TSI Math Met and TSI ELAR Met | Calculated in workbook | 🟢 Live |
| TSI Math Met | `tsi_math_met` | Whether the student met the TSI math bar (1 = met, 0 = not met). | Calculated from SAT, ACT, and TSIA2 math scores | Calculated in workbook | 🟢 Live |
| TSI Math Met by | Calculated | Which assessment the student met the TSI math bar with (TSIA2, SAT, or ACT). If more than one qualifies, the first one that meets the criteria is shown. | Calculated from TSI Math Met | Calculated in workbook | 🟢 Live |
| SAT Math | `sat_math` | SAT math score. | Garland - SAT, Garland - Early Warning | College Board; TEA CCMR Early Warning System | 🟢 Live |
| ACT Math | `act_math` | ACT math score. | Garland - ACT, Garland - Early Warning | ACT; TEA CCMR Early Warning System | 🟢 Live |
| TSIA Math Score | `tsia2_math_crc` | TSIA2 math college-readiness score. | Garland - TSIA2, Garland - Early Warning | College Board; TEA CCMR Early Warning System | 🟢 Live |
| TSIA Math Diagnostic | `tsia2_math_diag_level` | TSIA2 math diagnostic level. | Garland - TSIA2, Garland - Early Warning | College Board; TEA CCMR Early Warning System | 🟢 Live |
| TSI ELAR Met | `tsi_elar_met` | Whether the student met the TSI ELAR bar (1 = met, 0 = not met). | Calculated from SAT, ACT, and TSIA2 ELAR scores | Calculated in workbook | 🟢 Live |
| TSI ELAR Met by | Calculated | Which assessment the student met the TSI ELAR bar with (TSIA2, SAT, or ACT). If more than one qualifies, the first one that meets the criteria is shown. | Calculated from TSI ELAR Met | Calculated in workbook | 🟢 Live |
| SAT Reading and Writing | `sat_ebrw` | SAT Evidence-Based Reading & Writing score (also reads satela). | Garland - SAT, Garland - Early Warning | College Board; TEA CCMR Early Warning System | 🟢 Live |
| ACT English | `act_english` | ACT English score. | Garland - ACT, Garland - Early Warning | ACT; TEA CCMR Early Warning System | 🟢 Live |
| TSIA ELAR Score | `tsia2_elar_crc` | TSIA2 ELAR college-readiness score. | Garland - TSIA2, Garland - Early Warning | College Board; TEA CCMR Early Warning System | 🟢 Live |
| TSIA ELAR Essay | `tsia2_essay_score` | TSIA2 essay score. | Garland - TSIA2, Garland - Early Warning | College Board; TEA CCMR Early Warning System | 🟢 Live |
| TSIA ELAR Diagnostic | `tsia2_elar_diag_level` | TSIA2 ELAR diagnostic level. | Garland - TSIA2, Garland - Early Warning | College Board; TEA CCMR Early Warning System | 🟢 Live |
 
## Dual credit (Dallas College)
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| Dual Credit Program | `dual_credit_path` | Student's dual-credit pathway. | Dallas College - Enrollments | Dallas College | 🔴 Not yet available |
| DC College Credits Earned | `dual_credit_earned` | Dual-credit hours/credit the student has earned. | Dallas College - Enrollments | Dallas College | 🟢 Live |
| Academic College Standing | `dual_credit_standing` | Student's current academic standing in dual credit. | Dallas College - Enrollments | Dallas College | 🟢 Live |
| Dual Credit GPA | `dual_credit_gpa` | Student's cumulative dual-credit GPA. | Dallas College - Enrollments | Dallas College | 🟢 Live |
| College Credits Enrolled | `dual_credit_enrolled` | Dual-credit hours the student is currently or upcoming enrolled in. | Dallas College - Courses | Dallas College | 🟢 Live |
| Associate Degree Earned | `associate_degree` | Whether the student earned an associate degree (AA or AS). | Garland - Associate Degree, Dallas College - Credentials | Dallas College | 🟢 Live |
 
## Career readiness & CTE
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| IBC Completed | `ibc_latest_aligned` | The student's most recent aligned Industry-Based Certification. | Garland - Certifications | EduThings | 🟢 Live |
| Program of Study (name) | `pos_name` | Name of the student's aligned CTE Program of Study. | Garland - All Time Course Enrollment | EduThings | 🟢 Live |
| Program of Study Status | `pos_status` | Student's CTE Program of Study status. | Garland - Student Coding | EduThings | 🟢 Live |
| Level I Certification Earned | `credential_level_1` | Whether the student earned a Level 1 certificate (C1). | Garland - Associate Degree, Dallas College - Credentials | Dallas College | 🟢 Live |
| Level II Certification Earned | `credential_level_2` | Whether the student earned a Level 2 certificate (C2). | Garland - Associate Degree, Dallas College - Credentials | Dallas College | 🟢 Live |
 
## College application & enrollment (Promise)
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| Path Form Submitted | `path_form_submitted` | Whether the student submitted the PathForm / pledge (pledge status not ineligible). | Promise - Pledge Roster | Promise program data | 🟢 Live |
| Interest (from Path form) | `path_form_interest` | Career pathway the student is most interested in. | Promise - Pledge Roster | Promise program data | 🟢 Live |
| Senior Survey Submitted | `senior_survey` | Whether the student submitted the senior survey. | Promise - Pledge Roster | Promise program data | 🟢 Live |
| Applied | `applied` | Whether the student applied to any partner college. | Promise - Pledge Roster | Promise program data | 🟢 Live |
| Applied to 3 | `applied_three` | Whether the student applied to at least 3 partner colleges. | Promise - Pledge Roster | Promise program data | 🟢 Live |
| Financial Aid | `financial_aid_status` | Whether the student submitted FAFSA or TASFA. | Promise - Pledge Roster | Promise program data | 🟢 Live |
| Accepted | `accepted` | Whether the student was admitted to a partner college. | Promise - Pledge Roster | Promise program data | 🟢 Live |
| Enrolled | `postsecondary_enrolled` | Whether the student is enrolled at a partner college (status = Enrolled). | Promise - Pledge Roster | Promise program data | 🟢 Live |
| Advanced Diploma | `advanced_diploma` | Whether the student has an advanced diploma designation (based on graduation code plus program). | Garland - Roster | Skyward | 🟢 Live |
 
## Class Schedule
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| Class,Teacher | `class_teacher_1` | Teacher for class period 1. | Garland - Schedules | Skyward | 🟢 Live |
| Class,Teacher 2 | `class_teacher_2` | Teacher for class period 2. | Garland - Schedules | Skyward | 🟢 Live |
| Class,Teacher 3 | `class_teacher_3` | Teacher for class period 3. | Garland - Schedules | Skyward | 🔴 Not yet available |
| Class,Teacher 4 | `class_teacher_4` | Teacher for class period 4. | Garland - Schedules | Skyward | 🔴 Not yet available |
| Class,Teacher 5 | `class_teacher_5` | Teacher for class period 5. | Garland - Schedules | Skyward | 🔴 Not yet available |
| Class,Teacher 6 | `class_teacher_6` | Teacher for class period 6. | Garland - Schedules | Skyward | 🔴 Not yet available |
| Class,Teacher 7 | `class_teacher_7` | Teacher for class period 7. | Garland - Schedules | Skyward | 🔴 Not yet available |
| Class,Teacher 8 | `class_teacher_8` | Teacher for class period 8. | Garland - Schedules | Skyward | 🔴 Not yet available |
| Extra Curricular | `extracurricular` | Student's extracurricular participation. | Not provided by district | n/a | 🔴 Not yet available |
 
## Advanced coursework and Prep
 
| Column Name | Data field | What it means | Data source | Originates from | Status |
|---|---|---|---|---|---|
| Highest AP Score | `highest_ap_score` | Student's highest AP exam score across all AP subjects. | Garland - Advanced Placement | College Board | 🟢 Live |
| Highest IB Score | `highest_ib_score` | Student's highest IB score. | Not provided by district | n/a | 🔴 Not yet available |
| Highest OnRamps College Grade | `highest_onramps_grade` | Student's highest OnRamps letter grade. | OnRamps file | UT Austin OnRamps | 🟢 Live |
| College Prep Type | `college_Prep` | The college prep course pathway the student is enrolled in through Texas College Bridge. | Garland - TX English Bridge, Garland - TX Math Bridge | NROC (Texas College Bridge) | 🔴 Not yet available |
| College Prep Type 2 | `college_prep2` | A second college prep pathway, if the student is enrolled in more than one. | Garland - TX English Bridge, Garland - TX Math Bridge | NROC (Texas College Bridge) | 🔴 Not yet available |
| College Prep Math Status | TBD | The student's status in the college prep math course (Texas College Bridge), used toward TSI math readiness. | Garland - TX Math Bridge | NROC (Texas College Bridge) | 🔴 Not yet available |
| College Prep ELAR Status | TBD | The student's status in the college prep ELAR course (Texas College Bridge), used toward TSI ELAR readiness. | Garland - TX English Bridge | NROC (Texas College Bridge) | 🔴 Not yet available |
| HB3 CCMR | `ccmr_hb3` | CCMR indicator under HB3 (met both ELA and math, excluding certain cases). | Garland - Early Warning | TEA CCMR Early Warning System | 🟢 Live |
| HB3 IBC Status | `ibc_hb3` | Whether the student earned at least one Industry-Based Certification (HB3 indicator). | Garland - Early Warning | TEA CCMR Early Warning System | 🟢 Live |
| A-F Career Status | `career_af` | Career A-F accountability indicator. | Garland - Early Warning | TEA CCMR Early Warning System | 🟢 Live |

---
