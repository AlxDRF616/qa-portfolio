# Web Testing – SauceDemo Shopify

## Objective

Validate core user flows in a web application, focusing on form validation, user experience, and security behavior.


## Scope

- User registration
- Login functionality
- Password recovery
- Form validations


## Approach

- Executed manual test cases based on user flows
- Tested both valid and invalid inputs
- Observed UI behavior and error messages


## Key Findings

### 1. Weak Input Validation

- System accepts 1-character names
- No minimum length enforced

Impact:
- Poor data quality


### 2. UX Issue in Login

- Error message is ambiguous
- Input fields are cleared after failure

Impact:
- Increased user friction


### 3. Security Risk – User Enumeration

- System reveals when an email is not registered

Impact:
- Potential for account discovery attacks


## Technical Insight

The password reset flow exposes internal system logic, which should be abstracted using generic responses to prevent information leakage.


## Tools Used

- Browser testing
- DevTools (basic inspection)


## Repository

https://github.com/AlxDRF616/web-testing-saucedemo