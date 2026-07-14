# Differentiate Testware on ToolShop Holtesting V6

## Title

Differentiate Testware on ToolShop Holtesting V6

## Background

The Scrum team is testing the Sprint 6 increment on **ToolShop Holtesting V6** ([https://holtesting.practicesoftwaretesting.com/](https://holtesting.practicesoftwaretesting.com/)). The release adds PayU payment, delivery-cost rules, and Czech-language support to the checkout flow.

During a test-process review, the test lead asks you to **differentiate testware** — the work products created by each test activity (section 1.4.1). Several artifacts already exist in the team wiki, but labels are inconsistent. Your job is to classify each artifact to the **test activity that produces it**, not to the feature it covers.

## Reference

- ISTQB FL – 1.4.3 Testware
- ToolShop V6: [https://holtesting.practicesoftwaretesting.com/](https://holtesting.practicesoftwaretesting.com/)
- API documentation: [https://api.practicesoftwaretesting.com/api/documentation](https://api.practicesoftwaretesting.com/api/documentation)
- ToolShop documentation: [https://github.com/testsmith-io/practice-software-testing/tree/main/docs](https://github.com/testsmith-io/practice-software-testing/tree/main/docs)
- Test account: `customer@practicesoftwaretesting.com` / `welcome01`

## Tasks

1. Open ToolShop Holtesting V6, add one product to the cart, and navigate to checkout. Skim the PayU payment step and note **one observable behavior** you would cover in this sprint (for example: order-total calculation, delivery-cost display, or Czech-language labels).
2. Classify each testware item below into **exactly one** test-activity category from section 1.4.3. Use the syllabus category names only:

   - Test planning
   - Test monitoring and test control
   - Test analysis
   - Test design
   - Test implementation
   - Test execution
   - Test completion

   Write one short rationale per row.


| # | Testware item from the ToolShop V6 sprint | Test activity (1.4.3 category) | Rationale |
| - | ----------------------------------------- | ------------------------------ | --------- |
| A | Sprint test plan listing checkout scope, entry criteria, and exit criteria for PayU | | |
| B | Risk register with likelihood and impact for PayU sandbox downtime | | |
| C | Prioritized test conditions derived from the PayU user-story acceptance criteria | | |
| D | Defect report noting a wrong VAT rate in the checkout user story (test basis defect) | | |
| E | Eight checkout test cases covering PayU success, cancel, and timeout paths | | |
| F | Document listing required test data: valid card numbers, expired cards, and empty-cart edge cases | | |
| G | Playwright script that automates guest checkout through PayU | | |
| H | WireMock stub simulating PayU gateway responses for offline testing | | |
| I | Daily test progress report e-mailed to the Scrum Master | | |
| J | Test log recording three passed and one failed PayU checkout run from last night's pipeline | | |
| K | Jira defect report for wrong delivery cost shown on the cart page | | |
| L | Sprint test completion report summarizing coverage and residual risk | | |
| M | Lessons-learned note: "PayU sandbox credentials expire weekly — rotate before regression" | | |

3. Write **two distinguishing sentences** (one sentence each):
   - Explain how items **C** and **E** differ, even though both relate to PayU checkout coverage.
   - Explain how items **D** and **K** differ, even though both are defect reports.
4. Item **H** (WireMock stub) is classified under test implementation. Name **one other testware type** from section 1.4.3 that also belongs to test implementation and would support the same PayU checkout flow. One short phrase is enough.

## Expected Outcome

The completed classification table (task 2, all thirteen rows), two one-sentence distinctions (task 3), and one additional test-implementation testware type (task 4).

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
