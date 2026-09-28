# QA Final Project – Urban Scooter & Urban Routes

Manual and API testing project developed during the **TripleTen QA Engineering Bootcamp**.
It covers the full QA cycle: test design, checklists, test cases, bug reports, API testing,
and SQL data validation on two related products:

- **Urban Scooter** – a scooter rental web app + courier mobile app (Android).
- **Urban Routes** – a ride-hailing web app (used for test automation with Selenium).

---

## Table of Contents

- [Objective](#objective)
- [Scope](#scope)
- [Tools & Technologies](#tools--technologies)
- [Repository Structure](#repository-structure)
- [Project Breakdown](#project-breakdown)
  - [1. Test Design Theory](#1-test-design-theory)
  - [2. Manual Testing – Urban Scooter](#2-manual-testing--urban-scooter)
  - [3. Test Cases – Mobile App](#3-test-cases--mobile-app)
  - [4. API Testing – Urban Scooter Backend](#4-api-testing--urban-scooter-backend)
- [Key Findings](#key-findings)
- [How to Use This Repository](#how-to-use-this-repository)
- [Author](#author)

---

## Objective

Apply QA theory and practice to real-world scenarios:

- Analyze requirements and detect gray areas before designing tests.
- Design effective test coverage using equivalence classes, boundary values,
  decision tables, and checklists.
- Report and track defects with clear, reproducible bug reports.
- Validate REST APIs with Postman (status codes, payloads, error handling).
- Validate backend data with SQL queries.

---

## Scope

| Area | Product | Type |
|------|---------|------|
| Manual testing | Urban Scooter (web + mobile) | Functional, UI, cross-browser |
| Test design | Urban Scooter | Checklists, test cases, data validation |
| API testing | Urban Scooter backend | REST endpoints (Postman) |
| Database validation | Urban Scooter backend | SQL (PostgreSQL) |
| Automation | Urban Routes (web) | Selenium + Python (POM) |

---

## Tools & Technologies

- **Test management:** Jira (bug tracking)
- **API testing:** Postman
- **Database:** PostgreSQL, `psql`
- **Mobile testing:** Android emulator (Pixel 9 Pro, API 37.2)
- **Browsers:** Google Chrome, Mozilla Firefox
- **Automation:** Python, Selenium WebDriver, pytest
- **Documentation:** Google Sheets / Excel, Markdown

---

## Repository Structure
