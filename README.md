# OrangeHRM - Manual Testing (Login and PIM Modules)

Manual test cases and execution results for the **OrangeHRM public demo** (https://opensource-demo.orangehrmlive.com), covering the Login page and the PIM (Employee) module.

## Project Summary
| Item | Details |
|---|---|
| Application | OrangeHRM open source demo |
| Test type | Manual: functional, negative, UI, security, compatibility |
| Total test cases | 60 (Login 40, PIM 20) |
| Result | 57 Pass, 3 Blocked, 0 Fail |

## Modules Covered
| Module | Test cases | Pass | Blocked |
|---|---:|---:|---:|
| Login | 10 | 10 | 0 |
| Logout | 1 | 1 | 0 |
| UI | 6 | 6 | 0 |
| Input Validation | 10 | 10 | 0 |
| Usability | 3 | 1 | 2 |
| Compatibility | 2 | 2 | 0 |
| Session | 4 | 3 | 1 |
| Security | 4 | 4 | 0 |
| PIM (Employee) | 20 | 20 | 0 |
| **Total** | **60** | **57** | **3** |

## Highlights
- **Security:** SQL injection, XSS input, password masking, multiple failed logins, direct dashboard URL without login.
- **Input validation:** blank, space-only, special-character and very long (300+ characters) inputs.
- **Compatibility:** worked the same across multiple browsers; responsive layout checked on a phone browser.
- **PIM:** add employee (valid, blank and over-length names, duplicate Employee Id, login details rules, photo upload), search and filters, edit, delete.

## Blocked Test Cases
| Test case | Reason |
|---|---|
| TC_026 (Tab navigation), TC_039 (keyboard-only login) | Needed a physical keyboard |
| TC_032 (session timeout) | Needed a long idle wait |

## Notes
- No defects were found in the tested scenarios.
- Observation: no account lockout or CAPTCHA appeared after 5 failed login attempts.
- One first-run 404 on the dashboard URL was caused by a mistyped URL; the retest with the correct URL redirected to the login page.

## Files
- `OrangeHRM_Test_Cases.xlsx`: test cases in a standard template (Scenario ID, Test Case ID, Pre Condition, Steps, Expected Result, Actual Result, Status, Priority) with a Summary sheet.

## Tools and Skills
Microsoft Excel, Git, GitHub. Test case design, functional testing, security testing, input validation, cross-browser and responsive testing, test documentation.

## Author
**Rushikesh Garje**, QA Analyst (fresher)
[LinkedIn](https://www.linkedin.com/in/rushikesh-garje-450a9239a) | 
