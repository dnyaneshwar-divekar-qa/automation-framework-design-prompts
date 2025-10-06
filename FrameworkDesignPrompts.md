
# 1) Selenium Web Automation Framework
using **Java, Selenium WebDriver, TestNG, Maven, and Extent Reports (HTML reporting)** 

---

### 🧠 **Final ChatGPT Prompt**

> Act as an experienced QA Automation Lead and create a complete, production-ready **Web Automation Framework** using **Java**, **Selenium WebDriver**, **TestNG**, **Maven**, and **Extent Reports (HTML reporting)**.
>
> ✅ **Requirements:**
>
> 1. Use proper **Maven project structure**:
>
>    ```
>    src/main/java  
>    src/test/java  
>    src/test/resources  
>    ```
> 2. Include a fully working **pom.xml** with dependencies for:
>
>    * Selenium Java
>    * TestNG
>    * WebDriverManager
>    * ExtentReports
>    * SLF4J (for cleaner logs)
> 3. Implement the following classes with clear, modular code:
>
>    * `BaseTest.java` → Setup and teardown of WebDriver, Extent Reports initialization, and helper logging methods (`logInfo`, `logPass`, `logFail`).
>    * `ExtentManager.java` → Configures and manages ExtentReports instance.
>    * `ExtentTestListener.java` → Implements TestNG `ITestListener` for reporting test events.
>    * `LoginPage.java` → Page Object Model (POM) for login elements and actions.
>    * `HomePage.java` → Represents the landing page after successful login.
>    * `ConfigReader.java` → Loads data from `config.properties`.
>    * `LoginTest.java` → A sample test validating the login flow for
>      [https://opensource-demo.orangehrmlive.com/web/index.php/auth/login](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login).
> 4. Add a **config.properties** file with parameters like:
>
>    ```properties
>    base.url=https://opensource-demo.orangehrmlive.com/web/index.php/auth/login
>    username=Admin
>    password=admin123
>    browser=chrome
>    report.path=reports
>    ```
> 5. Create a working **testng.xml** that executes the login test.
> 6. Integrate **Extent Reports** to generate a **beautiful HTML report** after every execution (ensure `ExtentTest` is never null — fix listener linkage).
> 7. Implement a **Page Object Model (POM)** pattern (each page should have its own class).
> 8. Include screenshots on failure in the Extent Report.
> 9. Make sure the framework runs from command line using:
>
>    ```
>    mvn clean test
>    ```
> 10. Provide clear **comments in all classes** for easy understanding by beginners.
>
> 🎯 **Expected Output:**
>
> * Full Maven folder structure
> * All Java class codes
> * `pom.xml`
> * `config.properties`
> * `testng.xml`
> * Example HTML report output path
> * Instructions on how to execute tests and view results
>
> The final output must be **fully runnable in Eclipse or IntelliJ** without any manual fixes.

---


# 2) BDD Cucumber Selenium Framework
  using **Java, Maven, TestNG (optional), and Extent Reports (HTML reporting)**

---

### 🧠 **Final ChatGPT Prompt — BDD Cucumber Web Automation Framework**

> Act as an experienced QA Automation Lead and create a complete, production-ready **BDD Cucumber Web Automation Framework** using **Java**, **Selenium WebDriver**, **Cucumber (Gherkin)**, **Maven**, and **Extent Reports (HTML reporting)**.
>
> ✅ **Requirements:**
>
> 1. Use the proper **Maven project folder structure**:
>
>    ```
>    src/main/java  
>    src/test/java  
>    src/test/resources  
>    ```
> 2. Include a correct **pom.xml** file with dependencies for:
>
>    * Selenium Java
>    * Cucumber Java
>    * Cucumber TestNG
>    * TestNG
>    * WebDriverManager
>    * ExtentReports
>    * SLF4J (for cleaner logging)
> 3. Implement the following framework structure and files:
>
>    * **Base Classes:**
>
>      * `BaseTest.java` → WebDriver setup & teardown, Extent Reports initialization, logging helper methods (`logInfo`, `logPass`, `logFail`, screenshot capture).
>      * `ExtentManager.java` → Creates and configures the ExtentReports instance.
>      * `ExtentCucumberAdapter.java` → Integrates Cucumber results with Extent Reports.
>      * `ConfigReader.java` → Reads configuration values from `config.properties`.
>    * **Page Object Model (POM):**
>
>      * `LoginPage.java` → Page class with locators & methods for the OrangeHRM login page.
>      * `HomePage.java` → Represents the landing page after successful login.
>    * **Step Definition Classes:**
>
>      * `LoginSteps.java` → Contains step definitions for login feature.
>    * **Runner Class:**
>
>      * `TestRunner.java` → Cucumber TestNG runner file with proper glue paths and Extent adapter plugin.
>    * **Feature Files (BDD Scenarios):**
>
>      * `src/test/resources/features/Login.feature` → Contains a valid login scenario for
>        [https://opensource-demo.orangehrmlive.com/web/index.php/auth/login](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)
> 4. Add a **config.properties** file with:
>
>    ```properties
>    base.url=https://opensource-demo.orangehrmlive.com/web/index.php/auth/login
>    username=Admin
>    password=admin123
>    browser=chrome
>    report.path=reports
>    ```
> 5. Integrate **Extent Reports** using the **Extent Cucumber Adapter** to produce a **beautiful HTML report** with scenario, step, and screenshot details.
> 6. Ensure screenshot capture on test failure or step failure.
> 7. The framework should support running both from IDE and CLI using:
>
>    ```
>    mvn clean test
>    ```
> 8. Include **comments** throughout the code to help beginners understand each part.
> 9. The final framework should follow clean coding and reusability principles (POM + BDD + reporting).
>
> 🎯 **Expected Output:**
>
> * Full Maven project folder structure
> * All Java class codes
> * `pom.xml`
> * `config.properties`
> * `Login.feature` file with sample scenario
> * `testng.xml` (if TestNG integration is used)
> * Report output path (e.g., `reports/ExtentReport.html`)
> * Clear step-by-step instructions to run and view results.
>
> The final result must be **copy-paste runnable in Eclipse or IntelliJ** without any manual fixes.

---



# 3) API Test Automation Framework
  using **Java**, **RestAssured**, **TestNG**, **Maven**, and **Extent Reports (HTML reporting)**.
---

### 🧠 **Final ChatGPT Prompt**

> Act as an experienced QA Automation Lead and create a complete, production-ready **API Test Automation Framework** using **Java**, **RestAssured**, **TestNG**, **Maven**, and **Extent Reports (HTML reporting)**.
>
> ✅ Requirements:
>
> 1. Use proper **Maven folder structure** (`src/main/java`, `src/test/java`, `src/test/resources`).
> 2. Include a **pom.xml** with all correct dependencies for RestAssured, TestNG, Jackson, ExtentReports, and SLF4J.
> 3. Create the following **Java classes** with clean, reusable code:
>
>    * `BaseTest.java` → Common setup, teardown, and Extent logging methods (`logInfo`, `logPass`, `logFail`, `logApiResponse`).
>    * `ExtentManager.java` → Handles report creation and configuration.
>    * `ExtentTestListener.java` → Implements TestNG listeners (`onTestStart`, `onTestSuccess`, etc.) and integrates ExtentReports.
>    * `ConfigReader.java` → Reads values from a `config.properties` file.
>    * `GetUserTest.java` → A sample API test (`GET /users`) using base URL and token from `config.properties`.
> 4. Add a **config.properties** file with:
>
>    * `base.url=https://thinking-tester-contact-list.herokuapp.com`
>    * `auth.token=Bearer <sample_token>`
>    * `env=QA`
>    * `report.path=reports`
> 5. Integrate **Extent Reports** properly to generate an HTML report after test execution.
> 6. Ensure the framework **does not throw NullPointerException** for ExtentTest logging (fix listener/test linking).
> 7. Provide one working **testng.xml** to execute all tests.
> 8. Include comments for every file for beginner understanding.
>
> 🎯 Output should include:
>
> * Full folder structure
> * All Java file codes
> * `pom.xml`
> * `config.properties`
> * `testng.xml`
> * Instructions on how to run the project (`mvn clean test`)
> * Example report generation path and result message
>
> The output should be **fully copy-paste runnable in Eclipse or IntelliJ** without any modification.

---

# 4) Cypress Web Automation Framework 
  using **JavaScript** in **VS Code**, following best QA Lead practices

### 🧠 **Final ChatGPT Prompt — Cypress Web Automation Framework (JavaScript, VS Code)**

> Act as an experienced QA Automation Lead and create a complete, production-ready **Cypress Web Automation Framework** using **JavaScript** in **VS Code**.
>
> ✅ **Requirements:**
>
> 1. Use **Cypress (latest stable version)** with a clean project setup initialized via `npm init -y` and `npm install cypress --save-dev`.
> 2. Include all required dependencies and dev tools in `package.json`, such as:
>
>    * `cypress`
>    * `cypress-mochawesome-reporter` (for HTML reports)
>    * `dotenv` (for environment variables)
>    * `eslint` (for code quality)
> 3. Use a **Page Object Model (POM)** design pattern with the following folder structure:
>
>    ```
>    cypress/
>      ├── e2e/
>      │   └── tests/
>      │       └── loginTest.cy.js
>      ├── pages/
>      │   ├── LoginPage.js
>      │   └── HomePage.js
>      ├── fixtures/
>      │   └── credentials.json
>      ├── support/
>      │   ├── commands.js
>      │   ├── e2e.js
>      │   └── utils.js
>      └── reports/
>    cypress.config.js  
>    .env  
>    package.json  
>    ```
> 4. Create a working **test case for the OrangeHRM login page**:
>    🔗 URL: [https://opensource-demo.orangehrmlive.com/web/index.php/auth/login](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)
>
>    * Use POM to interact with the login elements.
>    * Validate successful login (check the presence of the dashboard or welcome message).
> 5. Add a **configurable environment setup**:
>
>    * `.env` file to store environment data like:
>
>      ```
>      CYPRESS_BASE_URL=https://opensource-demo.orangehrmlive.com/web/index.php/auth/login
>      CYPRESS_USERNAME=Admin
>      CYPRESS_PASSWORD=admin123
>      ```
>    * Load environment variables using the `dotenv` package inside Cypress config.
> 6. Integrate **Mochawesome Reports** to generate beautiful HTML reports after execution.
>
>    * Automatically merge and generate the final report.
> 7. Implement **Before and After hooks** in the test to handle setup and teardown.
> 8. Add **custom Cypress commands** for reusable actions (e.g., `cy.login()`).
> 9. Configure **ESLint** for clean, maintainable JavaScript code.
> 10. Add **scripts** in `package.json` for easy execution:
>
>     ```json
>     "scripts": {
>       "test": "cypress run",
>       "open": "cypress open",
>       "report": "npx mochawesome-merge cypress/reports/*.json | npx mochawesome-report-generator"
>     }
>     ```
> 11. Include comments in every file explaining functionality for beginners.
> 12. The final output should include step-by-step instructions for:
>
>     * Installing dependencies
>     * Running tests in headed/headless mode
>     * Generating and viewing the Mochawesome HTML report
>
> 🎯 **Expected Output:**
>
> * Full Cypress folder structure
> * All code files (`LoginPage.js`, `HomePage.js`, `loginTest.cy.js`, `commands.js`, `utils.js`)
> * `package.json`
> * `cypress.config.js`
> * `.env` file example
> * Example HTML report output path
> * Clear “how to run” commands for VS Code terminal (`npx cypress open`, `npx cypress run`).
>
> The final output must be **fully runnable in VS Code** without any manual configuration.

---
# 5) Cypress Web Automation Framework** 
  using **TypeScript** for use in **VS Code**.
> Act as an experienced QA Automation Lead and generate a complete, production-ready **Cypress Web Automation Framework** written in **TypeScript** for use in **VS Code**.
>
> ✅ **Hard requirements — include everything in one output so I can copy/paste or auto-generate files**:
>
> 1. Provide a **full project scaffold** and file contents (no placeholders only; every file should contain runnable/type-correct code). Use `npm` / `pnpm` compatible setup.
> 2. Use **Cypress + TypeScript** and include `tsconfig.json` and types so the project compiles without extra edits. Include necessary `@types/*` packages.
> 3. Provide a complete **package.json** (scripts + devDependencies) that installs:
>
>    * `cypress` (latest)
>    * `typescript`
>    * `ts-node`
>    * `@types/node`, `@types/chai` as needed
>    * `mochawesome`, `mochawesome-merge`, `mochawesome-report-generator` (for HTML reports)
>    * `dotenv` (load env vars)
>    * `eslint` + TypeScript parser + recommended config
>    * any helper libs you use (e.g., `dayjs` if needed)
> 4. Use **Page Object Model in TypeScript**. Include at least: `LoginPage.ts` and `DashboardPage.ts` under `cypress/support/pages` or `cypress/pages`. Pages should use Cypress commands and typed element getters.
> 5. Provide a sample **test** in TypeScript (`cypress/e2e/login.cy.ts`) that validates the login flow for:
>    `https://opensource-demo.orangehrmlive.com/web/index.php/auth/login`
>    — Use credentials from `.env` and `cypress.config.ts` environment config. Validate successful login by asserting dashboard visibility.
> 6. Add **custom commands** in TypeScript (`cypress/support/commands.ts`) and type definitions in `cypress/support/index.d.ts` so `cy.login()` is typed and autocompletes in VS Code.
> 7. Configure **cypress.config.ts** (TypeScript) to:
>
>    * Load base url from `.env` (use `dotenv`)
>    * Enable screenshots and videos on failure
>    * Set test retries and viewport defaults
>    * Configure `e2e` to use `specPattern` for `.cy.ts` files
> 8. Add **fixtures** (`cypress/fixtures/credentials.json`) and show usage.
> 9. Integrate **Mochawesome HTML reporting** with scripts to merge and generate the final report. Ensure test run produces JSON reports in `cypress/reports` and a merged HTML in `cypress/reports/html`. Include `package.json` scripts for: `cypress:open`, `cypress:run`, `report:merge`, `report:generate`, `clean:reports`.
> 10. Implement **hooks** (`before`, `afterEach`) in `cypress/support/e2e.ts` to:
>
>     * Automatically capture screenshots on failure and attach (in report metadata).
>     * Save video for failed tests.
> 11. Include **ESLint + Prettier** config to enforce consistent TypeScript style. Provide `.eslintrc.cjs` and `.prettierrc`.
> 12. Provide a **.env.example** showing keys: `CYPRESS_BASE_URL`, `CYPRESS_USERNAME`, `CYPRESS_PASSWORD`. Explain where to place `.env`.
> 13. Add **README.md** with exact step-by-step commands to:
>
>     * Install deps (`npm install`)
>     * Open Cypress (`npm run cypress:open`)
>     * Run headless tests and generate merged HTML report (`npm run cypress:run` then `npm run report:merge && npm run report:generate`)
>     * View the HTML report path.
> 14. Make the framework **CI-friendly**: include recommended GitHub Actions snippet in README to run tests and upload report as artifact.
> 15. Include **inline comments** in each file explaining purpose and important lines for beginners.
> 16. Ensure **type safety** so VS Code autocompletion works (export interfaces for page elements or responses if used).
> 17. Ensure tests **run without manual edits** after user fills `.env` values (i.e., no hardcoded tokens).
> 18. Provide an **example test run output** summary showing successful run and report generation path.
>
> 🎯 **Deliverable format** (single-chat output):
>
> * A tree of the full folder structure.
> * The complete contents of **every file** required by the scaffold (e.g., `package.json`, `tsconfig.json`, `cypress.config.ts`, `.eslintrc.cjs`, `.prettierrc`, `.env.example`, pages, support files, tests, README).
> * Do **not** ask clarifying questions — assume default values listed above and produce the full project.
>
> The generated project should be **copy-paste runnable in VS Code** and produce a working Cypress TypeScript test with Mochawesome HTML report when the user runs `npm install` and sets `.env`.
---

# 6) Playwright Web Automation Framework
   using **JavaScript** for use in **VS Code**.

---
> Act as an experienced QA Automation Lead and generate a complete, production-ready **Playwright Web Automation Framework** written in **JavaScript** for use in **VS Code**.
>
> ✅ **Hard requirements — include everything in one output so I can copy/paste or auto-generate files**:
>
> 1. Provide a **full project scaffold** and file contents (no placeholders only; every file should contain runnable code). Use `npm` compatible setup.
> 2. Use **Playwright Test Runner** (official `@playwright/test`) with JavaScript (not TypeScript). Include `playwright.config.js` configured for browsers: chromium, firefox, webkit.
> 3. Provide a complete **package.json** (scripts + devDependencies) that installs:
>
>    * `@playwright/test` (latest)
>    * `dotenv` (for env vars)
>    * `eslint` + recommended plugins + Prettier for JS lint/formatting
>    * any reporter libs if used (note: Playwright has built-in HTML reporter)
> 4. Use **Page Object Model (POM)** with JavaScript classes. Include at least: `LoginPage.js` and `DashboardPage.js` under `tests/pages` or `src/pages`. Pages should expose clear methods (e.g., `login(username, password)`) and use Playwright locators.
> 5. Provide sample **tests** under `tests/` (e.g., `tests/login.spec.js`) that validate the login flow for:
>    `https://opensource-demo.orangehrmlive.com/web/index.php/auth/login`
>    — Use credentials from `.env` and `playwright.config.js` environment config. Validate successful login by asserting dashboard visibility.
> 6. Add **fixtures** or `test-data` (e.g., `tests/fixtures/credentials.json`) and show usage in tests.
> 7. Create a **.env.example** showing keys: `BASE_URL`, `USERNAME`, `PASSWORD`. Explain where to place `.env`. Use `dotenv` to load in Playwright config or tests.
> 8. Configure `playwright.config.js` to:
>
>    * Read `BASE_URL` from `.env` (via `dotenv`)
>    * Enable HTML reporter and configure output directory (e.g., `playwright-report`)
>    * Enable `trace` (on-first-retry), screenshots and video capture on failure
>    * Set retries, timeout, and test directory
> 9. Implement **hooks** (Playwright fixtures) for common setup/teardown in a `tests/helpers/fixtures.js` or use `test.beforeEach` / `test.afterEach` to take screenshots and collect traces on failure.
> 10. Add **custom test utilities** under `tests/utils` (e.g., `apiHelper.js` if needed, `expectHelpers.js`) and show usage.
> 11. Integrate **ESLint + Prettier** with configs (`.eslintrc.cjs`, `.prettierrc`) and include an `.vscode` recommended settings JSON snippet for formatting on save.
> 12. Add **npm scripts** for easy execution:
>
> ```json
> "scripts": {
>   "test": "npx playwright test",
>   "test:headed": "npx playwright test --headed",
>   "test:report": "npx playwright show-report",
>   "test:grep": "npx playwright test --grep",
>   "install:browser": "npx playwright install"
> }
> ```
>
> 13. Provide a **README.md** with exact step-by-step commands to:
>
> * Install deps (`npm install`)
> * Install playwright browsers (`npm run install:browser`)
> * Run tests headless and headed (`npm test`, `npm run test:headed`)
> * Open the HTML report (`npm run test:report`)
> * Where to find screenshots, videos and traces (`playwright-report` directory)
>
> 14. Make the framework **CI-friendly**: include a recommended **GitHub Actions** workflow YAML in README to run tests, upload the Playwright report as an artifact, and optionally publish the HTML report.
> 15. Add **inline comments** in each file explaining purpose and important lines for beginners.
> 16. Ensure tests **use no hardcoded credentials** — they must read from `.env` or fixtures. Provide a final example showing a successful test run console snapshot and the location of the generated HTML report.
> 17. Provide the full **folder tree** at the top of the output and then the complete contents of every file needed by the scaffold (including `.gitignore`, `.env.example`, `package.json`, `playwright.config.js`, pages, tests, fixtures, utils, ESLint/Prettier, README, and GitHub Actions YAML).
> 18. Do **not** ask clarifying questions — assume the defaults listed above and produce the full project.
>
> 🎯 **Deliverable format** (single-chat output):
>
> * A tree of the full folder structure.
> * The complete contents of **every file** required by the scaffold.
> * No extra commentary; only the folder tree and file contents so I can copy/paste into files.
>
> The generated project should be **copy-paste runnable in VS Code** and produce a working Playwright JavaScript test with HTML report, screenshots, videos and traces when the user runs `npm install`, `npm run install:browser`, and `npm test`.
---

# 7) Playwright Test Framework
  using **TypeScript** for use in **VS Code**.

> Act as an experienced QA Automation Lead and generate a complete, production-ready **Playwright Test Framework** written in **TypeScript** for use in **VS Code**.
>
> ✅ **Hard requirements — include everything in one output so I can copy/paste or auto-generate files**:
>
> 1. Provide a **full project scaffold** and file contents (no placeholders only; every file should contain runnable/type-correct code). Use `npm` compatible setup.
> 2. Use **Playwright Test Runner** (`@playwright/test`) with **TypeScript**. Include `playwright.config.ts` configured to run tests on `chromium`, `firefox` and `webkit`. Ensure Playwright TypeScript support is properly configured.
> 3. Provide a complete **package.json** (scripts + devDependencies) that installs:
>
>    * `@playwright/test` (latest)
>    * `typescript`
>    * `ts-node` or necessary types for running config in TS if needed
>    * `@types/node`
>    * `dotenv` (for env vars)
>    * `eslint`, `prettier`, `@typescript-eslint/parser`, `@typescript-eslint/eslint-plugin` for lint/formatting
>    * any helper libs you use (e.g., `date-fns` if needed)
> 4. Use **Page Object Model (POM)** with TypeScript classes. Include at least: `LoginPage.ts` and `DashboardPage.ts` under `src/pages` (or `tests/pages`). Pages must use Playwright locators and return typed results. Export interfaces/types where appropriate.
> 5. Provide sample **tests** in TypeScript under `tests/` (e.g., `tests/login.spec.ts`) that validate the login flow for:
>    `https://opensource-demo.orangehrmlive.com/web/index.php/auth/login`
>    — Tests must read credentials from `.env` via `dotenv` (wired into `playwright.config.ts` or fixtures) and assert dashboard visibility after login.
> 6. Add **fixtures/test-data** (e.g., `tests/fixtures/credentials.json`) and demonstrate usage.
> 7. Create a **.env.example** showing keys: `BASE_URL`, `USERNAME`, `PASSWORD`. Explain where to put `.env`. Use `dotenv` in `playwright.config.ts` to load envs so tests can reference `process.env`.
> 8. Configure `playwright.config.ts` to:
>
>    * Read `BASE_URL` from `.env`
>    * Enable HTML reporter and set output directory (e.g., `playwright-report`)
>    * Enable screenshots, traces and video capture on failure (trace: on-first-retry)
>    * Set retries, global timeout, and test directory
>    * Configure projects for `chromium`, `firefox`, and `webkit` with simple device emulation if needed
> 9. Implement **fixtures/hooks** using Playwright’s `test.extend` or `test.beforeEach` / `test.afterEach` to:
>
>    * Automatically capture screenshots and videos on failure and save traces on first retry
>    * Provide a logged-in `page` fixture (optional) or helper `login()` that can be reused in tests
> 10. Add **custom utilities** under `tests/utils` (e.g., `helpers.ts` for common actions, `selectors.ts` for shared selectors) and show usage with TypeScript typing.
> 11. Integrate **ESLint + Prettier** with configs (`.eslintrc.cjs`, `.prettierrc`) for TypeScript; include an `.vscode` recommended settings JSON snippet for formatting on save.
> 12. Add **npm scripts** for easy execution:
>
> ```json
> "scripts": {
>   "test": "npx playwright test",
>   "test:headed": "npx playwright test --headed",
>   "test:report": "npx playwright show-report",
>   "install:browser": "npx playwright install"
> }
> ```
>
> 13. Provide a **README.md** with exact step-by-step commands to:
>
> * Install dependencies (`npm install`)
> * Install Playwright browsers (`npm run install:browser`)
> * Run tests headless and headed (`npm test`, `npm run test:headed`)
> * Open the HTML report (`npm run test:report`)
> * Where to find screenshots, videos and traces (`playwright-report` directory)
>
> 14. Make the framework **CI-friendly**: include a recommended **GitHub Actions** workflow YAML in the README to run tests, save the Playwright report and upload screenshots/videos/traces as artifacts.
> 15. Add **TypeScript types** and interfaces for page models and test data to enable VS Code autocompletion (e.g., `type Credentials = { username: string; password: string }`).
> 16. Ensure tests **use no hardcoded credentials** — they must read from `.env` or fixtures. Provide clear instructions to populate `.env`.
> 17. Provide a final example of the **expected console output** for a successful test run and the path of the generated HTML report.
> 18. Provide a full **folder tree** at the top of the output, then the complete contents of **every file** required by the scaffold (including `.gitignore`, `.env.example`, `package.json`, `tsconfig.json`, `playwright.config.ts`, pages, tests, fixtures, utils, ESLint/Prettier configs, README, and GitHub Actions YAML).
> 19. Do **not** ask clarifying questions — assume the defaults listed above and produce the full project.
>
> 🎯 **Deliverable format** (single-chat output):
>
> * A tree of the full folder structure.
> * The complete contents of **every file** required by the scaffold.
> * Minimal extra commentary — only the necessary inline comments inside files.
>
> The generated project should be **copy-paste runnable in VS Code** and produce a working Playwright TypeScript test with HTML report, screenshots, videos and traces when the user runs `npm install`, `npm run install:browser`, and `npm test`.

---

# 8) Appium Android Mobile Automation Framework
using **Java**, **Maven**, **TestNG**, and **Extent Reports**, intended to be imported and run in **Eclipse**.


> Act as an experienced Mobile QA Automation Lead and generate a complete, production-ready **Appium Android Mobile Automation Framework** using **Java**, **Maven**, **TestNG**, and **Extent Reports**, intended to be imported and run in **Eclipse**.
>
> ✅ **Hard requirements — include everything in one output so I can copy/paste or auto-generate files**:
>
> 1. Produce a full **Maven** project scaffold and file contents (no placeholders only; every file should contain runnable/type-correct Java code). Provide the full folder tree at the top. Target Java 11 compatibility.
> 2. Use **Appium Java Client** + **Selenium** + **TestNG** + **ExtentReports** for HTML reporting. Include proper dependency versions in a single `pom.xml`. Configure `maven-compiler-plugin` for Java 11 and `maven-surefire-plugin` to run TestNG `testng.xml`.
> 3. Implement **Page Object Model (POM)** for the mobile app. Include at minimum: `LoginPage.java` and `HomePage.java` under `src/test/java/<your_package>/pages`. Pages should use Appium `AndroidDriver` and typed mobile element locators.
> 4. Provide core framework classes under `src/test/java/<your_package>/core` or `base`:
>
>    * `BaseTest.java` → Sets up Appium `AndroidDriver` with capabilities, handles driver lifecycle, provides common logging and utilities (startTest, logInfo, logPass, logFail, attachScreenshot). Should read configuration from `config.properties`.
>    * `DriverFactory.java` → Creates driver instances for local emulator, real device (USB), and remote (Appium server) using parameters from `config.properties`. Provide examples for `udid`, `deviceName`, `platformVersion`, `appPackage`, `appActivity`, `automationName` (UiAutomator2), and `systemPort` for parallel runs.
>    * `ConfigReader.java` → Reads `src/test/resources/config.properties`.
>    * `ScreenshotUtil.java` → Captures screenshots and returns file path for attaching to Extent.
>    * `ExtentManager.java` → Initializes ExtentReports (timestamped HTML output in `reports/`).
>    * `TestListener.java` → TestNG listener implementing `ITestListener` to manage Extent lifecycle, attach screenshots on failure, and mark pass/fail/skip.
> 5. Provide a sample **Test Class** `LoginTest.java` in `src/test/java/<your_package>/tests` that:
>
>    * Uses TestNG annotations (`@BeforeClass`, `@Test`, `@AfterClass`).
>    * Reads config for app path / appPackage & appActivity or uses installed app caps.
>    * Demonstrates a real login scenario (enter username/password, tap login, assert home screen element). If app strings are unknown, use a sample open-source Android demo app (e.g., `ApiDemos-debug.apk` or `ContactManager.apk`) and write the test accordingly — but include instructions to replace with the user's APK or appPackage/appActivity.
> 6. Include a **testng.xml** to run the tests and show parallel execution example (e.g., parallel="tests" thread-count="2") with sample test suite entries for emulator and real device.
> 7. Provide `config.properties` under `src/test/resources` with keys and example values for:
>
>    * `appium.server.url=http://127.0.0.1:4723/wd/hub`
>    * `platformName=Android`
>    * `deviceName=Android_Emulator`
>    * `platformVersion=11.0`
>    * `udid=` (empty by default)
>    * `automationName=UiAutomator2`
>    * `app.path=apps/ApiDemos-debug.apk` (include note)
>    * `appPackage=` (optional)
>    * `appActivity=` (optional)
>    * `systemPort=8200`
>    * `report.path=reports`
>    * `tester=QA_Team`
> 8. Provide an `apps/` folder reference (not the binary itself) and instructions to place the APK there or update `config.properties` to use installed app via `appPackage`/`appActivity`.
> 9. Integrate **Extent Reports**: HTML output saved in `reports/Appium_Report_<timestamp>.html` and include screenshots on failure attached to report. Ensure no NullPointerExceptions when logging — properly initialize Extent and ExtentTest for each test.
> 10. Add **screenshot capture** on failure via TestNG listener and show how to attach images to report. Also include optional code for page-level screenshot (e.g., `captureElementScreenshot`).
> 11. Include **parallel execution** tips and sample capability `systemPort` handling for running multiple emulator/device tests concurrently. Provide sample `DriverFactory` logic to increment ports.
> 12. Add helpful utility classes for wait & swipe actions: `MobileActions.java` with methods like `waitForElement`, `tap`, `swipeUp`, `swipeDown`, `hideKeyboard`. Use explicit waits (WebDriverWait) with sensible timeouts.
> 13. Provide `pom.xml` scripts and README instructions on how to run tests from Eclipse:
>
> * Import Maven project into Eclipse.
> * Start Appium server (`appium` CLI or Appium Desktop) and start Android emulator or connect device.
> * Run `mvn clean test` or run `testng.xml` from Eclipse.
>
> 14. Provide **README.md** with exact step-by-step setup for beginners covering:
>
> * JDK 11 install & Eclipse setup (Maven support).
> * Appium installation and starting server.
> * Android SDK / AVD setup and connecting real device (adb).
> * Placing APK into `apps/` folder or using `appPackage`/`appActivity`.
> * Running tests and locating the Extent HTML report and screenshots.
>
> 15. Provide a **GitHub Actions** workflow YAML example in README to run tests on an Android emulator via `reactivecircus/android-emulator-runner` or similar, capture artifacts (reports/screenshots) and upload them. Make the CI config optional but fully detailed.
> 16. Add `.gitignore` with standard Maven, Eclipse, and report exclusions.
> 17. Include **inline comments** throughout Java files explaining key lines for beginners. Add Javadoc-style comments for public methods.
> 18. Provide an **example console output** snippet for a successful `mvn clean test` run and the path to the final HTML report.
> 19. At the end, include a short checklist for troubleshooting common issues (Appium server not reachable, APK not installed, adb device not found, port conflicts).
> 20. Do not ask clarifying questions — assume default values above and produce the full project. If any app-specific locator is unknown, use the open-source `ApiDemos-debug.apk` element ids and include a clear comment telling users to replace locators for their app.
>
> 🎯 **Deliverable format (single-chat output)**:
>
> * A tree of the full project folder structure.
> * The complete contents of **every file** required by the scaffold (including `pom.xml`, `testng.xml`, all Java classes, `config.properties`, `README.md`, `.gitignore`, and GitHub Actions YAML).
> * Minimal extra commentary — only necessary inline comments inside files.
>
> The generated framework should be **copy-paste runnable in Eclipse** (after the user places APK or sets appPackage/appActivity), start Appium and emulator/device, run `mvn clean test`, and produce an Extent HTML report with screenshots.
---

# 9) Playwright MCP + Agent (GitHub Copilot Agent) workflow
for **VS Code** that covers **manual test documentation** and **web + API automation**.

> Act as an experienced QA Automation Lead and generate a complete, end-to-end **Playwright MCP + Agent (GitHub Copilot Agent) workflow** for **VS Code** that covers **manual test documentation** and **web + API automation**.
>
> **Hard requirements — produce everything in one shot (copy/paste runnable and ready-to-follow):**
>
> 1. Explain what **Playwright MCP (Model Context Protocol)** and **GitHub Copilot Agent mode** are and how they work together at a high level (short, 3–5 bullet summary). Cite the official Playwright MCP repo and GitHub Copilot agent docs (include links).
> 2. Provide **step-by-step setup instructions** for a developer workstation (Windows/macOS/Linux) to run:
>
>    * VS Code extensions to install (Playwright, GitHub Copilot, GitLens, REST Client, etc.).
>    * Clone and run the official **Playwright MCP server** (exact `git clone` and `npm` commands), install deps, and start the server with example config. Show sample `mcp.config.json` (host, port, token) and secure token guidance.
>    * Enable **GitHub Copilot agent mode** in VS Code and connect it to the local Playwright MCP server (show exact UI steps and minimal settings).
>    * Start a Playwright browser session that MCP/Copilot can use (native Playwright install + `npx playwright test --project=chromium` example).
> 3. Create a fully working **Playwright (TypeScript)** project scaffold that integrates with MCP:
>
>    * Provide the full folder tree and every file content (package.json, tsconfig.json, playwright.config.ts, src/pages, tests, support, fixtures, utils, .env.example, README).
>    * Tests must include **web UI** (login scenario for `https://opensource-demo.orangehrmlive.com/web/index.php/auth/login`) and **API tests** (example using Playwright `request` API to call a sample API). Use `.env` for base URLs/credentials.
>    * Include **Page Object Model (POM)** pages (LoginPage, DashboardPage) in TypeScript with types and exported interfaces.
>    * Include a sample Playwright test that is generated manually (baseline) and also show a variant **generated by MCP/Copilot** (copy the generated test file).
> 4. Provide an **MCP-driven agent workflow** (the exact commands/prompts the Copilot agent will use) to:
>
>    * Explore the app (open URL, take accessibility snapshots), identify the login flow.
>    * Create Playwright test code (TypeScript) + POM from a natural-language test case.
>    * Improve generated tests iteratively (fix selectors, add retries, add wait/timeout adjustments) using Copilot agent “Fix with AI” style actions.
>    * Export a human-readable **manual test case document** (Markdown) for the same scenario.
> 5. Provide **exact agent prompts** to paste into Copilot Agent (or the Playwright Trace Viewer “Copy as Prompt”) — ready-to-copy natural-language instructions for the agent to:
>
>    * Generate a Page Object for the login page (include type annotations).
>    * Generate an end-to-end Playwright test for login with assertions and retries.
>    * Generate API test(s) for the login/auth endpoints using Playwright Request API.
>    * Convert the automated test into a step-by-step manual test case document (preconditions, steps, expected result, test data table).
>    * Create negative tests and edge-case test cases and add them to the test suite.
> 6. Provide **step-by-step documentation prompts** (these are prompts the QA or product writer will paste into ChatGPT/Copilot to create docs). For each prompt include a one-line description of the expected output. Deliver at least these prompts:
>
>    * “Generate a one-page **Manual Test Case** for Login — preconditions, test steps, expected results, test data table, severity, priority.” (expected output: markdown manual test).
>    * “Create an **Exploratory Test Charter** for the Login area — risks, areas to explore, heuristics.” (expected output: short charter).
>    * “Convert the following Playwright test file (paste code) into a step-by-step manual test with screenshots placeholders.” (expected output: a manual test with screenshot placeholders).
>    * “Create an **API Test Matrix** for authentication endpoints: endpoints, methods, sample request/response, success and failure test cases.” (expected output: table).
>    * “Write a **Test Plan** section for automating web + API login flows using Playwright MCP and Copilot Agent — include scope, risk, resources, CI steps.” (expected output: markdown test plan).
>    * “Create a **How-to** guide for triaging flaky tests generated by MCP: steps to reproduce, capture trace, fix selectors, re-run.” (expected: a troubleshooting checklist).
> 7. Provide **example Copilot Agent prompts** (low-level) the agent should receive to produce code snippets. Make them explicit and practical (e.g., “Open URL X, click element with accessible-name ‘Username’, fill with VALUE, click ‘Submit’, verify element H6 text ‘Dashboard’”). Provide at least 8 such prompts (for happy path, negative tests, API calls, data-driven iteration, screenshot capture).
> 8. Provide an example **CI pipeline** (GitHub Actions) workflow that:
>
>    * Starts the Playwright MCP server (or uses a hosted MCP if necessary), installs dependencies, runs Playwright tests headless, collects Playwright HTML report, uploads artifacts, and (optionally) invokes Copilot Agent in an automated step to generate/update tests from new requirements. Include the full YAML file.
> 9. Provide **best practices & security** checklist: how to secure MCP server tokens, avoid leaking credentials to Copilot, safe network settings, local-only MCP guidance, and limits for agent access.
> 10. Provide an **appendix** that includes:
>
>     * Example `mcp.config.json` for Playwright MCP server.
>     * Example `.env.example` with variables: `BASE_URL`, `USERNAME`, `PASSWORD`, `MCP_HOST`, `MCP_PORT`, `MCP_TOKEN`.
>     * Example terminal commands in order to get from fresh machine → running agent-driven test generation → producing HTML report.
> 11. The output must include **many ready-to-copy prompts** grouped under two headings: **A. “Generate automation (code) prompts”** and **B. “Generate documentation (manual test) prompts”**. Each prompt must have a one-line “what it produces” description. Provide at least 12 prompts total (6 automation, 6 documentation).
> 12. All generated code snippets and configs must be **TypeScript Playwright** (for tests and POM), and be copy-paste runnable after `npm install` and `npx playwright install` (assuming user fills `.env`). Where exact MCP or Copilot features require tokens or experimental flags, show how to set them and provide safe defaults.
> 13. End the generated output with a **“Quick Start — 10 commands”** list that takes a developer from an empty clone to: start MCP, connect Copilot, generate an automated login test, run tests, and open the Playwright report.
>
> **Deliverables (what ChatGPT should return):**
>
> * Full, single-shot output that includes: short conceptual summary, step-by-step setup, full Playwright TypeScript project scaffold (folder tree + critical file examples — you don’t need to print every file, but must print all files relevant to MCP integration and sample tests), precise MCP and Copilot connection steps, sample agent prompts, the “documentation prompts” list, CI YAML, security checklist, appendix, and the 10-command quick start.
> * Mark clearly which portions are **“COPY-PASTE PROMPTS”** (these are the exact strings the user should paste into Copilot Agent or ChatGPT) and which are configuration or code.
> * Ensure everything is actionable and minimizes the need for manual editing.
>
> **Tone & style:** produce clear, concise, stepwise instructions and copy-ready prompts — prefer bullet lists and code blocks where appropriate. Avoid asking clarifying questions; assume defaults listed above.

---
