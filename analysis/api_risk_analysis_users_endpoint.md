# API Security Risk Analysis — Users Endpoint

## API Overview
- API Name: JSONPlaceholder (Public Demo API)
- Endpoint Tested: GET /users
- Base URL: https://jsonplaceholder.typicode.com
- Authentication: None
- Tool Used: Postman
- Scope: Read-only analysis (no exploitation)

## Identified Security Risks

### Risk 1 — Open / Unauthenticated Endpoint
*Observation:*
The /users endpoint is publicly accessible without any authentication mechanism such as API keys, tokens, or user sessions.

*Security Risk:*
Any external party can access sensitive user-related data without authorization.

*Business Impact:*
- Unauthorized data access
- Data scraping at scale
- Increased exposure to privacy-related incidents

*Risk Severity:* 🔴 High

---

### Risk 2 — Excessive Data Exposure
*Observation:*
The API response exposes full user profiles including:
- Full name
- Email address
- Phone number
- Physical address
- Geo-location coordinates
- Company details

*Security Risk:*
The API violates the principle of least privilege by returning more data than typically required by clients.

*Business Impact:*
- User privacy violations
- Increased risk of phishing and social engineering
- Regulatory compliance concerns

*Risk Severity:* 🔴 High

---

### Risk 3 — Missing Authorization Controls
*Observation:*
There are no role-based or user-specific access controls applied to the endpoint.

*Security Risk:*
All users’ data is accessible regardless of requester identity or permissions.

*Business Impact:*
- Horizontal data exposure
- Unauthorized access to entire datasets

*Risk Severity:* 🟠 Medium–High

---

### Risk 4 — No Rate Limiting Controls
*Observation:*
The API does not indicate any rate limiting or request throttling mechanisms.

*Security Risk:*
The endpoint may be abused through automated scraping or high-volume requests.

*Business Impact:*
- Service performance degradation
- Increased infrastructure costs
- Potential denial-of-service scenarios

*Risk Severity:* 🟡 Medium

---

## Risk Classification Summary

| Risk | Severity |
|-----|----------|
| Open Endpoint | High |
| Excessive Data Exposure | High |
| Missing Authorization | Medium–High |
| Missing Rate Limiting | Medium |

## Recommended Remediation Actions

- Implement authentication mechanisms such as API keys, OAuth 2.0, or JWT tokens.
- Enforce authorization checks to ensure users can only access their own data.
- Apply the principle of least privilege by limiting exposed response fields.
- Introduce rate limiting and request throttling to prevent abuse.
- Monitor API usage and implement logging and alerting for abnormal behavior.
- Regularly review API security posture using OWASP API Security Top 10 guidelines
