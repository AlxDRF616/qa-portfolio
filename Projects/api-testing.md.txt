# API Testing – JSONPlaceholder

## Objective

Perform functional testing on a public REST API to validate correct behavior, error handling, and data validation.


## Scope

- GET endpoints validation
- POST endpoint behavior
- Positive and negative scenarios
- Response status codes


## Approach

- Designed test cases for valid and invalid requests
- Used Postman to send requests and analyze responses
- Compared expected vs actual behavior


## Key Findings

### 1. Missing Input Validation (Critical)

- Endpoint accepts empty or null fields
- Returns '201 Created' instead of validation error

Impact:
- Risk of inconsistent or corrupted data


## Technical Insight

The API does not enforce server-side validation, which highlights the importance of backend data validation even when frontend controls exist.


## Tools Used

- Postman
- REST API
- HTTP methods (GET, POST)


## Repository

https://github.com/AlxDRF616/api-testing-jsonplaceholder