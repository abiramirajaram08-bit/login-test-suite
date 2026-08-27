# Test Plan — Login Form Test Suite

## Application Under Test
saucedemo.com — login page

## Objective
Verify the login functionality works correctly for valid, invalid, edge-case, and security-related inputs.

## Scope
- In scope: Username field, password field, Login button, error messages, logout, session handling on browser back
- Out of scope: Signup, forgot password, product pages, checkout flow

## Test Approach
Manual black-box testing using:
- **Equivalence Partitioning** — grouping valid/invalid input classes (valid user, invalid user, locked-out user, empty fields)
- **Boundary Value Analysis** — testing edges of accepted input (empty vs filled, case sensitivity)
- **Security testing basics** — SQL injection and XSS input attempts on the login form

## Test Environment
- Browser: Chrome (latest)
- URL: https://www.saucedemo.com
- Test accounts: standard_user, locked_out_user (both with password `secret_sauce`)

## Entry Criteria
- Login page is accessible and loads without errors

## Exit Criteria
- All 18 planned test cases executed
- All identified defects logged with severity/priority

## Deliverables
- test-cases.xlsx — full test case sheet with results
- bug-reports.md — any defects found during execution
- README.md — project summary and findings
