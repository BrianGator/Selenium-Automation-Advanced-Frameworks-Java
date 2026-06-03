# Selenium Automation Advanced Frameworks with Java

**Written by Brian McCarthy**

This repository is a comprehensive Selenium WebDriver automation showcase focused on **Java, Selenium WebDriver 4, TestNG, Maven, Page Object Model, data-driven testing, framework design, Jenkins CI/CD, Selenium Grid, Chrome DevTools Protocol, Cucumber BDD, Excel utilities, JDBC database validation, cloud execution, API testing, login testing, and technical interview preparation**.

The README is organized around the requested 36-chapter Selenium WebDriver course structure, with additional non-duplicate supplemental modules based on the detailed Packt course table of contents. The base modules cover the core course path; the supplemental modules add advanced topics such as Java Streams, Selenium 4 relative locators, CDP network interception, Extent Reports, ThreadLocal, retries, Cucumber, Selenium Grid, BrowserStack/Sauce Labs, JDBC, AutoIT, Excel utilities, API testing, login testing, and framework architecture.

---

## Course Table of Contents

| Module # | Module Name | Module Details |
|---:|---|---|
| 1 | [Introduction](#module-1---introduction) | Selenium purpose, automation value, WebDriver architecture, browser automation flow, framework objectives, and course learning strategy. |
| 2 | [Setup and Configuration](#module-2---setup-and-configuration) | Java, Eclipse/IntelliJ, Maven project setup, browser drivers, Selenium Manager, WebDriverManager, Chrome/Firefox/Edge setup, and troubleshooting. |
| 3 | [Understanding Variables and Data Types](#module-3---understanding-variables-and-data-types) | Java variables, primitive types, strings, booleans, numeric values, test data values, expected results, and automation constants. |
| 4 | [Advanced Data Types](#module-4---advanced-data-types) | Arrays, ArrayList, HashMap, Set, collections, multi-value test data, product lists, login users, and locator containers. |
| 5 | [Comparison and Boolean Operators](#module-5---comparison-and-boolean-operators) | Equality, relational operators, boolean logic, compound checks, assertion conditions, enabled/disabled validation, and test decision logic. |
| 6 | [Program Control Flow](#module-6---program-control-flow) | `if/else`, `switch`, `for`, enhanced `for`, `while`, `do while`, break/continue, loops through products, pagination, and tables. |
| 7 | [Functions/Methods - Reusable Code](#module-7---functionsmethods---working-with-reusable-code) | Reusable methods, parameters, return values, utility actions, custom waits, generic calendar handlers, parsing methods, and helper functions. |
| 8 | [Classes and Object-Oriented Programming](#module-8---classes-and-object-oriented-programming) | Classes, objects, constructors, `this`, `super`, inheritance, interfaces, abstract classes, overloading, overriding, access modifiers, static/final, and framework OOP. |
| 9 | [Exception Handling](#module-9---exception-handling) | Selenium exceptions, Java `try/catch/finally`, stale elements, no such element, timeouts, click interception, failed test handling, and custom failure evidence. |
| 10 | [Modules and Packages](#module-10---modules-and-packages) | Java packages, Maven project modules, `base`, `pages`, `tests`, `utils`, `listeners`, `resources`, imports, and framework organization. |
| 11 | [Working with Files](#module-11---working-with-files) | Properties files, JSON files, Excel files, screenshots, logs, downloads, upload files, test data files, and file validation. |
| 12 | [Inspecting Elements on Different Browsers](#module-12---how-to-inspect-elements-on-different-browsers) | Chrome/Edge/Firefox DevTools, SelectorsHub, DOM inspection, attributes, parent-child relationships, siblings, accessibility attributes, and locator validation. |
| 13 | [Selenium WebDriver Setup and Installation](#module-13---selenium-webdriver-setup-and-installation) | Selenium Java dependency, WebDriver setup, Selenium Manager, ChromeDriver, GeckoDriver, EdgeDriver, first WebDriver script, and driver lifecycle. |
| 14 | [Running Tests on Various Browsers](#module-14---selenium-webdriver-running-tests-on-various-browsers) | Chrome, Firefox, Edge, cross-browser strategy, driver factory, browser parameters, headless execution, and browser-specific options. |
| 15 | [Finding Elements](#module-15---selenium-webdriver---finding-elements) | ID, name, class name, tag name, link text, partial link text, CSS selector, XPath, `findElement`, `findElements`, and scoped searches. |
| 16 | [CSS Selectors - Advanced Locators](#module-16---cascading-style-sheets-css-selectors---advanced-locators) | CSS by ID/class/attribute, contains/starts-with/ends-with patterns, parent-child hierarchy, nth-child, regular-expression-style matching, and locator quality. |
| 17 | [XPath - Advanced Locators](#module-17---xpath---advanced-locators) | Relative XPath, text, contains, starts-with, parent-child traversal, child-to-parent traversal, siblings, dynamic XPath, and XPath interview examples. |
| 18 | [Working with WebElements](#module-18---selenium-webdriver---working-with-webelements) | Input fields, buttons, dropdowns, dynamic dropdowns, checkboxes, auto-suggestive dropdowns, calendars, Java alerts, disabled/enabled elements, and end-to-end UI flows. |
| 19 | [Useful Methods and Properties](#module-19---selenium-webdriver---useful-methods-and-properties) | URL, title, page source, window size, cookies, maximize, delete cookies, attributes, text, enabled/displayed/selected, screenshots, and broken link status codes. |
| 20 | [Wait Types](#module-20---selenium-webdriver---wait-types) | Implicit wait, explicit wait, FluentWait, custom wait methods, polling, ignored exceptions, Ajax synchronization, and why static sleeps should be avoided. |
| 21 | [Advanced Interactions](#module-21---selenium-webdriver--advanced-interactions) | Actions class, mouse hover, drag-and-drop, scrolling, JavaScriptExecutor, web tables, generated totals, Ajax calls, calendar widgets, and advanced UI problems. |
| 22 | [File Upload and Download](#module-22---selenium-webdriver---file-upload-and-download) | Upload with `sendKeys`, download path configuration, downloaded file validation, synchronized toast messages, Excel upload/download, and system-dialog limitations. |
| 23 | [Switch Windows and Iframes](#module-23---selenium-webdriver---switch-window-and-iframes) | Alerts, child windows, tabs, window handles, iframe switching, default content, nested frames, focus management, and multi-window validation. |
| 24 | [Actions Class](#module-24---selenium-webdriver---working-with-actions-class) | Mouse interactions, keyboard interactions, hover menus, right-click, double-click, drag-and-drop, sliders, composite actions, and real-time examples. |
| 25 | [Logging Infrastructure](#module-25---logging-infrastructure) | Log4j2 setup, framework logs, console/file appenders, logging standards, debug strategy, and CI-friendly execution logs. |
| 26 | [TestNG Infrastructure](#module-26---testng-infrastructure) | TestNG annotations, suite XML, groups, priorities, dependencies, parameters, DataProvider, listeners, parallel execution, and reports. |
| 27 | [JUnit/Pytest Equivalents for Java](#module-27---junitpytest-equivalents-for-java) | Java alternatives to Python testing frameworks, JUnit 5, TestNG comparisons, parameterized tests, tags, runners, and lifecycle hooks. |
| 28 | [Automation Framework - Part 1](#module-28---automation-framework---part-1) | Maven framework creation, dependencies, ecommerce app demo, WebDriverManager, login flow, product list, explicit waits, add-to-cart, and checkout validation. |
| 29 | [Automation Framework - Part 2](#module-29---automation-framework---part-2) | Page Object Model, PageFactory, page actions, abstract components, product catalogue page, reusable methods, and complete refactor into POM. |
| 30 | [Automation Framework - Part 3](#module-30---automation-framework---part-3) | BaseTest, global properties, driver initialization, error validation tests, dependency strategy, groups, TestNG XML, and parallel class execution. |
| 31 | [Automation Framework Practice Exercise](#module-31---automation-framework-practice-exercise) | End-to-end practice exercise, ecommerce flow, calendar handling, reusable methods, page objects, dynamic locators, and framework refactoring. |
| 32 | [Data-Driven Testing](#module-32---data-driven-testing) | TestNG DataProvider, multidimensional arrays, HashMap test data, JSON file data, Excel integration, Apache POI, and parameterized tests. |
| 33 | [Running the Complete Test Suite](#module-33---running-complete-test-suite) | Maven commands, terminal execution, smoke/regression suites, TestNG XML, Maven parameters, headless mode, and suite-level reporting. |
| 34 | [Git and GitHub Version Control](#module-34---git-and-github---version-control-system) | Git config, repositories, staging, commits, remotes, push, branching, merge conflicts, GitHub framework storage, and Jenkins/GitHub integration. |
| 35 | [Continuous Integration with Jenkins](#module-35---continuous-integration-with-jenkins) | Jenkins installation, plugins, Maven jobs, GitHub webhooks, parameterized jobs, scheduled jobs, nightly automation, artifacts, and CI/CD flow. |
| 36 | [Conclusion](#module-36---conclusion) | Framework maturity, next steps, cloud execution, CDP, Grid, API testing, BDD, reporting, and interview preparation roadmap. |
| 37 | [Supplemental: Java Streams for Web Tables](#supplemental-module-37---selenium-java-streams-for-web-tables) | Java Streams, sorting, pagination, filtering web tables, mapping elements to text, and stream-based validation. |
| 38 | [Supplemental: Selenium 4 Features](#supplemental-module-38---selenium-40-latest-features) | Relative locators, multiple tabs/windows, WebElement screenshots, element size checks, and UX validation. |
| 39 | [Supplemental: Framework Part 4 - Test Strategy and Parallel Control](#supplemental-module-39---framework-part-4-test-strategy-and-parallel-control) | DataProvider parameterization, HashMap data, JSON data, screenshot utility, groups, parallel tests, and execution control. |
| 40 | [Supplemental: Framework Part 5 - Extent Reports, Listeners, ThreadLocal, Retry](#supplemental-module-40---framework-part-5-extent-reports-listeners-threadlocal-and-retry) | ExtentReports, TestNG listeners, screenshots in reports, ThreadLocal driver isolation, and IRetryAnalyzer. |
| 41 | [Supplemental: Framework Part 6 - Maven and Jenkins CI/CD](#supplemental-module-41---framework-part-6-maven-and-jenkins-cicd) | Maven terminal execution, global Maven parameters, Jenkins parameters, headless execution, scheduled/nightly jobs. |
| 42 | [Supplemental: Framework Part 7 - Cucumber BDD Wrapper](#supplemental-module-42---framework-part-7-cucumber-bdd-wrapper) | Cucumber terminology, dependencies, feature files, step definitions, regex, TestNG runner, tags, and background. |
| 43 | [Supplemental: Selenium Grid and Cloud Testing](#supplemental-module-43---cross-browser-testing-with-selenium-grid-and-cloud) | Selenium Grid hub/node, RemoteWebDriver, desired capabilities, cloud vendors, BrowserStack/Sauce Labs, and parallel browser coverage. |
| 44 | [Supplemental: Selenium 4 Chrome DevTools Protocol](#supplemental-module-44---selenium-4-chrome-devtools-protocol-cdp) | Device emulation, localization, network responses, status codes, request blocking, network speed, basic auth, and JavaScript errors. |
| 45 | [Supplemental: Database Testing with JDBC](#supplemental-module-45---database-connection-to-selenium-testcases) | MySQL setup, JDBC connection, SQL queries, table validation, UI-to-database validation, and backend data checks. |
| 46 | [Supplemental: AutoIT and Native Dialogs](#supplemental-module-46---file-uploading-autoit-and-downloading-with-selenium) | Window authentication popups, AutoIT installation, desktop object inspection, upload dialogs, downloads, and Chrome download preferences. |
| 47 | [API Tests for Selenium Java Frameworks](#api-tests-for-selenium-java-frameworks) | Rest Assured setup, GET/POST/PUT/DELETE, authentication, status/body validation, API setup/cleanup, and hybrid UI/API testing. |
| 48 | [Login Tests for Selenium Java Frameworks](#login-tests-for-selenium-java-frameworks) | Valid login, invalid login, empty fields, locked users, logout, session expiration, role-based login, secure credentials, and login POM. |
| 49 | [Locator Reference Guide](#locator-reference-guide) | ID, name, CSS, XPath, link text, class name, tag name, relative locators, dynamic locator guidance, and locator anti-patterns. |
| 50 | [Building a Selenium Java Framework from Scratch](#building-a-selenium-java-framework-from-scratch) | Required files/folders, dependencies, BaseTest, DriverFactory, Page Objects, utilities, listeners, reports, API helpers, and CI/CD readiness. |
| 51 | [Build from Scratch vs Pre-Built Frameworks](#build-from-scratch-vs-pre-built-frameworks) | When custom frameworks are needed, when pre-built tools are better, popular framework stacks, and scenario-based guidance. |
| 52 | [Top 30 Selenium Java Technical Interview Questions](#top-30-selenium-java-technical-interview-questions) | Interview Q&A with Java code examples covering Selenium, waits, locators, TestNG, Maven, API, CI/CD, Grid, CDP, and frameworks. |

---

## Project Overview

This repository is organized as an advanced Selenium WebDriver with Java learning and framework-building project. It begins with core Selenium and Java concepts, then advances into locators, waits, WebElements, Actions, windows, iframes, file handling, logging, TestNG, Maven, Page Object Model, Extent Reports, ThreadLocal parallel execution, retries, Cucumber BDD, Selenium Grid, cloud execution, Chrome DevTools Protocol, JDBC database validation, API testing, and CI/CD.

The detailed Packt-style course outline includes 39 expandable table-of-contents sections ranging from Selenium introduction through Cucumber BDD and defect tracking. This README consolidates that content into a non-duplicated 36-module base course plus supplemental modules for unique advanced topics such as Java Streams, Selenium 4 features, Grid, CDP, JDBC, AutoIT, Extent Reports, and Cucumber. fileciteturn45file0

---

## Module 1 - Introduction

<details>
<summary>Get more details for Module 1</summary>

### What This Module Covers

- Selenium features and why Selenium is used for browser automation.
- WebDriver architecture: test code, WebDriver API, browser driver, browser.
- Difference between Selenium IDE, Selenium WebDriver, and Selenium Grid.
- Where Selenium fits in regression, smoke testing, functional testing, and CI/CD.
- How an advanced framework grows from simple scripts into reusable architecture.

### Java Example

```java
WebDriver driver = new ChromeDriver();
driver.get("https://example.com");
System.out.println("Title: " + driver.getTitle());
driver.quit();
```

### Expected Result

Chrome opens, navigates to the site, prints the page title, and closes cleanly.

</details>

---

## Module 2 - Setup and Configuration

<details>
<summary>Get more details for Module 2</summary>

### What This Module Covers

- Install Java and configure `JAVA_HOME`.
- Install Eclipse or IntelliJ IDEA.
- Create Maven project from scratch.
- Add Selenium, TestNG, WebDriverManager, Log4j, Rest Assured, and reporting dependencies.
- Understand browser driver classes and the WebDriver interface.
- Use Selenium Manager or WebDriverManager to avoid manual driver downloads.
- Troubleshoot Chrome, Firefox, and Edge launch failures.

### Maven Dependencies

```xml
<dependencies>
    <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>4.21.0</version>
    </dependency>
    <dependency>
        <groupId>org.testng</groupId>
        <artifactId>testng</artifactId>
        <version>7.10.2</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>io.github.bonigarcia</groupId>
        <artifactId>webdrivermanager</artifactId>
        <version>5.8.0</version>
    </dependency>
</dependencies>
```

### Expected Result

`mvn test` downloads dependencies, compiles tests, and runs the Selenium test suite.

</details>

---

## Module 3 - Understanding Variables and Data Types

<details>
<summary>Get more details for Module 3</summary>

### What This Module Covers

- Java primitives: `int`, `double`, `boolean`, `char`.
- Reference types: `String`, objects, collections.
- Variables for URLs, credentials, expected messages, timeouts, browser names, and environment values.
- String methods used in automation parsing.

### Java Example

```java
String baseUrl = "https://example.com";
String expectedTitle = "Example Domain";
int timeoutSeconds = 10;
boolean headless = false;

driver.get(baseUrl);
Assert.assertEquals(driver.getTitle(), expectedTitle);
Assert.assertTrue(timeoutSeconds > 0);
Assert.assertFalse(headless);
```

### Expected Result

The test navigates to the URL, verifies the title, and validates basic runtime values.

</details>

---

## Module 4 - Advanced Data Types

<details>
<summary>Get more details for Module 4</summary>

### What This Module Covers

- Arrays and ArrayLists.
- HashMap and Set.
- Differences between arrays and ArrayList.
- Iterating over arrays and collections.
- Using collections to store products, login users, expected values, locators, and test data.

### Java Example

```java
List<String> expectedProducts = Arrays.asList("ZARA COAT 3", "ADIDAS ORIGINAL", "IPHONE 13 PRO");
List<WebElement> products = driver.findElements(By.cssSelector(".mb-3"));

for (WebElement product : products) {
    String productName = product.findElement(By.cssSelector("b")).getText();
    if (expectedProducts.contains(productName)) {
        product.findElement(By.cssSelector("button:last-of-type")).click();
    }
}
```

### Expected Result

Only products listed in `expectedProducts` are added to the cart.

</details>

---

## Module 5 - Comparison and Boolean Operators

<details>
<summary>Get more details for Module 5</summary>

### What This Module Covers

- `==`, `.equals()`, `!=`, `<`, `>`, `<=`, `>=`.
- Boolean AND `&&`, OR `||`, and NOT `!`.
- Assertion conditions for visible/enabled/selected states.
- Attribute-based enabled/disabled validation.

### Java Example

```java
WebElement promoCode = driver.findElement(By.id("promoCode"));
String disabled = promoCode.getAttribute("disabled");

Assert.assertTrue(disabled != null || !promoCode.isEnabled());
Assert.assertFalse(promoCode.isSelected());
```

### Expected Result

The test confirms the promo code field is disabled and not selected.

</details>

---

## Module 6 - Program Control Flow

<details>
<summary>Get more details for Module 6</summary>

### What This Module Covers

- `if/else` and nested conditions.
- `for`, enhanced `for`, `while`, and `do while` loops.
- Looping through arrays, ArrayLists, product cards, links, and web table rows.
- Pagination logic and condition-controlled iteration.

### Java Example

```java
boolean productFound = false;
while (!productFound) {
    List<WebElement> rows = driver.findElements(By.cssSelector("table tbody tr"));
    for (WebElement row : rows) {
        if (row.getText().contains("Rice")) {
            productFound = true;
            break;
        }
    }
    if (!productFound) {
        driver.findElement(By.cssSelector("[aria-label='Next']")).click();
    }
}
Assert.assertTrue(productFound);
```

### Expected Result

The test searches through paginated rows until `Rice` is found.

</details>

---

## Module 7 - Functions/Methods - Working with Reusable Code

<details>
<summary>Get more details for Module 7</summary>

### What This Module Covers

- Method declaration and method calls.
- Parameters and return values.
- Reusable wait methods.
- Reusable product search, calendar handling, and parsing helpers.
- Static vs instance helper methods.

### Java Example

```java
public WebElement waitForElement(By locator) {
    WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
    return wait.until(ExpectedConditions.visibilityOfElementLocated(locator));
}

public void type(By locator, String value) {
    WebElement element = waitForElement(locator);
    element.clear();
    element.sendKeys(value);
}
```

### Expected Result

Page classes and tests can reuse a consistent wait/type pattern instead of repeating code.

</details>

---

## Module 8 - Classes and Object-Oriented Programming

<details>
<summary>Get more details for Module 8</summary>

### What This Module Covers

- Classes, objects, constructors, `this`, and `super`.
- Interfaces and abstract classes.
- Inheritance in framework classes.
- Method overloading and overriding.
- Access modifiers, packages, static, final.
- OOP foundations for Page Object Model.

### Java Example

```java
public abstract class AbstractComponent {
    protected WebDriver driver;
    protected WebDriverWait wait;

    public AbstractComponent(WebDriver driver) {
        this.driver = driver;
        this.wait = new WebDriverWait(driver, Duration.ofSeconds(10));
    }

    public void waitForElement(By locator) {
        wait.until(ExpectedConditions.visibilityOfElementLocated(locator));
    }
}

public class ProductCataloguePage extends AbstractComponent {
    public ProductCataloguePage(WebDriver driver) {
        super(driver);
    }
}
```

### Expected Result

Common waits and shared methods live in the abstract parent class and are inherited by page classes.

</details>

---

## Module 9 - Exception Handling

<details>
<summary>Get more details for Module 9</summary>

### What This Module Covers

- Java `try/catch/finally`.
- Different kinds of exceptions.
- Selenium exceptions: `NoSuchElementException`, `TimeoutException`, `StaleElementReferenceException`, `ElementClickInterceptedException`.
- Taking screenshots and logs on failure.
- Safe retry patterns.

### Java Example

```java
try {
    driver.findElement(By.id("checkout")).click();
} catch (ElementClickInterceptedException e) {
    ((JavascriptExecutor) driver).executeScript("arguments[0].click();", driver.findElement(By.id("checkout")));
} catch (NoSuchElementException e) {
    throw new AssertionError("Checkout button was not found", e);
} finally {
    System.out.println("Checkout click attempt completed");
}
```

### Expected Result

The framework handles click interception safely and gives a meaningful failure if the button is missing.

</details>

---

## Module 10 - Modules and Packages

<details>
<summary>Get more details for Module 10</summary>

### What This Module Covers

- Java packages and imports.
- Maven source structure.
- Framework package design.
- Separation of pages, tests, utilities, base classes, listeners, and resources.

### Recommended Package Structure

```text
src/test/java/
├── base/
├── factory/
├── pages/
├── tests/
├── utils/
├── listeners/
├── api/
└── data/
```

### Expected Result

The framework remains organized, searchable, and scalable as test coverage grows.

</details>

---

## Module 11 - Working with Files

<details>
<summary>Get more details for Module 11</summary>

### What This Module Covers

- Properties files.
- JSON files for HashMap test data.
- Excel data with Apache POI.
- Screenshots and download file validation.
- Reading and writing test evidence.

### Properties Example

```java
Properties properties = new Properties();
try (FileInputStream input = new FileInputStream("src/test/resources/config.properties")) {
    properties.load(input);
}
String browser = properties.getProperty("browser");
String baseUrl = properties.getProperty("baseUrl");
```

### Expected Result

Browser and URL values are loaded from configuration files rather than hardcoded in tests.

</details>

---

## Module 12 - How To Inspect Elements On Different Browsers

<details>
<summary>Get more details for Module 12</summary>

### What This Module Covers

- Chrome, Firefox, and Edge DevTools.
- SelectorsHub plugin usage.
- DOM structure and attributes.
- Validating CSS selectors and XPath.
- Parent-child and sibling locator inspection.
- Locating dynamic elements safely.

### Example Locator Discovery

```java
By email = By.id("userEmail");
By submit = By.cssSelector("button[type='submit']");
By dynamicButton = By.xpath("//button[contains(text(),'Submit')]");
```

### Expected Result

Inspectors identify stable locators that can be used reliably in Selenium tests.

</details>

---

## Module 13 - Selenium WebDriver Setup and Installation

<details>
<summary>Get more details for Module 13</summary>

### What This Module Covers

- Selenium Java dependency.
- Selenium Manager and WebDriverManager.
- WebDriver interface and browser driver classes.
- First Java Selenium script.

### Java Example

```java
WebDriver driver = new ChromeDriver();
driver.manage().window().maximize();
driver.get("https://rahulshettyacademy.com/client");
System.out.println(driver.getCurrentUrl());
driver.quit();
```

### Expected Result

Chrome launches, maximizes, opens the app URL, prints the current URL, and quits.

</details>

---

## Module 14 - Selenium WebDriver Running Tests on Various Browsers

<details>
<summary>Get more details for Module 14</summary>

### What This Module Covers

- Chrome, Firefox, Edge.
- Browser driver classes.
- Cross-browser execution.
- Headless mode.
- DriverFactory pattern.

### DriverFactory Example

```java
public class DriverFactory {
    public static WebDriver createDriver(String browser) {
        switch (browser.toLowerCase()) {
            case "firefox": return new FirefoxDriver();
            case "edge": return new EdgeDriver();
            case "chrome":
            default: return new ChromeDriver();
        }
    }
}
```

### Expected Result

The same test suite can run on the browser selected by configuration or Maven parameter.

</details>

---

## Module 15 - Selenium WebDriver - Finding Elements

<details>
<summary>Get more details for Module 15</summary>

### What This Module Covers

- `findElement` vs `findElements`.
- ID, name, class, tag, link text, partial link text, CSS, XPath.
- Scope-limited searches.
- Handling empty element lists.

### Java Example

```java
driver.findElement(By.id("userEmail")).sendKeys("qa@example.com");
driver.findElement(By.id("userPassword")).sendKeys("Password123");
driver.findElement(By.id("login")).click();

List<WebElement> products = driver.findElements(By.cssSelector(".mb-3"));
Assert.assertTrue(products.size() > 0);
```

### Expected Result

Login fields are filled, login is submitted, and product cards are located.

</details>

---

## Module 16 - Cascading Style Sheets (CSS) Selectors - Advanced Locators

<details>
<summary>Get more details for Module 16</summary>

### What This Module Covers

- CSS IDs, classes, and attributes.
- Parent-child selectors.
- Contains, starts-with, and ends-with matching patterns.
- `nth-child` and hierarchy.
- Customized CSS locators based on HTML attributes.

### CSS Examples

```java
By email = By.cssSelector("#userEmail");
By password = By.cssSelector("input[type='password']");
By productCards = By.cssSelector("div.mb-3");
By addToCart = By.cssSelector(".card-body button:last-of-type");
By partialId = By.cssSelector("input[id*='Email']");
```

### Expected Result

CSS selectors locate stable elements by ID, attributes, classes, hierarchy, and partial attribute values.

</details>

---

## Module 17 - XPath - Advanced Locators

<details>
<summary>Get more details for Module 17</summary>

### What This Module Covers

- Relative XPath.
- Text-based XPath.
- `contains()` and `starts-with()`.
- Parent-child traversal.
- Child-to-parent traversal.
- Sibling traversal.
- Dynamic XPath for buttons and table cells.

### XPath Examples

```java
By loginButton = By.xpath("//input[@id='login']");
By productByText = By.xpath("//b[text()='ZARA COAT 3']");
By addToCartForProduct = By.xpath("//b[text()='ZARA COAT 3']/ancestor::div[contains(@class,'card-body')]//button[contains(text(),'Add To Cart')]");
By siblingButton = By.xpath("//td[text()='Brian']/following-sibling::td/button");
By parentInput = By.xpath("//label[text()='Email']/parent::div//input");
```

### Expected Result

XPath locators identify elements using text, parent/child relationships, and sibling relationships.

</details>

---

## Module 18 - Selenium WebDriver - Working with WebElements

<details>
<summary>Get more details for Module 18</summary>

### What This Module Covers

- Static dropdowns with `Select`.
- Dynamic dropdowns.
- Auto-suggestive dropdowns.
- Checkboxes and checkbox counts.
- Assertions.
- Calendar UI handling.
- Disabled/enabled validation.
- Java alerts.
- End-to-end UI element automation.

### Java Example

```java
Select dropdown = new Select(driver.findElement(By.id("country")));
dropdown.selectByVisibleText("United States");

List<WebElement> checkboxes = driver.findElements(By.cssSelector("input[type='checkbox']"));
Assert.assertTrue(checkboxes.size() > 0);

WebElement submit = driver.findElement(By.id("submit"));
Assert.assertTrue(submit.isEnabled());
submit.click();
```

### Expected Result

The test selects a dropdown value, validates checkbox count, confirms a button is enabled, and submits the form.

</details>

---

## Module 19 - Selenium WebDriver - Useful Methods and Properties

<details>
<summary>Get more details for Module 19</summary>

### What This Module Covers

- `getTitle`, `getCurrentUrl`, `getPageSource`.
- Window maximize and size.
- Delete cookies.
- Screenshots.
- Broken link validation with HTTP status codes.
- Element attributes and properties.

### Java Example

```java
driver.manage().window().maximize();
driver.manage().deleteAllCookies();
String title = driver.getTitle();
String url = driver.getCurrentUrl();
String href = driver.findElement(By.linkText("Broken Link")).getAttribute("href");

Assert.assertTrue(url.startsWith("https"));
Assert.assertNotNull(title);
Assert.assertNotNull(href);
```

### Expected Result

Browser window state, page metadata, and link attributes are validated.

</details>

---

## Module 20 - Selenium WebDriver - Wait Types

<details>
<summary>Get more details for Module 20</summary>

### What This Module Covers

- Implicit wait.
- Explicit wait.
- FluentWait.
- Real-time wait scenarios.
- Ajax synchronization.
- Custom wait methods.
- Polling and ignored exceptions.

### Java Example

```java
WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
wait.until(ExpectedConditions.visibilityOfElementLocated(By.cssSelector(".toast-container")));
wait.until(ExpectedConditions.invisibilityOfElementLocated(By.cssSelector(".toast-container")));
```

### FluentWait Example

```java
Wait<WebDriver> wait = new FluentWait<>(driver)
        .withTimeout(Duration.ofSeconds(20))
        .pollingEvery(Duration.ofMillis(500))
        .ignoring(NoSuchElementException.class);

WebElement result = wait.until(d -> d.findElement(By.id("result")));
```

### Expected Result

The test waits for elements to appear, disappear, or become usable without fixed sleeps.

</details>

---

## Module 21 - Selenium WebDriver – Advanced Interactions

<details>
<summary>Get more details for Module 21</summary>

### What This Module Covers

- Ajax and mouse interactions.
- Actions class real-time examples.
- Child windows.
- Frames.
- Scrolling within tables and window level using JavaScriptExecutor.
- Table grids.
- Parsing strings and validating generated sums.
- End-to-end programming exercises.

### JavaScript Scroll Example

```java
JavascriptExecutor js = (JavascriptExecutor) driver;
WebElement table = driver.findElement(By.cssSelector(".tableFixHead"));
js.executeScript("arguments[0].scrollTop = arguments[0].scrollHeight", table);
```

### Table Sum Example

```java
List<WebElement> amounts = driver.findElements(By.cssSelector(".tableFixHead td:nth-child(4)"));
int sum = amounts.stream().mapToInt(e -> Integer.parseInt(e.getText())).sum();
String totalText = driver.findElement(By.cssSelector(".totalAmount")).getText();
int displayedTotal = Integer.parseInt(totalText.replaceAll("[^0-9]", ""));
Assert.assertEquals(sum, displayedTotal);
```

### Expected Result

The table scrolls, all amount values are summed, and the calculated sum matches the displayed total.

</details>

---

## Module 22 - Selenium WebDriver - File Upload And Download

<details>
<summary>Get more details for Module 22</summary>

### What This Module Covers

- File upload with file input `sendKeys`.
- Browser download path setup.
- Validating downloaded files.
- Excel upload/download workflows.
- Toast message waits.

### Upload Example

```java
WebElement upload = driver.findElement(By.cssSelector("input[type='file']"));
upload.sendKeys(Paths.get("src/test/resources/upload.xlsx").toAbsolutePath().toString());
```

### Download Path Example

```java
Map<String, Object> prefs = new HashMap<>();
prefs.put("download.default_directory", Paths.get("downloads").toAbsolutePath().toString());
ChromeOptions options = new ChromeOptions();
options.setExperimentalOption("prefs", prefs);
WebDriver driver = new ChromeDriver(options);
```

### Expected Result

Selenium uploads the selected file and downloads files into the configured folder.

</details>

---

## Module 23 - Selenium WebDriver - Switch Window and iframes

<details>
<summary>Get more details for Module 23</summary>

### What This Module Covers

- Child windows.
- Multiple tabs.
- Window handles.
- Frames and nested frames.
- Switching back to default content.
- JavaScript alerts, confirms, and prompts.

### Java Example

```java
String parent = driver.getWindowHandle();
driver.findElement(By.id("openwindow")).click();

for (String handle : driver.getWindowHandles()) {
    if (!handle.equals(parent)) {
        driver.switchTo().window(handle);
        break;
    }
}

Assert.assertTrue(driver.getTitle().length() > 0);
driver.close();
driver.switchTo().window(parent);
```

### Iframe Example

```java
driver.switchTo().frame("courses-iframe");
driver.findElement(By.linkText("Courses")).click();
driver.switchTo().defaultContent();
```

### Expected Result

The test switches to the child window or iframe, validates content, and returns to the original context.

</details>

---

## Module 24 - Selenium WebDriver - Working with Actions Class

<details>
<summary>Get more details for Module 24</summary>

### What This Module Covers

- Mouse hover.
- Drag-and-drop.
- Right-click.
- Double-click.
- Keyboard actions.
- Composite user interactions.

### Java Example

```java
Actions actions = new Actions(driver);
WebElement menu = driver.findElement(By.id("mousehover"));
actions.moveToElement(menu).perform();
driver.findElement(By.linkText("Top")).click();
```

### Expected Result

The hover menu appears and Selenium clicks the submenu option.

</details>

---

## Module 25 - Logging Infrastructure

<details>
<summary>Get more details for Module 25</summary>

### What This Module Covers

- Log4j2 configuration.
- Console and file logs.
- Logging test start/end.
- Logging page object actions.
- Debugging failures locally and in Jenkins.

### Java Example

```java
private static final Logger logger = LogManager.getLogger(LoginTests.class);

logger.info("Starting login test");
logger.debug("Typing username");
logger.error("Login failed due to missing dashboard");
```

### Expected Result

Logs provide a readable execution trail for debugging.

</details>

---

## Module 26 - TestNG Infrastructure

<details>
<summary>Get more details for Module 26</summary>

### What This Module Covers

- TestNG advantages.
- `testng.xml`.
- Priorities, include/exclude, regex package execution.
- Annotations and helper attributes.
- Groups.
- Parameters.
- DataProvider.
- Listeners.
- Parallel execution and reports.

### Java Example

```java
@Test(groups = {"smoke", "login"}, priority = 1)
public void validLoginTest() {
    Assert.assertTrue(true);
}

@Test(dependsOnMethods = "validLoginTest")
public void orderPlacementTest() {
    Assert.assertTrue(true);
}
```

### Expected Result

TestNG controls order, dependencies, grouping, and suite execution.

</details>

---

## Module 27 - JUnit/Pytest Equivalents for Java

<details>
<summary>Get more details for Module 27</summary>

### What This Module Covers

The original 36-chapter outline mentions Unittest and Pytest. In a Java Selenium framework, the closest equivalents are **JUnit 5** and **TestNG**.

### JUnit Example

```java
@BeforeEach
void setup() {
    driver = new ChromeDriver();
}

@Test
void validTitleTest() {
    driver.get("https://example.com");
    Assertions.assertEquals("Example Domain", driver.getTitle());
}

@AfterEach
void teardown() {
    driver.quit();
}
```

### Expected Result

JUnit executes setup, test, and teardown around each test case.

</details>

---

## Module 28 - Automation Framework - Part 1

<details>
<summary>Get more details for Module 28</summary>

### What This Module Covers

- Framework design FAQs.
- Maven project and dependencies.
- Ecommerce demo app.
- WebDriverManager login script.
- Product list retrieval.
- Java Streams product selection.
- Explicit wait implementation.
- Cart and checkout validation.

### Java Example

```java
List<WebElement> products = driver.findElements(By.cssSelector(".mb-3"));
WebElement target = products.stream()
        .filter(product -> product.findElement(By.cssSelector("b")).getText().equals("ZARA COAT 3"))
        .findFirst()
        .orElseThrow();

target.findElement(By.cssSelector("button:last-of-type")).click();
```

### Expected Result

The framework selects the target ecommerce product using stream filtering.

</details>

---

## Module 29 - Automation Framework - Part 2

<details>
<summary>Get more details for Module 29</summary>

### What This Module Covers

- Page Object Model advantages.
- Login screen page object.
- PageFactory migration.
- Action methods for page WebElements.
- Abstract components.
- Product catalogue page.
- Common reusable methods.
- Complete refactor into POM.

### Page Object Example

```java
public class LandingPage extends AbstractComponent {
    WebDriver driver;

    @FindBy(id = "userEmail")
    WebElement userEmail;

    @FindBy(id = "userPassword")
    WebElement password;

    @FindBy(id = "login")
    WebElement loginButton;

    public LandingPage(WebDriver driver) {
        super(driver);
        this.driver = driver;
        PageFactory.initElements(driver, this);
    }

    public ProductCataloguePage loginApplication(String email, String pwd) {
        userEmail.sendKeys(email);
        password.sendKeys(pwd);
        loginButton.click();
        return new ProductCataloguePage(driver);
    }
}
```

### Expected Result

Tests call `loginApplication()` and receive the next page object.

</details>

---

## Module 30 - Automation Framework - Part 3

<details>
<summary>Get more details for Module 30</summary>

### What This Module Covers

- BaseTest.
- Global properties.
- Utility to launch app.
- `@BeforeMethod` driver initialization.
- Error validation test.
- Test strategy by modules.
- Test dependencies.
- Parallel TestNG XML execution.

### BaseTest Example

```java
public class BaseTest {
    public WebDriver driver;

    public WebDriver initializeDriver() throws IOException {
        Properties prop = new Properties();
        prop.load(new FileInputStream("src/test/resources/GlobalData.properties"));
        String browserName = System.getProperty("browser") != null ? System.getProperty("browser") : prop.getProperty("browser");
        driver = DriverFactory.createDriver(browserName);
        driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10));
        driver.manage().window().maximize();
        return driver;
    }
}
```

### Expected Result

The framework launches the browser based on Maven/system properties or global configuration.

</details>

---

## Module 31 - Automation Framework Practice Exercise

<details>
<summary>Get more details for Module 31</summary>

### What This Module Covers

- Real-time exercises.
- Generic calendar methods.
- End-to-end ecommerce programming.
- Reusable methods.
- Page object refactoring.
- Dynamic product/cart validation.

### Java Example

```java
@Test
public void submitOrderTest() {
    ProductCataloguePage productCatalogue = landingPage.loginApplication("user@example.com", "Password123");
    productCatalogue.addProductToCart("ZARA COAT 3");
    CartPage cartPage = productCatalogue.goToCartPage();
    Assert.assertTrue(cartPage.verifyProductDisplay("ZARA COAT 3"));
    CheckoutPage checkoutPage = cartPage.goToCheckout();
    checkoutPage.selectCountry("India");
    ConfirmationPage confirmationPage = checkoutPage.submitOrder();
    Assert.assertEquals(confirmationPage.getConfirmationMessage(), "THANKYOU FOR THE ORDER.");
}
```

### Expected Result

The test performs login, product selection, cart validation, checkout, and confirmation validation.

</details>

---

## Module 32 - Data-Driven Testing

<details>
<summary>Get more details for Module 32</summary>

### What This Module Covers

- TestNG DataProvider.
- Multidimensional arrays.
- HashMap objects as test data.
- JSON to List<HashMap>.
- Excel data with Apache POI.
- DataProvider + Excel integration.

### DataProvider Example

```java
@DataProvider
public Object[][] getData() {
    HashMap<String, String> map = new HashMap<>();
    map.put("email", "user@example.com");
    map.put("password", "Password123");
    map.put("product", "ZARA COAT 3");
    return new Object[][] {{map}};
}

@Test(dataProvider = "getData")
public void submitOrder(HashMap<String, String> input) {
    landingPage.loginApplication(input.get("email"), input.get("password"));
}
```

### Expected Result

TestNG runs tests using structured HashMap data.

</details>

---

## Module 33 - Running Complete Test Suite

<details>
<summary>Get more details for Module 33</summary>

### What This Module Covers

- Maven terminal execution.
- TestNG suite execution.
- Smoke/regression separation.
- Browser/system parameters.
- Headless execution.
- Full suite reporting.

### Commands

```bash
mvn clean test
mvn clean test -Dbrowser=chrome
mvn clean test -Dbrowser=firefox -Denv=qa
mvn clean test -DsuiteXmlFile=testng.xml
```

### Expected Result

The selected suite runs from terminal and generates TestNG/Surefire reports.

</details>

---

## Module 34 - Git and GitHub - Version Control System

<details>
<summary>Get more details for Module 34</summary>

### What This Module Covers

- Git introduction.
- GitHub importance.
- Git config and repositories.
- Staging and commits.
- Remotes and push.
- Branching.
- Merge conflicts.

### Commands

```bash
git init
git add .
git commit -m "Add Selenium framework"
git remote add origin https://github.com/BrianGator/Selenium-Automation-Advanced-Frameworks-Java-Showcase.git
git push -u origin master
```

### Expected Result

Framework source code is version-controlled and available for Jenkins/GitHub integration.

</details>

---

## Module 35 - Continuous Integration with Jenkins

<details>
<summary>Get more details for Module 35</summary>

### What This Module Covers

- Continuous integration and delivery flow.
- Jenkins WAR setup and plugins.
- GitHub integration.
- GitHub webhook trigger.
- Maven job execution.
- Parameterized Jenkins jobs.
- Headless mode.
- Scheduled and nightly jobs.

### Jenkins Pipeline Example

```groovy
pipeline {
    agent any
    tools {
        maven 'Maven-3.9'
        jdk 'JDK-17'
    }
    stages {
        stage('Checkout') {
            steps { git 'https://github.com/BrianGator/Selenium-Automation-Advanced-Frameworks-Java-Showcase.git' }
        }
        stage('Run Tests') {
            steps { sh 'mvn clean test -Dbrowser=chrome -Dheadless=true' }
        }
    }
    post {
        always {
            junit 'target/surefire-reports/*.xml'
            archiveArtifacts artifacts: 'reports/**/*, screenshots/**/*, logs/**/*', allowEmptyArchive: true
        }
    }
}
```

### Expected Result

Jenkins checks out code, runs Maven tests, publishes JUnit results, and archives reports/screenshots/logs.

</details>

---

## Module 36 - Conclusion

<details>
<summary>Get more details for Module 36</summary>

### Next Steps

- Add cloud cross-browser testing.
- Add Selenium Grid execution.
- Add API setup/cleanup tests.
- Add JDBC validations.
- Add Cucumber BDD wrapper.
- Add CDP network and JavaScript error checks.
- Add Allure or ExtentReports.
- Add Dockerized CI execution.
- Add portfolio screenshots and reports.

### Expected Result

The project becomes a complete Java Selenium automation portfolio with enterprise framework skills.

</details>

---

## Supplemental Module 37 - Selenium Java Streams for Web Tables

<details>
<summary>Get more details for Supplemental Module 37</summary>

### What This Module Covers

- Java Streams for sorting, mapping, filtering, and pagination.
- Web table sorting validation.
- Mapper methods for reusable stream logic.
- Pagination using `do while`.

### Java Example

```java
List<String> originalList = driver.findElements(By.xpath("//tr/td[1]")).stream()
        .map(WebElement::getText)
        .collect(Collectors.toList());

List<String> sortedList = originalList.stream().sorted().collect(Collectors.toList());
Assert.assertEquals(originalList, sortedList);
```

### Expected Result

The table column order is compared against a sorted copy to verify sort behavior.

</details>

---

## Supplemental Module 38 - Selenium 4.0 Latest Features

<details>
<summary>Get more details for Supplemental Module 38</summary>

### What This Module Covers

- Relative locators.
- Multiple windows/tabs.
- WebElement partial screenshots.
- Element height and width checks.
- UX validation.

### Java Example

```java
WebElement emailLabel = driver.findElement(By.xpath("//label[text()='Email']"));
WebElement emailInput = driver.findElement(RelativeLocator.with(By.tagName("input")).below(emailLabel));
emailInput.sendKeys("qa@example.com");

File logoScreenshot = driver.findElement(By.cssSelector("img.logo")).getScreenshotAs(OutputType.FILE);
Dimension size = driver.findElement(By.cssSelector("img.logo")).getSize();
Assert.assertTrue(size.getHeight() > 0);
```

### Expected Result

Selenium 4 locates elements relative to other elements and captures partial element screenshots.

</details>

---

## Supplemental Module 39 - Framework Part 4 Test Strategy and Parallel Control

<details>
<summary>Get more details for Supplemental Module 39</summary>

### What This Module Covers

- DataProvider parameterization.
- HashMap test data.
- JSON data files.
- Screenshot utility in BaseTest.
- Test groups.
- Parallel execution strategy.

### Java Example

```java
public String getScreenshot(String testCaseName, WebDriver driver) throws IOException {
    File source = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
    String path = System.getProperty("user.dir") + "/reports/" + testCaseName + ".png";
    FileUtils.copyFile(source, new File(path));
    return path;
}
```

### Expected Result

Screenshots are saved and can be attached to reports after failures.

</details>

---

## Supplemental Module 40 - Framework Part 5 Extent Reports, Listeners, ThreadLocal and Retry

<details>
<summary>Get more details for Supplemental Module 40</summary>

### What This Module Covers

- ExtentReports.
- TestNG listeners.
- Attaching screenshots to failed tests.
- ThreadLocal to avoid parallel driver conflicts.
- IRetryAnalyzer for controlled reruns.

### ThreadLocal Example

```java
private static ThreadLocal<WebDriver> driver = new ThreadLocal<>();

public static WebDriver getDriver() {
    return driver.get();
}

public static void setDriver(WebDriver webDriver) {
    driver.set(webDriver);
}
```

### Retry Example

```java
public class Retry implements IRetryAnalyzer {
    int count = 0;
    int maxTry = 1;

    public boolean retry(ITestResult result) {
        if (count < maxTry) {
            count++;
            return true;
        }
        return false;
    }
}
```

### Expected Result

Parallel tests avoid WebDriver collisions, failed tests capture report evidence, and selected failures can retry once.

</details>

---

## Supplemental Module 41 - Framework Part 6 Maven and Jenkins CI/CD

<details>
<summary>Get more details for Supplemental Module 41</summary>

### What This Module Covers

- Maven terminal execution.
- Global runtime parameters.
- Jenkins parameterized jobs.
- Headless mode.
- Nightly scheduled jobs.

### Maven Command Examples

```bash
mvn clean test -Dbrowser=chrome -Dheadless=true
mvn clean test -Dbrowser=firefox -Dgroups=smoke
mvn clean test -Denv=qa -DsuiteXmlFile=testng.xml
```

### Expected Result

Maven and Jenkins can control browser, environment, suite, and headless settings at runtime.

</details>

---

## Supplemental Module 42 - Framework Part 7 Cucumber BDD Wrapper

<details>
<summary>Get more details for Supplemental Module 42</summary>

### What This Module Covers

- Cucumber terminology.
- Feature files.
- Step definitions.
- Regex and parameterized steps.
- TestNG runner.
- Tags and background.
- Tidy Gherkin plugin concept.

### Feature File

```gherkin
Feature: Login

  Background:
    Given the user opens the login page

  @smoke
  Scenario: Valid user logs in
    When the user logs in with email "qa@example.com" and password "Password123"
    Then the dashboard should be displayed
```

### Step Definition

```java
@When("the user logs in with email {string} and password {string}")
public void login(String email, String password) {
    new LandingPage(driver).loginApplication(email, password);
}
```

### Expected Result

Business-readable Gherkin scenarios execute Selenium page object methods.

</details>

---

## Supplemental Module 43 - Cross Browser Testing with Selenium Grid and Cloud

<details>
<summary>Get more details for Supplemental Module 43</summary>

### What This Module Covers

- Selenium Grid advantages.
- Hub/node infrastructure.
- RemoteWebDriver.
- Grid health.
- Cloud vendors such as BrowserStack and Sauce Labs.
- Browser/OS combinations.

### RemoteWebDriver Example

```java
ChromeOptions options = new ChromeOptions();
WebDriver driver = new RemoteWebDriver(new URL("http://localhost:4444/wd/hub"), options);
driver.get("https://example.com");
Assert.assertEquals(driver.getTitle(), "Example Domain");
driver.quit();
```

### Expected Result

Tests execute remotely on a Grid node or cloud browser instead of the local machine.

</details>

---

## Supplemental Module 44 - Selenium 4 Chrome DevTools Protocol CDP

<details>
<summary>Get more details for Supplemental Module 44</summary>

### What This Module Covers

- Chrome DevTools Protocol concepts.
- Device metrics override for mobile emulation.
- Localization testing.
- Network responses and status codes.
- Failed request testing.
- Blocking unwanted network calls.
- Network speed emulation.
- Basic authentication.
- JavaScript error logging.

### CDP Network Blocking Example

```java
ChromeDriver driver = new ChromeDriver();
DevTools devTools = driver.getDevTools();
devTools.createSession();
devTools.send(Network.enable(Optional.empty(), Optional.empty(), Optional.empty()));
devTools.send(Network.setBlockedURLs(List.of("*.jpg", "*.png", "*.css")));
driver.get("https://example.com");
```

### Expected Result

Image/CSS requests are blocked, which can speed up test execution or validate degraded network behavior.

</details>

---

## Supplemental Module 45 - Database Connection to Selenium Testcases

<details>
<summary>Get more details for Supplemental Module 45</summary>

### What This Module Covers

- MySQL setup.
- Creating databases and tables.
- Inserting records.
- JDBC connection.
- Validating database data from Selenium tests.

### JDBC Example

```java
Connection connection = DriverManager.getConnection(
        "jdbc:mysql://localhost:3306/seleniumqa", "root", "password");
Statement statement = connection.createStatement();
ResultSet resultSet = statement.executeQuery("SELECT status FROM orders WHERE id = 1001");

if (resultSet.next()) {
    Assert.assertEquals(resultSet.getString("status"), "PLACED");
}
connection.close();
```

### Expected Result

The test validates backend database state after a UI or API action.

</details>

---

## Supplemental Module 46 - File Uploading AutoIT and Downloading with Selenium

<details>
<summary>Get more details for Supplemental Module 46</summary>

### What This Module Covers

- Window authentication popups.
- Modified URL basic-auth handling.
- AutoIT installation.
- Desktop object inspection.
- AutoIT script conversion.
- File upload through native dialogs.
- Chrome download path configuration.

### Basic Auth URL Example

```java
driver.get("https://username:password@the-internet.herokuapp.com/basic_auth");
```

### Upload Preferred Selenium Way

```java
driver.findElement(By.cssSelector("input[type='file']"))
        .sendKeys(Paths.get("src/test/resources/file.pdf").toAbsolutePath().toString());
```

### Expected Result

Basic authentication is bypassed through URL credentials, and file upload works through the file input element when available.

</details>

---

## API Tests for Selenium Java Frameworks

API testing helps set up data, validate backend behavior, and clean up data after Selenium UI tests.

### Rest Assured Dependency

```xml
<dependency>
    <groupId>io.rest-assured</groupId>
    <artifactId>rest-assured</artifactId>
    <version>5.4.0</version>
    <scope>test</scope>
</dependency>
```

### GET API Test

```java
@Test
public void getUserProfileTest() {
    given()
        .baseUri("https://api.example.com")
        .header("Authorization", "Bearer token")
    .when()
        .get("/users/123")
    .then()
        .statusCode(200)
        .body("id", equalTo(123))
        .body("email", containsString("@"));
}
```

### POST Setup for UI Test

```java
String orderId = given()
    .baseUri("https://api.example.com")
    .contentType("application/json")
    .body("{\"productId\":101,\"quantity\":1}")
.when()
    .post("/orders")
.then()
    .statusCode(201)
    .extract()
    .path("id");
```

### Expected Result

The API creates or validates data quickly, and Selenium can use the created record in UI validation.

---

## Login Tests for Selenium Java Frameworks

Login tests validate authentication, authorization, sessions, and access control.

### Login Page Object

```java
public class LoginPage {
    private WebDriver driver;
    private By email = By.id("userEmail");
    private By password = By.id("userPassword");
    private By loginButton = By.id("login");
    private By errorMessage = By.cssSelector(".toast-message");

    public LoginPage(WebDriver driver) {
        this.driver = driver;
    }

    public ProductCataloguePage login(String userEmail, String userPassword) {
        driver.findElement(email).sendKeys(userEmail);
        driver.findElement(password).sendKeys(userPassword);
        driver.findElement(loginButton).click();
        return new ProductCataloguePage(driver);
    }

    public String getErrorMessage() {
        return driver.findElement(errorMessage).getText();
    }
}
```

### Test Coverage

| Scenario | Expected Result |
|---|---|
| Valid login | User reaches product catalogue/dashboard |
| Invalid login | Error message appears |
| Empty fields | Required validation appears |
| Locked user | Locked account message appears |
| Logout | User returns to login screen |
| Expired session | User is redirected to login |
| Role-based login | Correct role-specific features appear |

---

## Locator Reference Guide

| Locator | Example | Best Use |
|---|---|---|
| ID | `By.id("userEmail")` | Best when stable and unique |
| Name | `By.name("email")` | Useful for form fields |
| CSS | `By.cssSelector("button[type='submit']")` | Fast and readable attribute/class selectors |
| XPath | `By.xpath("//button[text()='Login']")` | Text, parent/child, sibling traversal |
| Link text | `By.linkText("Forgot Password?")` | Exact anchor text |
| Partial link text | `By.partialLinkText("Forgot")` | Partial anchor text |
| Class name | `By.className("btn-primary")` | Use carefully; often not unique |
| Tag name | `By.tagName("a")` | Counting/listing elements |
| Relative locator | `RelativeLocator.with(By.tagName("input")).below(label)` | Selenium 4 relative positioning |

### Locator Best Practices

- Prefer stable IDs or test-specific attributes.
- Use CSS for attributes and hierarchy.
- Use XPath for text and relational traversal.
- Avoid absolute XPath.
- Avoid dynamic generated class names.
- Keep locators inside Page Objects.
- Validate uniqueness in DevTools or SelectorsHub.

---

## Building a Selenium Java Framework from Scratch

A custom Selenium framework is needed when the project requires reusable browser setup, configuration, page objects, waits, data-driven execution, reporting, CI/CD, parallel execution, and maintainable test organization.

### Required Framework Files

```text
selenium-java-framework/
├── pom.xml
├── testng.xml
├── Jenkinsfile
├── README.md
├── src/test/java/base/BaseTest.java
├── src/test/java/factory/DriverFactory.java
├── src/test/java/pages/LandingPage.java
├── src/test/java/pages/ProductCataloguePage.java
├── src/test/java/pages/CartPage.java
├── src/test/java/pages/CheckoutPage.java
├── src/test/java/components/AbstractComponent.java
├── src/test/java/tests/SubmitOrderTest.java
├── src/test/java/tests/ErrorValidationTest.java
├── src/test/java/utils/ConfigReader.java
├── src/test/java/utils/ExcelUtils.java
├── src/test/java/utils/JsonUtils.java
├── src/test/java/utils/ScreenshotUtils.java
├── src/test/java/listeners/TestListener.java
├── src/test/java/retry/Retry.java
├── src/test/java/api/ApiClient.java
├── src/test/resources/GlobalData.properties
├── src/test/resources/testdata/orders.json
├── src/test/resources/testdata/orders.xlsx
├── reports/
├── screenshots/
└── logs/
```

### Build Steps

1. Create Maven project.
2. Add Selenium, TestNG, WebDriverManager, Log4j, ExtentReports, Rest Assured, Jackson/Gson, and Apache POI dependencies.
3. Create global properties.
4. Build DriverFactory.
5. Build BaseTest.
6. Create AbstractComponent.
7. Create Page Object classes.
8. Add utility classes for waits, screenshots, JSON, Excel, and config.
9. Create TestNG tests.
10. Add DataProvider support.
11. Add TestNG listeners and ExtentReports.
12. Add ThreadLocal for parallel execution.
13. Add retry analyzer.
14. Add API setup/cleanup helper.
15. Add Jenkinsfile.
16. Add GitHub webhook or scheduled CI job.

### BaseTest Example

```java
public class BaseTest {
    public WebDriver driver;
    public LandingPage landingPage;

    @BeforeMethod(alwaysRun = true)
    public void launchApplication() throws IOException {
        driver = initializeDriver();
        landingPage = new LandingPage(driver);
        landingPage.goTo();
    }

    @AfterMethod(alwaysRun = true)
    public void tearDown() {
        if (driver != null) {
            driver.quit();
        }
    }
}
```

### Best Practices

- Keep business assertions in tests.
- Keep locators and UI actions in Page Objects.
- Keep shared waits in abstract components or utilities.
- Use explicit waits instead of sleeps.
- Use DataProvider/JSON/Excel for test data.
- Use ThreadLocal for parallel drivers.
- Use API calls for setup and cleanup where possible.
- Capture screenshots and logs on failure.
- Run smoke tests on every commit and full regression nightly.

---

## Build from Scratch vs Pre-Built Frameworks

### Build from Scratch When

| Scenario | Why Custom Framework Helps |
|---|---|
| Enterprise regression suite | Needs shared structure, CI/CD, roles, test data, reporting, and parallel execution |
| Complex ecommerce or workflow app | Needs Page Objects, API setup, cart/order cleanup, and reusable actions |
| Multiple QA engineers | Needs consistent naming, package organization, utilities, and standards |
| UI + API + DB validation | Needs hybrid test layers in one framework |
| Parallel execution | Needs ThreadLocal, Grid/cloud, and safe driver lifecycle |

### Use Pre-Built / Simpler Frameworks When

| Scenario | Better Choice |
|---|---|
| Learning Selenium | Simple Maven + Selenium + TestNG project |
| Small smoke suite | Minimal POM with BaseTest |
| BDD-first team | Cucumber + Selenium Java |
| Rich reporting needed quickly | Serenity BDD or Selenide + reports |
| Cross-browser infrastructure needed | BrowserStack/Sauce Labs/LambdaTest templates |

### Popular Selenium Java Framework Options

| Framework / Stack | Best Scenario |
|---|---|
| Selenium + Java + TestNG + Maven | Standard QA automation framework |
| Selenium + Java + JUnit 5 | Java engineering teams and unit/integration style projects |
| Selenium + Cucumber + Java | BDD acceptance testing |
| Selenium + Serenity BDD | Rich reports and living documentation |
| Selenide | Shorter syntax and built-in smart waits |
| Selenium Grid | Local distributed cross-browser execution |
| BrowserStack/Sauce Labs/LambdaTest | Cloud cross-browser and OS coverage |
| Rest Assured + Selenium | API setup/cleanup plus UI validation |

### Decision Rule

Use the simplest framework that solves the actual problem. Build from scratch only when repeated complexity requires custom setup, data management, reporting, and CI/CD integration.

---

## Top 30 Selenium Java Technical Interview Questions

<details open>
<summary>Click to expand Top 30 interview questions</summary>

### 1. What is Selenium WebDriver?

Selenium WebDriver is a browser automation API that sends commands to browser drivers such as ChromeDriver, GeckoDriver, and EdgeDriver.

```java
WebDriver driver = new ChromeDriver();
driver.get("https://example.com");
driver.quit();
```

### 2. What is the Selenium WebDriver architecture?

Test code communicates with the WebDriver API, which sends commands to a browser driver. The browser driver controls the browser and returns responses.

### 3. What is the difference between Selenium WebDriver and Selenium Grid?

WebDriver controls browsers. Grid distributes test execution across remote nodes, browsers, and platforms.

### 4. What are Selenium locators?

Locators identify web elements using ID, name, CSS, XPath, class name, tag name, link text, or partial link text.

### 5. Which locator is preferred?

Stable unique ID or test-specific attribute is preferred. CSS is often faster/readable. XPath is useful for text and relationships.

### 6. What is the difference between `findElement` and `findElements`?

`findElement` returns the first matching element or throws an exception. `findElements` returns a list and returns an empty list if no elements match.

### 7. What is an implicit wait?

Implicit wait polls for element lookup for a configured time.

```java
driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10));
```

### 8. What is an explicit wait?

Explicit wait waits for a specific expected condition.

```java
new WebDriverWait(driver, Duration.ofSeconds(10))
    .until(ExpectedConditions.elementToBeClickable(By.id("login")));
```

### 9. What is FluentWait?

FluentWait allows custom timeout, polling interval, and ignored exceptions.

### 10. Why avoid `Thread.sleep()`?

It creates fixed delays and increases flakiness. Use explicit waits instead.

### 11. How do you handle dropdowns?

Use `Select` for native `<select>` elements.

```java
new Select(driver.findElement(By.id("country"))).selectByVisibleText("India");
```

### 12. How do you handle dynamic dropdowns?

Type into the field, wait for suggestions, loop through suggestions, and click the matching option.

### 13. How do you handle checkboxes?

Check `isSelected()` before clicking.

```java
WebElement checkbox = driver.findElement(By.id("agree"));
if (!checkbox.isSelected()) checkbox.click();
```

### 14. How do you handle JavaScript alerts?

```java
Alert alert = driver.switchTo().alert();
alert.accept();
```

### 15. How do you handle iframes?

Switch into the frame, interact, then switch back.

```java
driver.switchTo().frame("frameName");
driver.switchTo().defaultContent();
```

### 16. How do you handle child windows?

Use window handles and switch to the child handle.

### 17. What is the Actions class used for?

Mouse hover, right-click, double-click, drag-and-drop, keyboard actions, and composite interactions.

### 18. How do you take screenshots?

```java
File src = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
```

### 19. What is JavaScriptExecutor?

It executes JavaScript in the browser from Selenium.

```java
((JavascriptExecutor) driver).executeScript("window.scrollTo(0, document.body.scrollHeight)");
```

### 20. What is Page Object Model?

POM stores locators and actions in page classes so tests remain readable and maintainable.

### 21. What is PageFactory?

PageFactory initializes fields annotated with `@FindBy`, often used in Selenium frameworks.

### 22. What is TestNG used for?

TestNG provides annotations, assertions, groups, XML suites, parameters, DataProvider, listeners, and parallel execution.

### 23. What is DataProvider?

DataProvider runs the same test with multiple data rows.

### 24. How do you run tests in parallel?

Use TestNG XML parallel mode and isolate WebDriver with ThreadLocal.

### 25. Why is ThreadLocal important?

ThreadLocal prevents parallel tests from sharing the same WebDriver instance.

### 26. What is ExtentReports used for?

ExtentReports creates rich HTML reports with test status, logs, and screenshots.

### 27. How do you run Selenium tests from Maven?

Use `mvn clean test`, usually with Surefire plugin and TestNG XML.

### 28. How do you integrate Selenium with Jenkins?

Configure Jenkins to pull from GitHub and run Maven commands, then publish JUnit results and archive artifacts.

### 29. How can API testing support Selenium?

APIs can create test data, authenticate users, validate backend state, and clean up records after UI tests.

### 30. What makes a Selenium framework maintainable?

Clear package structure, Page Objects, reusable utilities, explicit waits, configuration management, logs, reports, screenshots, ThreadLocal parallel execution, data-driven tests, and CI/CD integration.

</details>

---

## Summary

This README documents a complete advanced Selenium WebDriver with Java course and framework guide. It covers the requested 36 base modules plus non-duplicate supplemental topics drawn from the detailed Packt table of contents: Java Streams, Selenium 4 features, ExtentReports, ThreadLocal, retries, Cucumber BDD, Selenium Grid, Chrome DevTools Protocol, JDBC, AutoIT, cloud execution, API testing, login testing, locator strategy, framework construction, and interview preparation. fileciteturn45file0
