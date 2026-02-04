🔐 API Security Risk Analysis

Cyber Security Task 3 – Future Interns (2026)

📌 Project Overview

This project presents a professional API Security Risk Analysis performed on a public demo API, following a real-world SaaS security assessment methodology.
The objective is to identify common API security weaknesses, explain their business impact, and propose clear remediation strategies — without exploiting or attacking systems.

This task reflects how security agencies, AppSec teams, and SaaS consultants perform read-only API risk assessments for clients.

🎯 Objectives

Analyze public/demo APIs safely and ethically

Identify common API security risks

Assess authentication & authorization weaknesses

Evaluate data exposure risks

Explain security issues in business-friendly language

Provide actionable remediation recommendations

🛡️ Scope & Ethics

Allowed

Public/demo APIs only

Read-only requests (GET)

Documentation-based analysis

Header, response, and access inspection

Not Allowed

Exploitation or bypass attempts

DoS or stress testing

Testing private or production APIs

✔ This project follows ethical security research principles.

🧪 API Tested

API Name: JSONPlaceholder (Public Demo API)

Base URL: https://jsonplaceholder.typicode.com

Endpoint Analyzed: GET /users

Authentication: None

Purpose: Identify real-world API security risks

🛠️ Tools Used

Postman – API request testing & response inspection

Browser DevTools – Header and response analysis

Markdown / PDF – Professional documentation

🔍 Methodology

Review API documentation

Identify exposed endpoints

Test endpoints using Postman

Inspect authentication & authorization mechanisms

Analyze response data for overexposure

Identify missing security controls

Classify risks by severity

Propose remediation actions

🚨 Identified Security Risks
Risk	Severity
Open / Unauthenticated Endpoint	🔴 High
Excessive Data Exposure	🔴 High
Missing Authorization Controls	🟠 Medium-High
Missing Rate Limiting	🟡 Medium
Key Findings

Public access to user data without authentication

Exposure of sensitive personal information

No role-based or user-specific access control

No visible request throttling or abuse prevention

🧩 Business Impact

Unauthorized access to sensitive data

Increased phishing & social engineering risk

Privacy and regulatory compliance concerns

Service abuse and performance degradation

Higher operational and infrastructure costs

🛠️ Recommended Remediation

Implement authentication (API keys, OAuth 2.0, JWT)

Enforce authorization checks per user and role

Apply least-privilege and data minimization

Introduce rate limiting and throttling

Enable logging, monitoring, and alerting

Regularly review APIs using OWASP API Security Top 10

📂 Repository Structure
FUTURE_CS_03/
│
├── analysis/
│   └── api_risk_analysis_users_endpoint.md
│
├── report/
│   └── API_Security_Risk_Analysis_Report.pdf
│
├── screenshots/
│   ├── step1_git_initialization.png
│   ├── step2_api_documentation_review.png
│   ├── step3_postman_launch.png
│   ├── step4_users_endpoint_postman.png
│   └── step5_api_risk_analysis_written.png
│
└── README.md

📸 Screenshots Included

Git repository initialization

API documentation review

Postman setup and launch

Users endpoint response analysis

Written API risk analysis

Each screenshot is referenced directly inside the report for traceability.

📚 References (Study Only)

OWASP API Security Top 10
https://github.com/OWASP/API-Security

Public APIs for Testing
https://github.com/public-apis/public-apis

JSONPlaceholder API
https://jsonplaceholder.typicode.com

✅ Final Notes

This project demonstrates modern API security thinking, focusing on:

Risk identification (not exploitation)

Business impact analysis

Client-ready documentation

SaaS security fundamentals

🎯 Strong fit for:

AppSec Engineer

Security Analyst

SaaS Security Consultant
