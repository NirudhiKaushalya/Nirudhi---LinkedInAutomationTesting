# LinkedIn Automation Testing

## Project Overview

This project automates selected LinkedIn login and search functionalities using Selenium WebDriver, Java, and TestNG. It demonstrates automated functional testing, validation, assertions, and screenshot capture.

## Technologies Used

- Java 21
- Selenium WebDriver 4.27.0
- TestNG 7.10.2
- Maven
- IntelliJ IDEA
- Google Chrome

## Project Structure

```text
LinkedInAutomationTesting/
├── src/test/java/
│   ├── base/
│   │   └── BaseTest.java
│   ├── pages/
│   │   ├── LoginPage.java
│   │   └── SearchPage.java
│   └── tests/
│       ├── LoginTest.java
│       ├── SearchTest.java
│       └── SearchResultTest.java
├── test-screenshots/
│   ├── PASSED/
│   └── FAILED/
├── pom.xml
└── testng.xml
```

## Automated Test Cases

| Test ID | Description |
|---|---|
| TC01 | Verify login page loads |
| TC02 | Verify empty login form validation |
| TC03 | Verify password visibility toggle |
| TC04 | Verify invalid email format validation |
| TC05 | Verify empty password validation |
| TC06 | Verify invalid login credentials |
| TC07 | Verify successful login |
| TC08 | Verify LinkedIn search functionality |
| TC09 | Verify search result navigation |

## How to Execute

1. Clone or download the repository.
2. Open the project in IntelliJ IDEA.
3. Ensure Java 21 and Maven dependencies are configured.
4. Configure the `LINKEDIN_EMAIL` and `LINKEDIN_PASSWORD` environment variables in the test run configuration.
5. Open `testng.xml`.
6. Right-click and select **Run**.

## Screenshot Capture

The automation framework captures screenshots after test execution and organizes them into `PASSED` and `FAILED` folders according to the TestNG result. Screenshot filenames include timestamps.

## Test Execution Results

Final execution date: November 5, 2026.

- Total tests: 9
- Passed: 8
- Failed: 1
- Skipped: 0
- Pass rate: 88.89%

The invalid login credentials test (TC06) encountered a timeout while waiting for the expected error message.

## Conclusion

The project demonstrates automated functional testing of LinkedIn login and search workflows using Selenium WebDriver and TestNG. It also includes reusable page classes and automatic screenshot capture to support test execution and reporting.
