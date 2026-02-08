# Secure_api_testing
Secure API authentication testing using Postman, including invalid credential handling, HTTP response analysis, and OWASP API Security mapping.

# API Security Testing Report 

## Objective
To test REST API authentication mechanisms and observe authorization behavior using valid and invalid inputs.

## Tools Used
- Postman
- Public Test API (ReqRes)

## API Tested
Endpoint:
POST https://reqres.in/api/register

## Tests Performed

### 1. Authentication Testing
- Sent registration request with missing password
- Observed server response

### 2. Invalid Credential Handling
- API correctly returned 400 Bad Request
- Error response confirms authentication enforcement

## Findings

| Test Case | Result | Risk |
|---------|------|------|
| Invalid registration | 400 Bad Request | Low |

## OWASP API Security Mapping
- API2: Broken Authentication (Tested – Not vulnerable)

## Conclusion
The API correctly validates input and rejects invalid authentication attempts, demonstrating proper authentication controls.
