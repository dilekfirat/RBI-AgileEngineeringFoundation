# Distinguish Test Types on ToolShop Holtesting V6

## Title

Distinguish Test Types on ToolShop Holtesting V6

## Background

The Scrum team is preparing test coverage for the Sprint 6 increment on **ToolShop Holtesting V6** ([https://holtesting.practicesoftwaretesting.com/](https://holtesting.practicesoftwaretesting.com/)). The checkout flow now includes PayU payment, delivery-cost rules, and Czech-language support.

During sprint planning, testers proposed many checks — but several overlap. The test lead asks you to **distinguish** the syllabus test types so the team assigns the right techniques, environments, and owners. ISTQB section 2.2.2 defines four test types: functional, non-functional, black-box, and white-box.

## Reference

- ISTQB FL – 2.2.2 Test Types
- ToolShop V6: [https://holtesting.practicesoftwaretesting.com/](https://holtesting.practicesoftwaretesting.com/)
- API documentation: [https://api.practicesoftwaretesting.com/api/documentation](https://api.practicesoftwaretesting.com/api/documentation)
- ToolShop documentation: [https://github.com/testsmith-io/practice-software-testing/tree/main/docs](https://github.com/testsmith-io/practice-software-testing/tree/main/docs)
- Test account: `customer@practicesoftwaretesting.com` / `welcome01`

## Tasks

1. Open ToolShop Holtesting V6, add one product to the cart, and navigate to checkout. Note **one functional behavior** you would verify (for example: order total calculation, PayU payment option, or delivery-cost display).
2. On the same checkout flow, note **one non-functional characteristic** you would verify (for example: page response time, usability of the payment form, or cross-browser layout).
3. Classify each test idea below into **exactly one** of the four syllabus test types. Write one short rationale per row.


| # | Test idea on ToolShop V6 | Test type (functional / non-functional / black-box / white-box) | Rationale |
| - | ------------------------ | ----------------------------------------------------------------- | --------- |
| A | Complete checkout with PayU and confirm the order-confirmation page shows the correct total | | |
| B | Measure elapsed time from clicking **Pay** to seeing the confirmation page; fail if it exceeds 3 seconds | | |
| C | Derive test cases from the PayU user-story acceptance criteria without inspecting source code | | |
| D | Achieve branch coverage on the `CartService` discount-calculation method by inspecting its source code | | |
| E | Run the checkout flow in Chrome, Firefox, and Edge and compare layout and behavior | | |
| F | Send malformed input to the login API and verify the service rejects injection attempts | | |


4. Write **two distinguishing sentences** (one sentence each):
   - Explain how test ideas **A** and **B** differ, even though both use the same checkout flow.
   - Explain how test ideas **C** and **D** differ, even though both target cart/checkout logic.
5. State **one test level** (from section 2.2.1) where test idea **D** would typically run, and **one test level** where test idea **A** would typically run. One short phrase per answer is enough.

## Expected Outcome

The completed classification table (task 3, all six rows), two one-sentence distinctions (task 4), and two test levels (task 5).

## Original Syllabus K-Level

K2

## Original Syllabus Text

A lot of test types exist and can be applied in projects. In this syllabus, the following four test types are addressed:

**Functional testing** evaluates the functions that a component or system should perform. The functions are "what" the test object should do. The main objective of functional testing is checking the functional completeness, functional correctness and functional appropriateness.

**Non-functional testing** evaluates attributes other than functional characteristics of a component or system. Non-functional testing is the testing of "how well the system behaves". The main objective of non-functional testing is checking the non-functional quality characteristics. The ISO/IEC 25010 standard provides the following classification of the non-functional quality characteristics:

- Performance efficiency
- Compatibility
- Usability (also known as interaction capability)
- Reliability
- Security
- Maintainability
- Portability (also known as flexibility)
- Safety

It is sometimes appropriate for non-functional testing to start early in the SDLC (e.g., as part of reviews or component testing). Many non-functional tests are derived from functional tests as they use the same functional tests, but check that while performing the function, a non-functional constraint is satisfied (e.g., checking that a function performs within a specified time, or a function can be ported to a new platform). The late discovery of non-functional defects can pose a serious threat to the success of a project. Non-functional testing sometimes needs a very specific test environment, such as a usability lab for usability testing.

**Black-box testing** (see section 4.2) is specification-based and derives tests from documentation not related to the internal structure of the test object. The main objective of black-box testing is checking the system's behavior against its specifications.

**White-box testing** (see section 4.3) is structure-based and derives tests from the system's implementation or internal structure (e.g., code, architecture, work flows, and data flows). The main objective of white-box testing is to cover the underlying structure by the tests to an acceptable level.

All the four above mentioned test types can be applied to all test levels, although the focus will be different at each level. Different test techniques can be used to derive test conditions and test cases for all the mentioned test types.
