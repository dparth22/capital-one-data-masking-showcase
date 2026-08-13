# Data Masking & Analytics Portal — Capital One-Sponsored Senior Capstone

A Django-based data portal built to manage and analyze customer records containing PII and financial data, developed as a 4-person senior capstone project sponsored by Capital One. Presented at VCU's Capstone Expo 2026.

**The full source code lives in a private repository** (created through GitHub Classroom and locked to the course organization), so this repo exists to showcase the project through a demo video and a written breakdown of my specific contributions.

## Demo Video

**[Watch the 5-minute demo](https://youtu.be/iekY0t65zGM)**

## What the project does

The portal lets authorized users manage and analyze customer records containing sensitive data, including names, emails, phone numbers, dates of birth, SSNs, credit card numbers, and addresses, while keeping that data masked and access-controlled.

## My contributions

I worked on a 4-person team. My specific focus was:

- **SQL and Django ORM querying, filtering, and pagination.** Built the structured querying layer for retrieving customer records, including sorting (by last/first name) and paginated results (15 records per page).
- **Data masking transformation logic.** Built the workflows that mask SSNs, credit card numbers, phone numbers, and dates of birth, while preserving specific fields (like the last four digits of a card or SSN) needed for identification and analysis.
- **Role-based access views and audit logging.** Implemented views that restrict what data a user can see based on their role, and built the audit logging system that records user, role, action taken, customer reference, IP address, and timestamp, to support data governance and monitoring.
- **Django UI.** Built out portions of the front-end views for the portal.

Database schema design and the Docker/AWS deployment pipeline were handled primarily by other members of the team.

## Tech stack

Python, Django, SQL, PostgreSQL, SQLite, AWS, Docker

## Team

4-person team, presented at VCU's Capstone Expo 2026.
