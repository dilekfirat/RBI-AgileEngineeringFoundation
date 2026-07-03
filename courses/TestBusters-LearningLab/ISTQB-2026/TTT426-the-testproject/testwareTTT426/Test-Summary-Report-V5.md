# Test Summary Report – V5

**ToolShop Web Application – Version 5**

## Document Information

| Field | Information |
|--------|-------------|
| Project | ToolShop Web Application |
| Team | QualityQuest Consulting (QQC) |
| Version | V5 |
| Document | Test Summary Report |
| Standard | ISO/IEC/IEEE 29119-3 |
| Author | Gülbin Deniz |
| Reviewer | Rudolf Gröetz |
| Date | 03.07.2026 |
| Status | Final |

---

## 1. Purpose

This Test Summary Report summarizes the testing activities performed for ToolShop Web Application Version 5. It provides an overview of the test scope, test execution, test results, identified defects, and the release recommendation for Version 5.

---

## 2. Test Scope

### Tested Functional Areas

- Admin Account
- Authentication
- Checkout
- Customer Account
- Product Overview
- Product Detail
- Product Category

### Features Not Tested

- Multi Language (Test cases were not completed.)
- Privacy Policy (No test cases were available.)

### Test Approach

- Risk-Based Testing
- Requirements-Based Testing
- Use Case-Based Testing
- User Acceptance Testing (UAT)
- Exploratory Testing
- Regression Testing

---

## 3. Test Execution Summary

| Metric | Result |
|---------|-------:|
| Planned Test Cases | 115 |
| Executed Test Cases | 84 |
| Passed | 75 |
| Failed | 7 |
| Blocked | 2 |
| Not Executed | 31 |

The detailed test results are documented in Testiny.

---

## 4. Test Results

The planned test activities were carried out in accordance with the Product Test Plan.

The User Acceptance Test (UAT) was successfully completed.

In addition to manual testing, automated tests were executed using Playwright. The results of the automated test runs are documented in Testiny.

---

## 5. Defect Summary

During User Acceptance Testing, several findings were identified.

| Defect | Severity | Priority | Status |
|---------|----------|----------|--------|
|  | High | P1 | Open |
|  | Medium | P2 | Fixed |
|  | Low | P3 | Open |

---

## 6. Risks and Limitations

During UAT, not all planned test cases could be executed. A total of **31 test cases** were not executed.

The following areas could not be fully tested:

- Multi Language (Test cases were not completed.)
- Privacy Policy (No test cases were available.)

---

## 7. Release Recommendation

Based on the completed testing activities and the successful completion of User Acceptance Testing (UAT), the release of ToolShop Web Application Version 5 is recommended.

---

## 8. References

- Product Test Plan V5
- Sprint Test Plan
- Testiny (Test Cases and Test Results)
- GitHub Issues (Defect Tracking)
- ISO/IEC/IEEE 29119-3

---

# Appendix

## Test Run Overview

| Test Run | Planned | Executed | Passed | Failed | Blocked | Not Executed |
|-----------|--------:|---------:|-------:|-------:|--------:|-------------:|
| CRUD | 6 | 0 | 0 | 0 | 0 | 6 |
| Reporting | 5 | 0 | 0 | 0 | 0 | 5 |
| Login | 5 | 5 | 5 | 0 | 0 | 0 |
| Two-Factor Authentication | 2 | 0 | 0 | 0 | 0 | 2 |
| Automated | 1 | 0 | 0 | 0 | 0 | 1 |
| Address Details | 6 | 6 | 5 | 0 | 1 | 0 |
| Delete Item | 5 | 5 | 5 | 0 | 0 | 0 |
| Increase/Decrease Quantity | 6 | 6 | 6 | 0 | 0 | 0 |
| Payment Options | 21 | 14 | 13 | 0 | 1 | 7 |
| Contact Form (Customer Account) | 5 | 5 | 4 | 1 | 0 | 0 |
| Customer Login | 5 | 5 | 3 | 2 | 0 | 0 |
| Favorites | 3 | 3 | 3 | 0 | 0 | 0 |
| Invoices | 3 | 3 | 3 | 0 | 0 | 0 |
| Messages | 2 | 2 | 2 | 0 | 0 | 0 |
| Profile | 4 | 4 | 0 | 4 | 0 | 0 |
| Privacy Policy | 5 | 0 | 0 | 0 | 0 | 5 |
| Multi Language | 5 | 0 | 0 | 0 | 0 | 5 |
| Product Category | 1 | 1 | 1 | 0 | 0 | 0 |
| Product Detail | 11 | 11 | 11 | 0 | 0 | 0 |
| Filter | 3 | 3 | 3 | 0 | 0 | 0 |
| Pagination | 1 | 1 | 1 | 0 | 0 | 0 |
| Price Range | 1 | 1 | 1 | 0 | 0 | 0 |
| Product List | 1 | 1 | 1 | 0 | 0 | 0 |
| Search | 5 | 5 | 5 | 0 | 0 | 0 |
| Sorting | 3 | 3 | 3 | 0 | 0 | 0 |
| **Total** | **115** | **84** | **75** | **7** | **2** | **31** |