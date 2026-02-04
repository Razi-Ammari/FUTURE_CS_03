🔐 API Security Risk Analysis – Public Demo API

(Future Interns – Cyber Security Task 3)

📌 Executive Summary

Modern SaaS platforms rely heavily on APIs to power applications, integrations, and data flows. While APIs enable scalability and flexibility, insecure API designs introduce critical business risks including unauthorized data access, privacy violations, and service abuse.

This project presents a professional, read-only API Security Risk Analysis conducted on a public demo API. The goal is to identify common API security weaknesses, assess their business impact, and propose practical remediation strategies, following real-world AppSec consulting methodologies.

This work reflects how security agencies and SaaS security teams evaluate API exposure — focusing on risk identification, not exploitation.

🎯 Objectives

Analyze a public API endpoint in a safe and ethical manner

Identify common API security risks aligned with OWASP API Security Top 10

Evaluate authentication, authorization, and exposure controls

Translate technical risks into business-friendly impact explanations

Provide clear, actionable remediation recommendations

🧭 Scope & Ethics

✔ Allowed

Public / demo APIs only

Read-only requests (GET)

Header, response, and access control inspection

Documentation-based analysis

❌ Not Allowed

Exploitation or bypass attempts

Denial-of-Service testing

Attacking private or production APIs

This assessment follows ethical security consulting standards.

🛠 Tools & Technologies

Postman – API request testing & response inspection

Browser DevTools – Header and request analysis

Public Demo API – JSONPlaceholder

Markdown Documentation – Professional reporting

GitHub – Transparent project delivery

🌐 API Under Assessment

API Name: JSONPlaceholder (Public Demo API)

Base URL: https://jsonplaceholder.typicode.com

Endpoint Tested: GET /users

Authentication: None

Testing Scope: Read-only analysis

🔍 Key Security Findings

The analysis identified multiple risks commonly seen in real SaaS environments:

1️⃣ Open / Unauthenticated Endpoint — High Risk

Endpoint accessible without authentication

No API keys, tokens, or user validation required

Enables unrestricted external access

Business Impact

Unauthorized data access

Large-scale data scraping

Increased exposure to privacy incidents

2️⃣ Excessive Data Exposure — High Risk

API returns full user profiles including:

Email addresses

Phone numbers

Physical addresses

Geo-location data

Company details

Business Impact

User privacy violations

Increased phishing & social engineering risk

Regulatory and compliance concerns

3️⃣ Missing Authorization Controls — Medium–High Risk

No role-based or user-specific access control

No enforcement of data ownership

Business Impact

Horizontal data exposure

Unauthorized access to entire datasets

4️⃣ Missing Rate Limiting — Medium Risk

No evidence of request throttling or abuse prevention

Endpoint vulnerable to automation and scraping

Business Impact

Service performance degradation

Increased infrastructure costs

Potential denial-of-service scenarios

📊 Risk Classification Summary
Risk Category	Severity
Open Endpoint	High
Excessive Data Exposure	High
Missing Authorization	Medium–High
Missing Rate Limiting	Medium
🛡 Recommended Remediation Actions

Enforce authentication (API keys, OAuth 2.0, JWT)

Apply strict authorization and access control checks

Limit API responses using least privilege principles

Introduce rate limiting and request throttling

Implement API logging and monitoring

Align API security posture with OWASP API Security Top 10

📁 Repository Structure

FUTURE_CS_03/
│
├── analysis/
│   └── api_risk_analysis_users_endpoint.md
│
├── screenshots/
│   ├── step1_git_initialization.png
│   ├── step2_api_documentation_review.png
│   ├── step3_postman_launch.png
│   ├── step4_users_endpoint_exposure.png
│   └── step5_api_risk_analysis_written.png
│
├── report/
│   └── API_Security_Risk_Analysis_Report.pdf
│
└── README.md

💼 Professional Value
This project demonstrates skills directly applicable to:

AppSec Engineer

Security Analyst

SOC Analyst

SaaS Security Consultant

GRC & Risk Assessment Roles

The methodology mirrors paid API security audits performed by cybersecurity agencies and internal security teams.

📚 References (Study Only)

OWASP API Security Top 10
https://github.com/OWASP/API-Security

API Security Checklist
https://github.com/shieldfy/API-Security-Checklist

Public APIs Collection
https://github.com/public-apis/public-apis

👤 Author
Razi Ammari
Cyber Security & API Security Enthusiast
Future Interns – Cyber Security Program (2026)

🏁 Final Note
This repository showcases security thinking, risk assessment, and communication skills — the exact combination required in modern cybersecurity roles.
