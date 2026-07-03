# Playwright QA Automation Framework

Professional QA automation framework for web application testing using Playwright, Java, TestNG, REST Assured, GitHub Actions, Docker, and Allure Reports.

## Purpose

This framework demonstrates end-to-end QA automation capability across UI, API, reporting, CI/CD, and containerized execution.

It is designed to show how a real-world QA automation framework can support regression testing, smoke testing, API validation, and release confidence.

## Tech Stack

| Area | Tool |
|---|---|
| Language | Java |
| UI Automation | Playwright |
| Test Runner | TestNG |
| API Testing | REST Assured |
| Reporting | Allure |
| CI/CD | GitHub Actions |
| Containerization | Docker |
| Test Data | JSON / POJO / DataProvider |
| Design Pattern | Page Object Model |

## Framework Architecture

```text
                  TestNG
                    |
        +-----------+-----------+
        |           |           |
       UI          API       Database
        |           |           |
    Playwright  REST Assured   JDBC
        |           |           |
        +-----------+-----------+
             Base Framework
                    |
        Configuration / Utilities
                    |
        Allure / Logging / Docker
```

## Key Features

- Page Object Model
- UI automation using Playwright
- API testing using REST Assured
- Data-driven testing using JSON and POJOs
- TestNG suite execution
- Screenshot capture on failure
- Allure reporting
- GitHub Actions CI execution
- Docker execution support
- Clean folder structure
- Environment-based configuration

## Suggested Test Coverage

### UI Tests
- Login
- Registration
- Logout
- Product search
- Add to cart
- Checkout smoke flow

### API Tests
- Create user
- Verify login
- Update user
- Delete user
- Negative response validation

### E2E Tests
- Create user through API
- Login through UI
- Validate user flow
- Delete user through API
- Verify login failure after deletion

## How to Run Locally

```bash
mvn clean test
```

## Run Specific Suite

```bash
mvn clean test -DsuiteXmlFile=src/test/resources/testng.xml
```

## Generate Allure Report

```bash
allure serve allure-results
```

## Run with Docker

```bash
docker build -t qa-automation-framework .
docker run qa-automation-framework
```

## Run with Docker Compose

```bash
docker-compose up --build
```

## GitHub Actions

The framework is designed to run tests automatically on:
- Pull requests
- Main branch pushes
- Scheduled nightly execution

## Reporting Screenshots

Add screenshots under:

```text
docs/screenshots/
├── allure-report.png
├── github-actions.png
├── docker-run.png
└── test-execution.png
```

Reference them in this README using:

```markdown
![Allure Report](docs/screenshots/allure-report.png)
```

## Portfolio Value

This framework demonstrates practical automation skills required for QA/SDET roles and freelance QA automation services:
- maintainable test design
- UI and API coverage
- CI/CD integration
- reporting
- Docker execution
- professional documentation
