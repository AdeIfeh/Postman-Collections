
**API Testing Documentation**

This README file documents the API testing conducted for the Ardilla Holdy and Hargon App projects. The focus was on validating the functionality and reliability of various endpoints.

**Summary**

**Objective**

To ensure the APIs meet functionality, reliability, and security requirements.

**Tools Used**

**Postman**: For endpoint testing and validations.

**Newman**: To automate test execution via CLI for CI/CD pipelines.


**Key Focus Areas**

**Authentication**

Validation of login, password reset, and session management endpoints.

**Transactions and Billing**

Ensuring accurate response for transaction histories and billing operations.

**Performance Metric**s

Monitoring response times to ensure acceptable performance.


**Endpoints Tested**

A. **Ardilla Holdy**

**Authentication**

1. **Forgot Password**

GET OTP: Ensured proper OTP generation.

Verify OTP: Confirmed validation logic and response structure.

Set Password: Verified functionality for password updates.

2. **Login**

Validated token generation and accurate response schema.

**Transactions**

1. View Personal History

Retrieved personal transaction history.

Checked for the presence of required fields like transaction_id and date_created.

2. View All User History

Verified retrieval of comprehensive user transaction data.


B. **Hargon App**

**Authentication**

1. **Forgot Password**

Initiate: Verified OTP request with phone number.

OTP Validation: Confirmed correctness and response integrity.

Set Password: Ensured security compliance during password updates.

2. **New Device Authentication**

Checked device details validation and OTP processes.

**Billing**

1. **Biller Group Enquiry**

Confirmed availability of biller groups.

Verified response schema integrity.

2. **Transaction Enquiry**

Queried transaction data for services like electricity and airtime.

**Cards**

1. **Card Initialization**

Confirmed proper setup of cards.

2. **Verify Transaction**

Validated transactions using reference numbers.


**Testing Methodology**

**Test Cases**

1. **Status Code Validation**

Verified endpoints return correct HTTP status codes (e.g., 200, 400).

2. **Response Time Checks**

Measured performance to ensure responses were within acceptable limits.

3. **Schema Validation**

Ensured responses match the defined JSON schema.

4. **Error Handling**

Tested APIs with invalid inputs to confirm proper error messages.

5. **Security Testing**

Validated bearer token-based authentication and sensitive data protection.


**Results**

**Success**: Major functionalities passed all test scenarios.

**Issues**: Minor inconsistencies in error messaging and response times were documented and shared with the development team.


**Recommendations**

1. Optimize response times exceeding 500ms.

2. Standardize error messages across endpoints.

3. Include detailed API documentation for required parameters.


**Getting Started**

**Steps to Run Tests**

1. **Import Collections**

Download the Postman collections and import them into your workspace.

2. **Configure Environment**

Set up environment variables like {{base_url}}, token, etc.

3. **Run Collections**

Execute tests via Postman or use Newman for automated testing.

4. **Analyze Results**

Review response data and logs for validation.


Feel free to reach out for any questions or further clarifications.

**Authored by:** Adebayo Elizabeth
**Role**: Software QA Engineer

