# Differentiate Testware on ToolShop Holtesting V6

## Title

Differentiate Testware on ToolShop Holtesting V6

## Background

The Scrum team is testing the Sprint 6 increment on **ToolShop Holtesting V6** ([https://holtesting.practicesoftwaretesting.com/](https://holtesting.practicesoftwaretesting.com/)). The release adds PayU payment, delivery-cost rules, and Czech-language support to the checkout flow.

Before sprint testing starts, the test lead asks you to map **testware** to the **test activities** that produce it (section 1.4.1). The team wiki mixes planning documents, scripts, and reports without clear labels. Your job is to differentiate testware by naming **one representative artifact per test activity** for this checkout scope — using syllabus terms only, not team nicknames.

## Reference

- ISTQB FL – 1.4.3 Testware
- ToolShop V6: [https://holtesting.practicesoftwaretesting.com/](https://holtesting.practicesoftwaretesting.com/)
- API documentation: [https://api.practicesoftwaretesting.com/api/documentation](https://api.practicesoftwaretesting.com/api/documentation)
- ToolShop documentation: [https://github.com/testsmith-io/practice-software-testing/tree/main/docs](https://github.com/testsmith-io/practice-software-testing/tree/main/docs)
- Test account: `customer@practicesoftwaretesting.com` / `welcome01`

## Tasks

1. Open ToolShop Holtesting V6, add one product to the cart, and navigate to checkout. Skim the PayU payment step and note **one observable behavior** you would cover in this sprint (for example: order-total calculation, delivery-cost display, or Czech-language labels).
2. For **each test activity** listed below, select **exactly one** testware type from section 1.4.3 that belongs to that activity. Use the official syllabus names (for example: *test plan* for test planning, *test cases* for test design). Do not reuse the same testware type for two different activities.

   Complete the table with one short sentence per row explaining how that artifact would apply to your checkout behavior from task 1.


| Test activity (1.4.1) | Testware artifact (1.4.3 syllabus term) | How it applies to ToolShop V6 checkout |
| --------------------- | --------------------------------------- | -------------------------------------- |
| Test planning | | |
| Test monitoring and test control | | |
| Test analysis | | |
| Test design | | |
| Test implementation | | |
| Test execution | | |
| Test completion | | |

3. Write **two distinguishing sentences** (one sentence each):
   - Explain why your **test analysis** artifact differs from your **test design** artifact, even though both relate to the same checkout behavior.
   - Explain why a **defect report regarding a defect in the test basis** (test analysis) differs from a **defect report** produced during test execution, even though both are called defect reports.

## Expected Outcome

One completed table with **seven rows** — exactly **one testware artifact per test activity** (for example: test planning → test plan; test design → test cases; test execution → test log) — plus two one-sentence distinctions (task 3).

## Original Syllabus K-Level

K2

## Original Syllabus Text

Testware is created as output work products from the test activities described in section 1.4.1. There is a significant variation in how different organizations produce, shape, name, organize and manage their work products. Proper configuration management (see section 5.4) ensures consistency and integrity of work products. The following list of work products is not exhaustive:

- Test planning work products include: test plan, test schedule, risk register, entry criteria and exit criteria (see section 5.1). Risk register is a list of risks together with risk likelihood, risk impact and information about risk mitigation (see section 5.2). Test schedule, risk register, entry criteria and exit criteria are often a part of the test plan.
- Test monitoring and test control work products include: test progress reports (see section 5.3.2), documentation of control directives (see section 5.3) and information about risks (see section 5.2).
- Test analysis work products include: (prioritized) test conditions (e.g., acceptance criteria, see section 4.5.2), and defect reports regarding defects in the test basis (if not fixed directly).
- Test design work products include: (prioritized) test cases, test charters, coverage items, test data requirements and test environment requirements.
- Test implementation work products include: test procedures, manual and automated test scripts, test suites, test data, test execution schedule, and test environment items. Examples of test environment items include: stubs, drivers, simulators, and service virtualizations.
- Test execution work products include: test logs, and defect reports (see section 5.5).
- Test completion work products include: test completion report (see section 5.3.2), action items for improvement of subsequent projects or iterations, documented lessons learned, and change requests (e.g., as product backlog items).
