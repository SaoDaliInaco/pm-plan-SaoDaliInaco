# Business case: live quizzes for the IT department

## 1. Problem

Lecturers in the IT department manually mark paper quizzes and basic assignments, causing heavy administrative delays and lacking real-time insight into student comprehension during lectures.

Assumptions:

- Lecturers running quizzes: 10
- Marking time per lecturer per week: 1 h
- Teaching weeks per year: 30
- Total manual marking hours per year: 300 hours
- Notional value of one hour: 10 USD (used as a benchmark for comparison)

## 2. Options

| Option | Description                              | One-off cost | Annual cost | Annual benefit |
| ------ | ---------------------------------------- | ------------ | ----------- | -------------- |
| A      | Do nothing                               | 0 USD        | 0 USD       | 0 USD          |
| B      | Buy SaaS (e.g., Kahoot/Quizizz Edu Plan) | 0 USD        | 1,800 USD   | 3,000 USD      |
| C      | Build Realtime Quiz platform             | 4,900 USD    | 300 USD     | 4,800 USD      |

_Note: Option B assumes 10 lecturer seats at 15 USD/month for 12 months (1,800 USD/year). Option C one-off cost includes 490 student/PM hours at 10 USD notional rate (4,900 USD)._

## 3. Comparison

| Option | Net annual benefit              | Payback (years)            | Sensitivity (6 lecturers)                     |
| ------ | ------------------------------- | -------------------------- | --------------------------------------------- |
| B      | 3,000 - 1,800 = 1,200 USD       | 0.00 (immediate)           | 1,800 - 1,080 = 720 USD                       |
| C      | 3,000 + 1,800 - 300 = 4,500 USD | 4,900 / 4,500 = 1.09 years | Net Benefit = 3,300 USD; Payback = 1.48 years |

## 4. Benefits not priced

- Complete in-house data ownership and student privacy control.
- No per-seat or per-student licensing limitations.
- Valuable practical capstone experience for software engineering students.

## 5. Risks per option

- **Option A:** Continued low student engagement and high ongoing grading workload.
- **Option B:** Vendor price hikes, recurring annual budget dependencies, potential data privacy issues with third-party hosting.
- **Option C:** Technical delivery risks (WebSocket delays, timer drift, Khmer font rendering in PDF exports) and potential project delay beyond week 14.

## 6. Recommendation and review gate

**Recommendation:** Proceed with **Option C (Build Realtime Quiz)**. Option C provides a full payback within 1.09 years, secures long-term institutional data ownership, and avoids external SaaS fees while fulfilling student learning objectives.

**Review Gate:** If the MVP demo in Week 7 fails to meet the core Must criteria, the project will pause, and the department will purchase Option B (SaaS) for the following semester while converting Option C into a two-semester academic effort.
