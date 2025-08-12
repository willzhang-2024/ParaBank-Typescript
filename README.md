# Parabank UI & API Automation with CI/CD integrated

## Overview
This project is designed to automate end-to-end testing for a web application using Typescript and Playwright. It includes functionalities such as user registration, account creation, fund transfer, bill payment, and transaction search. In addition, CI/CD is integrated with github actions and Jenkins pipeline

Two test environments are set up: dev and qa (only qa is valid)

## Features
UI Automation
- **User Registration**: Automates the registration process and verifies success.
- **Account Management**: Opens new accounts and verifies account details.
- **Fund Transfer**: Transfers funds between accounts and validates the transaction.
- **Bill Payment**: Automates bill payment and ensures payment completion.
- **Transaction Search**: Searches for transactions based on various criteria.

API automation
- **Transaction Search by amount**: Searches for transactions based on transfer amount.
  
## Technologies Used
- **Programming Language**: Typescript
- **Framework**: Playwright
- **Dependency Management**: npm


**Set up local project**
```shell
$ git clone https://github.com/willzhang-2024/ParaBank-Typescript.git
$ cd ParaBank-Typescript
```

**Install dependencies**
```shell
npm ci
```

**Install playwright**
```shell
npx playwright install
```

**Run test**
```shell
$env:ENV='qa'
npx playwright test
```

**Project Structure**
```

├───.github
│   └───workflows
├───api
├───data
├───env
├───pages
├───tests
├───trace
├───allure-report
├───playwright-report

