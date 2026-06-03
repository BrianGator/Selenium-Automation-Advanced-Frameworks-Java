# Selenium Automation Advanced Frameworks with Java

**Written by Brian McCarthy**

This repository is a comprehensive, visible, no-collapse Selenium WebDriver automation guide focused on **Java, Selenium WebDriver 4, TestNG, Maven, Page Object Model, framework architecture, data-driven testing, API testing, login testing, locator strategy, logging, reporting, Jenkins CI/CD, Selenium Grid, Chrome DevTools Protocol, Cucumber BDD, JDBC database validation, cloud execution, and technical interview preparation**.

All module data, explanations, code samples, expected results, best practices, and common mistakes are displayed directly on the page. No module body is hidden behind an arrow or collapsible details block.

---

## Course Table of Contents

| Module # | Module Name | Module Details |
|---:|---|---|
| 1 | [Introduction](#module-1---introduction) | Selenium purpose, WebDriver architecture, QA automation value, test pyramid context, and framework goals. |
| 2 | [Setup and Configuration](#module-2---setup-and-configuration) | Java, Maven, IDE, Selenium dependencies, WebDriverManager, Selenium Manager, browser setup, and troubleshooting. |
| 3 | [Understanding Variables and Data Types](#module-3---understanding-variables-and-data-types) | Java variables, primitive/reference types, strings, booleans, numeric values, constants, and automation runtime data. |
| 4 | [Advanced Data Types](#module-4---advanced-data-types) | Arrays, lists, maps, sets, collections, product lists, user data, locator dictionaries, and test data objects. |
| 5 | [Comparison and Boolean Operators](#module-5---comparison-and-boolean-operators) | Assertions, boolean expressions, equality, relational checks, compound UI validation, and state checks. |
| 6 | [Program Control Flow](#module-6---program-control-flow) | If/else, switch, loops, enhanced loops, while loops, table iteration, pagination, and conditional test behavior. |
| 7 | [Functions and Methods - Reusable Code](#module-7---functions-and-methods---reusable-code) | Reusable methods, parameters, return values, helper methods, custom waits, generic actions, and method design. |
| 8 | [Classes and Object-Oriented Programming](#module-8---classes-and-object-oriented-programming) | Classes, objects, constructors, inheritance, interfaces, abstract classes, overloading, overriding, encapsulation, and POM. |
| 9 | [Exception Handling](#module-9---exception-handling) | Java exception handling, Selenium exceptions, stale elements, timeouts, click interception, and failure handling. |
| 10 | [Modules and Packages](#module-10---modules-and-packages) | Java package design, Maven layout, base/pages/tests/utils/listeners/API folders, and scalable framework organization. |
| 11 | [Working with Files](#module-11---working-with-files) | Properties, JSON, Excel, CSV, screenshots, downloads, uploads, logs, test data files, and evidence files. |
| 12 | [Inspecting Elements on Different Browsers](#module-12---how-to-inspect-elements-on-different-browsers) | DevTools, DOM inspection, SelectorsHub, attributes, accessibility, dynamic elements, frames, and locator validation. |
| 13 | [Selenium WebDriver Setup and Installation](#module-13---selenium-webdriver-setup-and-installation) | Selenium Java setup, WebDriver interface, browser drivers, first script, driver lifecycle, and browser commands. |
| 14 | [Running Tests on Various Browsers](#module-14---selenium-webdriver-running-tests-on-various-browsers) | Chrome, Firefox, Edge, Safari notes, DriverFactory, headless mode, browser options, and cross-browser execution. |
| 15 | [Finding Elements](#module-15---selenium-webdriver---finding-elements) | ID, name, class, tag, link text, CSS, XPath, findElement, findElements, scoped lookup, and dynamic locator strategy. |
| 16 | [CSS Selectors - Advanced Locators](#module-16---cascading-style-sheets-css-selectors---advanced-locators) | CSS ID/class/attribute selectors, contains, starts-with, ends-with, hierarchy, nth-child, and selector quality. |
| 17 | [XPath - Advanced Locators](#module-17---xpath---advanced-locators) | XPath text, contains, starts-with, axes, parent/child/sibling traversal, dynamic XPath, and best practices. |
| 18 | [Working with WebElements](#module-18---selenium-webdriver---working-with-webelements) | Inputs, buttons, checkboxes, radio buttons, dropdowns, dynamic dropdowns, calendars, alerts, and element states. |
| 19 | [Useful Methods and Properties](#module-19---selenium-webdriver---useful-methods-and-properties) | URL, title, page source, cookies, window state, screenshots, attributes, text, size, broken links, and status checks. |
| 20 | [Wait Types](#module-20---selenium-webdriver---wait-types) | Implicit wait, explicit wait, FluentWait, ExpectedConditions, polling, ignored exceptions, and synchronization strategy. |
| 21 | [Advanced Interactions](#module-21---selenium-webdriver--advanced-interactions) | Ajax, JavaScriptExecutor, scrolling, tables, calendars, generated totals, mouse actions, and real-world UI workflows. |
| 22 | [File Upload and Download](#module-22---selenium-webdriver---file-upload-and-download) | Upload input, download preferences, file validation, Excel upload/download, native dialog limits, and AutoIT notes. |
| 23 | [Switch Windows and Iframes](#module-23---selenium-webdriver---switch-window-and-iframes) | Alerts, prompts, child windows, tabs, frame switching, nested frames, default content, and context management. |
| 24 | [Actions Class](#module-24---selenium-webdriver---working-with-actions-class) | Mouse hover, drag-and-drop, keyboard actions, context click, double click, sliders, composite actions, and realistic events. |
| 25 | [Logging Infrastructure](#module-25---logging-infrastructure) | Log4j2, log levels, appenders, framework logs, CI logs, page action logs, and debugging standards. |
| 26 | [TestNG Infrastructure](#module-26---testng-infrastructure) | TestNG annotations, groups, priorities, dependencies, XML suites, parameters, DataProvider, listeners, and parallel runs. |
| 27 | [JUnit/Pytest Equivalents for Java](#module-27---junitpytest-equivalents-for-java) | JUnit 5 vs TestNG, lifecycle hooks, assertions, tags, parameterized tests, and Java alternatives to Python test runners. |
| 28 | [Automation Framework - Part 1](#module-28---automation-framework---part-1) | Maven framework start, ecommerce app, login flow, product selection, waits, cart/checkout validation, and first framework test. |
| 29 | [Automation Framework - Part 2](#module-29---automation-framework---part-2) | Page Object Model, PageFactory, abstract components, page actions, product catalogue, and POM refactoring. |
| 30 | [Automation Framework - Part 3](#module-30---automation-framework---part-3) | BaseTest, global properties, driver initialization, error tests, TestNG groups, dependencies, and parallel XML execution. |
| 31 | [Automation Framework Practice Exercise](#module-31---automation-framework-practice-exercise) | End-to-end ecommerce practice, reusable methods, calendar handling, dynamic locators, and framework refactoring. |
| 32 | [Data-Driven Testing](#module-32---data-driven-testing) | TestNG DataProvider, arrays, HashMap, JSON, Excel, Apache POI, user/product datasets, and data utility design. |
| 33 | [Running Complete Test Suite](#module-33---running-complete-test-suite) | Maven commands, TestNG suites, smoke/regression execution, browser parameters, headless mode, reports, and local runs. |
| 34 | [Git and GitHub Version Control](#module-34---git-and-github---version-control-system) | Git config, staging, commits, branches, remotes, GitHub push/pull, merge conflicts, and framework versioning. |
| 35 | [Continuous Integration with Jenkins](#module-35---continuous-integration-with-jenkins) | Jenkins setup, Git integration, Maven jobs, parameters, scheduled runs, artifacts, reports, and CI/CD flow. |
| 36 | [Conclusion](#module-36---conclusion) | Framework maturity roadmap, next steps, Grid/cloud/CDP/API/BDD/reporting expansion, and portfolio improvement. |
| 37 | [Supplemental: Java Streams for Web Tables](#supplemental-module-37---selenium-java-streams-for-web-tables) | Streams, sorting, filtering, pagination, mapping WebElements to text, and stream-based web table assertions. |
| 38 | [Supplemental: Selenium 4 Features](#supplemental-module-38---selenium-40-latest-features) | Relative locators, tabs/windows API, element screenshots, dimensions, and Selenium 4 improvements. |
| 39 | [Supplemental: Framework Part 4 - Test Strategy and Parallel Control](#supplemental-module-39---framework-part-4-test-strategy-and-parallel-control) | Test strategy, JSON/HashMap data, screenshots, groups, parallel classes, and suite partitioning. |
| 40 | [Supplemental: Framework Part 5 - Extent Reports, Listeners, ThreadLocal, Retry](#supplemental-module-40---framework-part-5-extent-reports-listeners-threadlocal-and-retry) | ExtentReports, TestNG listeners, screenshot attachments, ThreadLocal WebDriver, retries, and parallel-safe reporting. |
| 41 | [Supplemental: Framework Part 6 - Maven and Jenkins CI/CD](#supplemental-module-41---framework-part-6-maven-and-jenkins-cicd) | Maven terminal runs, Jenkins parameters, headless mode, scheduled jobs, and environment-controlled CI execution. |
| 42 | [Supplemental: Framework Part 7 - Cucumber BDD Wrapper](#supplemental-module-42---framework-part-7-cucumber-bdd-wrapper) | Cucumber features, step definitions, runner, tags, background, TestNG integration, and BDD wrapper design. |
| 43 | [Supplemental: Selenium Grid and Cloud Testing](#supplemental-module-43---cross-browser-testing-with-selenium-grid-and-cloud) | Selenium Grid, RemoteWebDriver, cloud vendors, BrowserStack, Sauce Labs, capabilities, and parallel browser coverage. |
| 44 | [Supplemental: Selenium 4 Chrome DevTools Protocol](#supplemental-module-44---selenium-4-chrome-devtools-protocol-cdp) | CDP, device emulation, network blocking, response codes, throttling, basic auth, and JavaScript error capture. |
| 45 | [Supplemental: Database Testing with JDBC](#supplemental-module-45---database-connection-to-selenium-testcases) | MySQL, JDBC, SQL queries, UI-to-database validation, backend data verification, and cleanup. |
| 46 | [Supplemental: AutoIT and Native Dialogs](#supplemental-module-46---file-uploading-autoit-and-downloading-with-selenium) | Native dialogs, authentication popups, AutoIT use cases, file upload/download, and Selenium alternatives. |
| 47 | [API Tests for Selenium Java Frameworks](#api-tests-for-selenium-java-frameworks) | Rest Assured setup, GET/POST/PUT/PATCH/DELETE, auth, API setup/cleanup, and UI/API hybrid strategy. |
| 48 | [Login Tests for Selenium Java Frameworks](#login-tests-for-selenium-java-frameworks) | Valid login, invalid login, empty fields, locked user, logout, session expiration, role-based login, and secure credentials. |
| 49 | [Locator Reference Guide](#locator-reference-guide) | Locator types, examples, when to use each, locator priority, dynamic locator anti-patterns, and robust locator design. |
| 50 | [Building a Selenium Java Framework from Scratch](#building-a-selenium-java-framework-from-scratch) | Required files, dependencies, folder structure, BaseTest, DriverFactory, POM, utilities, listeners, reporting, API helpers, and CI/CD. |
| 51 | [Build from Scratch vs Pre-Built Frameworks](#build-from-scratch-vs-pre-built-frameworks) | When to build custom, when to use simpler/pre-built stacks, popular frameworks, and scenario-based recommendations. |
| 52 | [Top 30 Selenium Java Technical Interview Questions](#top-30-selenium-java-technical-interview-questions) | Technical interview Q&A with code examples for WebDriver, waits, locators, POM, TestNG, Grid, API, CI/CD, and frameworks. |

---

## Project Overview

This project documents a full Selenium WebDriver with Java automation path from beginner-level Java concepts through advanced enterprise test framework architecture. It is intended to show practical QA automation capability across UI testing, backend-assisted testing, CI/CD execution, reporting, debugging, parallel execution, and framework maintainability.

The repository is organized around a 36-module Selenium course structure and then expanded with supplemental advanced topics that are common in professional automation roles. The goal is not only to show Selenium syntax, but to explain how a maintainable automation framework is designed, executed, debugged, and scaled.

### What a Complete Selenium Java Automation Framework Should Demonstrate

| Capability | Why It Matters |
|---|---|
| Browser automation | Validates user workflows in real browsers. |
| Page Object Model | Keeps locators and page actions maintainable. |
| Explicit waits | Reduces flaky tests caused by timing issues. |
| Data-driven execution | Runs the same test with multiple users/products/roles. |
| API setup/cleanup | Makes UI tests faster and cleaner. |
| Logging and screenshots | Provides failure evidence for debugging. |
| TestNG suites/groups | Supports smoke, regression, login, API, and parallel execution. |
| Jenkins CI/CD | Executes tests automatically after code changes or on schedules. |
| Grid/cloud execution | Expands browser and platform coverage. |
| Interview readiness | Shows ability to explain architecture, not just write scripts. |

---

## Module 1 - Introduction

### Deep Dive

Selenium WebDriver is used to automate browser interactions exactly as a user would interact with a web application. It supports actions such as opening a URL, clicking links and buttons, entering text, selecting dropdown values, handling popups, validating content, and capturing evidence. Selenium is widely used for regression testing, smoke testing, cross-browser testing, and CI/CD quality gates.

Selenium WebDriver is different from record-and-playback tools because it allows engineers to build scalable code-based automation. A professional Selenium project should not be a collection of random scripts. It should evolve into a test framework that separates tests, page actions, locators, data, utilities, configuration, and reporting.

### Important Concepts

| Concept | Explanation |
|---|---|
| Selenium WebDriver | Java API used to control browsers. |
| Browser driver | Browser-specific executable or service that controls Chrome, Firefox, Edge, etc. |
| WebDriver protocol | Command model used to send browser automation instructions. |
| Test framework | TestNG/JUnit structure that runs and reports tests. |
| Automation framework | Full architecture including WebDriver, waits, POM, reports, data, CI/CD, and utilities. |

### Java Example

```java
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class FirstSeleniumTest {
    public static void main(String[] args) {
        WebDriver driver = new ChromeDriver();
        driver.get("https://example.com");
        System.out.println("Title: " + driver.getTitle());
        System.out.println("URL: " + driver.getCurrentUrl());
        driver.quit();
    }
}
```

### Expected Result

```text
Title: Example Domain
URL: https://example.com/
```

### Best Practices

- Always close the browser with `quit()`.
- Keep beginner scripts simple, then refactor into framework classes.
- Do not hardcode repeated values across many tests.
- Learn WebDriver fundamentals before jumping into advanced frameworks.

### Common Mistakes

- Writing all test logic inside one large class.
- Not closing the browser after execution.
- Using sleeps instead of waits.
- Mixing test assertions, locators, and framework setup in the same method.

---

## Module 2 - Setup and Configuration

### Deep Dive

A stable setup is the foundation of Selenium automation. Java must be installed correctly, Maven must manage dependencies, the IDE must recognize the project, and browsers must be available for execution. Selenium 4 can use Selenium Manager to resolve drivers, but many frameworks still use WebDriverManager for explicit driver setup.

### Required Tools

| Tool | Purpose |
|---|---|
| Java JDK 17+ | Runs Java tests and Maven builds. |
| Maven | Manages dependencies and test execution. |
| IntelliJ IDEA or Eclipse | IDE for writing and debugging code. |
| Selenium Java | WebDriver automation library. |
| TestNG | Test execution framework. |
| WebDriverManager | Optional driver binary management. |
| Chrome/Firefox/Edge | Browsers for local execution. |
| Git | Version control. |
| Jenkins | CI/CD execution. |

### `pom.xml` Dependencies

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
    <dependency>
        <groupId>org.apache.logging.log4j</groupId>
        <artifactId>log4j-api</artifactId>
        <version>2.23.1</version>
    </dependency>
    <dependency>
        <groupId>org.apache.logging.log4j</groupId>
        <artifactId>log4j-core</artifactId>
        <version>2.23.1</version>
    </dependency>
    <dependency>
        <groupId>io.rest-assured</groupId>
        <artifactId>rest-assured</artifactId>
        <version>5.4.0</version>
        <scope>test</scope>
    </dependency>
</dependencies>
```

### Maven Surefire Plugin

```xml
<build>
    <plugins>
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-surefire-plugin</artifactId>
            <version>3.2.5</version>
            <configuration>
                <suiteXmlFiles>
                    <suiteXmlFile>testng.xml</suiteXmlFile>
                </suiteXmlFiles>
            </configuration>
        </plugin>
    </plugins>
</build>
```

### First TestNG Test

```java
public class SetupSmokeTest {
    @Test
    public void openBrowserTest() {
        WebDriver driver = new ChromeDriver();
        driver.get("https://example.com");
        Assert.assertEquals(driver.getTitle(), "Example Domain");
        driver.quit();
    }
}
```

### Expected Result

`mvn test` downloads dependencies, opens Chrome, validates the title, closes the browser, and shows a passing TestNG/Surefire result.

### Best Practices

- Use Maven instead of manually adding JARs.
- Keep dependency versions in `pom.xml`.
- Use one Java version consistently locally and in CI.
- Use browser options for headless CI runs.
- Commit `pom.xml`, `testng.xml`, and source code; do not commit generated reports or browser drivers.

### Common Mistakes

- Installing JRE instead of JDK.
- Forgetting to import Maven dependencies.
- Running tests from IDE only and never validating Maven command-line execution.
- Using different Java versions locally and in Jenkins.

---

## Module 3 - Understanding Variables and Data Types

### Deep Dive

Variables store runtime values such as URLs, credentials, browser names, expected titles, timeout values, element text, product names, prices, and API response values. Java is statically typed, so type selection matters.

### Common Automation Variables

| Data Type | Selenium Use Case |
|---|---|
| `String` | URLs, credentials, expected messages, locator text. |
| `int` | Timeouts, counts, retry limits, table row numbers. |
| `double` | Prices, totals, tax values, numeric comparison. |
| `boolean` | Element state, test flags, headless mode, success/failure checks. |
| `WebElement` | Represents one element on the page. |
| `List<WebElement>` | Represents multiple matching elements. |

### Java Example

```java
String baseUrl = "https://example.com";
String expectedTitle = "Example Domain";
int explicitWaitSeconds = 10;
boolean shouldMaximize = true;

driver.get(baseUrl);
if (shouldMaximize) {
    driver.manage().window().maximize();
}

String actualTitle = driver.getTitle();
Assert.assertEquals(actualTitle, expectedTitle);
Assert.assertTrue(explicitWaitSeconds > 0);
```

### Price Parsing Example

```java
String priceText = "$149.99";
double price = Double.parseDouble(priceText.replace("$", ""));
Assert.assertTrue(price > 0);
```

### Expected Result

The test navigates to the target URL, optionally maximizes the browser, validates the title, and parses string-based price data into a numeric value.

### Best Practices

- Use meaningful variable names like `expectedTitle`, `actualMessage`, and `timeoutSeconds`.
- Avoid magic numbers; store timeouts as named values.
- Use `final` for constants.
- Parse text carefully when validating prices and totals.

### Common Mistakes

- Comparing strings with `==` instead of `.equals()`.
- Leaving credentials as hardcoded strings.
- Parsing prices without removing currency symbols.
- Using one variable for multiple unrelated meanings.

---

## Module 4 - Advanced Data Types

### Deep Dive

Advanced data types help manage multiple values in framework code. Lists store products, links, rows, or test users. Maps store key-value pairs such as configuration or test payloads. Sets store unique values and are useful for window handles.

### Data Structure Reference

| Structure | Selenium Use Case |
|---|---|
| Array | Fixed set of browsers or roles. |
| ArrayList | Product names, links, table values. |
| HashMap | Login credentials, JSON-style test data. |
| Set | Window handles, unique text values. |
| List<WebElement> | Multiple matching DOM elements. |

### List Example

```java
List<String> expectedProducts = Arrays.asList("ZARA COAT 3", "ADIDAS ORIGINAL", "IPHONE 13 PRO");
List<WebElement> productCards = driver.findElements(By.cssSelector(".mb-3"));

for (WebElement card : productCards) {
    String productName = card.findElement(By.cssSelector("b")).getText();
    if (expectedProducts.contains(productName)) {
        card.findElement(By.cssSelector("button:last-of-type")).click();
    }
}
```

### HashMap Test Data Example

```java
HashMap<String, String> user = new HashMap<>();
user.put("email", "qa@example.com");
user.put("password", "Password123");
user.put("role", "admin");

Assert.assertEquals(user.get("role"), "admin");
```

### Window Handles Set Example

```java
Set<String> handles = driver.getWindowHandles();
for (String handle : handles) {
    driver.switchTo().window(handle);
    System.out.println(driver.getTitle());
}
```

### Expected Result

The automation can process multiple products, store structured test data, and switch across browser windows using collections.

### Best Practices

- Use `List<WebElement>` for DOM collections.
- Use `HashMap<String, String>` for simple test data records.
- Use custom model classes for complex records.
- Use `Set<String>` for unique handles.

### Common Mistakes

- Assuming `findElements()` throws an exception when no elements exist; it returns an empty list.
- Using indexes when product text or IDs are more stable.
- Mutating shared collection data across parallel tests.

---

## Module 5 - Comparison and Boolean Operators

### Deep Dive

Comparison and boolean operators power assertions and decision logic. Selenium tests constantly ask questions such as: is the button visible, is the checkbox selected, does the URL contain the expected path, does the table include a product, or does the error message match the expected text?

### Java Example

```java
WebElement loginButton = driver.findElement(By.id("login"));
boolean visible = loginButton.isDisplayed();
boolean enabled = loginButton.isEnabled();

Assert.assertTrue(visible && enabled, "Login button should be visible and enabled");
```

### String Comparison Example

```java
String actualMessage = driver.findElement(By.cssSelector(".toast-message")).getText();
String expectedMessage = "Login Successfully";
Assert.assertTrue(actualMessage.contains("Login"));
Assert.assertEquals(actualMessage, expectedMessage);
```

### URL Logic Example

```java
String currentUrl = driver.getCurrentUrl();
Assert.assertTrue(currentUrl.contains("dashboard") || currentUrl.contains("products"));
```

### Expected Result

The test passes only when the UI state satisfies the expected boolean conditions.

### Best Practices

- Use descriptive assertion messages.
- Use `.equals()` or TestNG assertions for string values.
- Use compound boolean expressions only when readable.
- Split complex validations into smaller assertions.

### Common Mistakes

- Using `==` for strings.
- Creating unreadable assertions with too many `&&` and `||` checks.
- Not validating both visibility and enabled state before clicking.

---

## Module 6 - Program Control Flow

### Deep Dive

Control flow allows test code to make decisions, repeat actions, and stop once the desired condition is met. Real applications often require looping through product cards, rows, pagination pages, autocomplete suggestions, or calendar dates.

### If/Else Example

```java
WebElement error = driver.findElement(By.cssSelector(".error"));
if (error.isDisplayed()) {
    Assert.assertTrue(error.getText().contains("Invalid"));
} else {
    Assert.fail("Expected error message was not displayed");
}
```

### Product Loop Example

```java
List<WebElement> products = driver.findElements(By.cssSelector(".product"));
for (WebElement product : products) {
    String name = product.findElement(By.cssSelector(".product-name")).getText();
    if (name.equalsIgnoreCase("Laptop")) {
        product.findElement(By.cssSelector("button.add")).click();
        break;
    }
}
```

### Pagination Example

```java
boolean itemFound = false;
do {
    List<WebElement> rows = driver.findElements(By.cssSelector("table tbody tr"));
    itemFound = rows.stream().anyMatch(row -> row.getText().contains("Rice"));
    if (!itemFound) {
        driver.findElement(By.cssSelector("[aria-label='Next']")).click();
    }
} while (!itemFound);

Assert.assertTrue(itemFound);
```

### Expected Result

The automation searches through current and next pages until it finds the required item.

### Best Practices

- Break loops when the target is found.
- Use streams for readable filtering when appropriate.
- Add maximum retry/page limits to avoid infinite loops.
- Prefer test data that makes branching predictable.

### Common Mistakes

- Infinite loops in pagination.
- Clicking the wrong repeated element because of index misuse.
- Not waiting after moving to the next page.

---

## Module 7 - Functions and Methods - Reusable Code

### Deep Dive

Reusable methods turn repeated test steps into maintainable utilities. Professional Selenium frameworks should have reusable methods for wait, click, type, select, screenshot, scroll, API setup, test data loading, and assertions.

### Utility Method Example

```java
public class ElementUtils {
    private WebDriver driver;
    private WebDriverWait wait;

    public ElementUtils(WebDriver driver) {
        this.driver = driver;
        this.wait = new WebDriverWait(driver, Duration.ofSeconds(10));
    }

    public WebElement waitForVisible(By locator) {
        return wait.until(ExpectedConditions.visibilityOfElementLocated(locator));
    }

    public void click(By locator) {
        wait.until(ExpectedConditions.elementToBeClickable(locator)).click();
    }

    public void type(By locator, String value) {
        WebElement element = waitForVisible(locator);
        element.clear();
        element.sendKeys(value);
    }

    public String getText(By locator) {
        return waitForVisible(locator).getText();
    }
}
```

### Usage Example

```java
ElementUtils elementUtils = new ElementUtils(driver);
elementUtils.type(By.id("userEmail"), "qa@example.com");
elementUtils.type(By.id("userPassword"), "Password123");
elementUtils.click(By.id("login"));
```

### Expected Result

Tests interact with the page using consistent wait-aware helper methods.

### Best Practices

- Keep methods small and single-purpose.
- Return page objects from page action methods when navigation occurs.
- Do not hide assertions inside low-level utility methods unless clearly named.
- Use meaningful method names like `loginApplication`, `addProductToCart`, and `selectCountry`.

### Common Mistakes

- Creating one giant utility class with unrelated methods.
- Making all methods static unnecessarily.
- Catching exceptions silently in utility methods.

---

## Module 8 - Classes and Object-Oriented Programming

### Deep Dive

OOP allows a Selenium framework to be modular and maintainable. Page classes represent screens, component classes represent shared UI elements, utility classes provide reusable services, and factory classes create drivers or API clients.

### Core OOP Concepts in Frameworks

| OOP Concept | Framework Example |
|---|---|
| Class | `LoginPage`, `BaseTest`, `DriverFactory`. |
| Object | Instance of a page class used by a test. |
| Encapsulation | Locators kept private inside page objects. |
| Inheritance | Page classes extend `AbstractComponent`. |
| Polymorphism | WebDriver variable can hold ChromeDriver/FirefoxDriver. |
| Interface | Driver provider or reporting provider contract. |
| Abstract class | Shared navigation/wait functionality. |

### Abstract Component Example

```java
public abstract class AbstractComponent {
    protected WebDriver driver;
    protected WebDriverWait wait;

    public AbstractComponent(WebDriver driver) {
        this.driver = driver;
        this.wait = new WebDriverWait(driver, Duration.ofSeconds(10));
    }

    public void waitForElementToAppear(By locator) {
        wait.until(ExpectedConditions.visibilityOfElementLocated(locator));
    }

    public void waitForElementToDisappear(By locator) {
        wait.until(ExpectedConditions.invisibilityOfElementLocated(locator));
    }
}
```

### Page Object Inheritance Example

```java
public class ProductCataloguePage extends AbstractComponent {
    private By productsBy = By.cssSelector(".mb-3");

    public ProductCataloguePage(WebDriver driver) {
        super(driver);
    }

    public List<WebElement> getProductList() {
        waitForElementToAppear(productsBy);
        return driver.findElements(productsBy);
    }
}
```

### Expected Result

Common page behavior is inherited, reducing duplication across page classes.

### Best Practices

- Use private locators in page classes.
- Use public page action methods that describe business behavior.
- Return next page objects from actions that navigate.
- Keep test methods readable and high-level.

### Common Mistakes

- Putting all locators in test classes.
- Overusing inheritance when composition would be simpler.
- Exposing WebElements publicly from page objects.

---

## Module 9 - Exception Handling

### Deep Dive

Exception handling is necessary for reliable diagnostics, but it should not hide real bugs. A good framework uses waits to prevent common timing failures, captures screenshots/logs on failure, and throws meaningful errors when test expectations are not met.

### Common Selenium Exceptions

| Exception | Cause | Fix |
|---|---|---|
| `NoSuchElementException` | Locator did not match any element. | Check locator and wait strategy. |
| `TimeoutException` | Expected condition did not happen in time. | Check app timing or locator. |
| `StaleElementReferenceException` | DOM refreshed after element was found. | Re-locate the element. |
| `ElementClickInterceptedException` | Overlay or another element blocks click. | Wait for overlay to disappear. |
| `NoSuchFrameException` | Frame not found or not loaded. | Wait and switch correctly. |
| `NoSuchWindowException` | Window handle is invalid/closed. | Manage handles carefully. |

### Exception Handling Example

```java
public void safeClick(By locator) {
    try {
        WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
        wait.until(ExpectedConditions.elementToBeClickable(locator)).click();
    } catch (ElementClickInterceptedException e) {
        WebElement element = driver.findElement(locator);
        ((JavascriptExecutor) driver).executeScript("arguments[0].click();", element);
    } catch (TimeoutException e) {
        throw new AssertionError("Element was not clickable: " + locator, e);
    }
}
```

### Screenshot on Failure Example

```java
public static String captureScreenshot(WebDriver driver, String testName) throws IOException {
    File source = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
    String path = System.getProperty("user.dir") + "/screenshots/" + testName + ".png";
    FileUtils.copyFile(source, new File(path));
    return path;
}
```

### Expected Result

Failures produce meaningful messages and screenshot evidence rather than vague stack traces only.

### Best Practices

- Prefer waits over try/catch for timing issues.
- Throw meaningful assertion errors.
- Capture screenshots only on failure to avoid noise.
- Log the locator and action being attempted.

### Common Mistakes

- Catching exceptions and continuing tests incorrectly.
- Using JavaScript click for every click instead of fixing timing/locator issues.
- Retrying tests without investigating root causes.

---

## Module 10 - Modules and Packages

### Deep Dive

A professional Java framework separates code by responsibility. This makes the framework easier to scale, review, debug, and maintain.

### Recommended Package Structure

```text
src/test/java/
├── api/
│   └── ApiClient.java
├── base/
│   └── BaseTest.java
├── components/
│   └── AbstractComponent.java
├── factory/
│   └── DriverFactory.java
├── listeners/
│   └── TestListener.java
├── pages/
│   ├── LandingPage.java
│   ├── ProductCataloguePage.java
│   ├── CartPage.java
│   └── CheckoutPage.java
├── retry/
│   └── RetryAnalyzer.java
├── tests/
│   ├── SubmitOrderTest.java
│   ├── ErrorValidationTest.java
│   └── LoginTest.java
└── utils/
    ├── ConfigReader.java
    ├── ExcelUtils.java
    ├── JsonUtils.java
    └── ScreenshotUtils.java
```

### Resource Structure

```text
src/test/resources/
├── GlobalData.properties
├── log4j2.xml
├── testdata/
│   ├── orders.json
│   ├── login-data.xlsx
│   └── users.csv
└── files/
    └── upload.xlsx
```

### Expected Result

The project is organized so that tests, pages, setup, utilities, reports, and data are easy to locate.

### Best Practices

- Keep package names lower-case.
- Keep page classes in `pages`.
- Keep TestNG tests in `tests`.
- Keep reusable infrastructure out of test classes.
- Keep resources under `src/test/resources`.

### Common Mistakes

- Placing everything in the default package.
- Mixing API helpers with page object code.
- Storing test data in Java classes instead of resource files.

---

## Module 11 - Working with Files

### Deep Dive

Selenium frameworks use files for configuration, data, logs, screenshots, reports, uploads, and downloads. File handling should be reliable across local machines and CI systems.

### Properties File Example

```properties
browser=chrome
baseUrl=https://rahulshettyacademy.com/client
headless=false
timeout=10
```

### Config Reader

```java
public class ConfigReader {
    private static Properties properties = new Properties();

    static {
        try (FileInputStream input = new FileInputStream("src/test/resources/GlobalData.properties")) {
            properties.load(input);
        } catch (IOException e) {
            throw new RuntimeException("Unable to load config file", e);
        }
    }

    public static String get(String key) {
        return System.getProperty(key) != null ? System.getProperty(key) : properties.getProperty(key);
    }
}
```

### JSON Test Data Example

```json
[
  {
    "email": "user@example.com",
    "password": "Password123",
    "product": "ZARA COAT 3"
  }
]
```

### Download Validation Example

```java
Path downloadPath = Paths.get("downloads", "invoice.pdf");
Assert.assertTrue(Files.exists(downloadPath), "Downloaded invoice should exist");
Assert.assertTrue(Files.size(downloadPath) > 0, "Downloaded invoice should not be empty");
```

### Expected Result

The framework reads runtime settings and test data from files and validates file output such as downloads and screenshots.

### Best Practices

- Use relative paths from project root.
- Keep secrets out of committed files.
- Add generated folders to `.gitignore`.
- Use resource files for stable test data.

### Common Mistakes

- Hardcoding absolute paths like `C:\Users\...`.
- Committing screenshots/reports/downloads to the repository.
- Not closing file streams.

---

## Module 12 - How To Inspect Elements On Different Browsers

### Deep Dive

Element inspection is how automation engineers identify stable locators. DevTools helps inspect the DOM, attributes, text, frames, network calls, and dynamic rendering.

### What to Inspect

| Item | Why It Matters |
|---|---|
| `id` | Often the most stable locator. |
| `name` | Useful for forms. |
| `data-testid` | Best test-specific locator when available. |
| `aria-label` | Useful for accessible controls. |
| Text | Useful for buttons, links, headings, and labels. |
| Parent-child relationship | Useful when multiple similar controls exist. |
| Iframes | Must switch into iframe before locating elements. |
| Dynamic classes | Often unstable; avoid when generated. |

### Locator Discovery Example

```java
By email = By.id("userEmail");
By password = By.cssSelector("input[type='password']");
By submit = By.cssSelector("button[type='submit']");
By error = By.xpath("//div[contains(@class,'toast') and contains(text(),'Incorrect')]");
```

### DevTools Workflow

1. Right-click element and select Inspect.
2. Check if ID or data attribute exists.
3. Test CSS selector in browser console with `document.querySelector()`.
4. Test XPath with `$x("//button[text()='Login']")`.
5. Confirm locator returns exactly one element.
6. Check if the element is inside an iframe.

### Expected Result

Stable locators are identified and validated before being added to Page Objects.

### Best Practices

- Prefer `id`, `name`, `data-testid`, or stable CSS.
- Use XPath for text/relationship cases.
- Avoid brittle absolute XPath.
- Avoid dynamic generated classes.

### Common Mistakes

- Copying long absolute XPath from DevTools.
- Using a locator that matches multiple elements without realizing it.
- Forgetting to switch into iframes.

---

## Module 13 - Selenium WebDriver Setup and Installation

### Deep Dive

The WebDriver interface is the main Selenium entry point. Browser-specific classes such as ChromeDriver, FirefoxDriver, and EdgeDriver implement WebDriver.

### Basic WebDriver Commands

```java
WebDriver driver = new ChromeDriver();
driver.manage().window().maximize();
driver.get("https://rahulshettyacademy.com/client");
System.out.println(driver.getTitle());
System.out.println(driver.getCurrentUrl());
driver.navigate().to("https://example.com");
driver.navigate().back();
driver.navigate().forward();
driver.navigate().refresh();
driver.quit();
```

### WebDriverManager Setup

```java
WebDriverManager.chromedriver().setup();
WebDriver driver = new ChromeDriver();
```

### Browser Options Example

```java
ChromeOptions options = new ChromeOptions();
options.addArguments("--start-maximized");
options.addArguments("--disable-notifications");
WebDriver driver = new ChromeDriver(options);
```

### Expected Result

The browser launches reliably and executes navigation commands.

### Best Practices

- Use `quit()` instead of `close()` at the end of tests.
- Centralize driver creation in a factory.
- Use browser options for CI compatibility.
- Avoid creating WebDriver directly in every test.

### Common Mistakes

- Creating multiple drivers in one test accidentally.
- Forgetting to close browser sessions.
- Placing browser setup inside page objects.

---

## Module 14 - Selenium WebDriver Running Tests on Various Browsers

### Deep Dive

Cross-browser testing verifies that the same workflow behaves correctly across different rendering engines and browsers. A framework should allow the browser to be selected at runtime without changing code.

### DriverFactory Example

```java
public class DriverFactory {
    public static WebDriver createDriver(String browser, boolean headless) {
        switch (browser.toLowerCase()) {
            case "firefox":
                FirefoxOptions firefoxOptions = new FirefoxOptions();
                if (headless) firefoxOptions.addArguments("--headless");
                return new FirefoxDriver(firefoxOptions);
            case "edge":
                EdgeOptions edgeOptions = new EdgeOptions();
                if (headless) edgeOptions.addArguments("--headless");
                return new EdgeDriver(edgeOptions);
            case "chrome":
            default:
                ChromeOptions chromeOptions = new ChromeOptions();
                if (headless) chromeOptions.addArguments("--headless=new");
                chromeOptions.addArguments("--window-size=1920,1080");
                return new ChromeDriver(chromeOptions);
        }
    }
}
```

### Maven Runtime Example

```bash
mvn clean test -Dbrowser=chrome -Dheadless=true
mvn clean test -Dbrowser=firefox
mvn clean test -Dbrowser=edge
```

### Expected Result

The same test suite runs on Chrome, Firefox, or Edge based on runtime configuration.

### Best Practices

- Test smoke flows in multiple browsers.
- Run full cross-browser regression on release builds or nightly schedules.
- Use headless mode in CI if no display is available.
- Keep browser-specific workarounds isolated in DriverFactory.

### Common Mistakes

- Hardcoding ChromeDriver everywhere.
- Assuming a test passing in Chrome guarantees Firefox/Edge compatibility.
- Running parallel browser tests with shared static WebDriver.

---

## Module 15 - Selenium WebDriver - Finding Elements

### Deep Dive

Finding elements is the core Selenium skill. A locator should be unique, readable, stable, and close to how a user or business rule identifies the element.

### Locator Examples

```java
driver.findElement(By.id("userEmail")).sendKeys("qa@example.com");
driver.findElement(By.name("password")).sendKeys("Password123");
driver.findElement(By.className("login-btn")).click();
driver.findElement(By.linkText("Forgot password?")).click();
driver.findElement(By.partialLinkText("Forgot")).click();
driver.findElement(By.tagName("h1")).getText();
driver.findElement(By.cssSelector("button[type='submit']")).click();
driver.findElement(By.xpath("//button[text()='Login']")).click();
```

### `findElements` Example

```java
List<WebElement> links = driver.findElements(By.tagName("a"));
System.out.println("Total links: " + links.size());

for (WebElement link : links) {
    System.out.println(link.getText() + " -> " + link.getAttribute("href"));
}
```

### Scoped Search Example

```java
WebElement productCard = driver.findElement(By.xpath("//b[text()='ZARA COAT 3']/ancestor::div[contains(@class,'card-body')]"));
productCard.findElement(By.cssSelector("button:last-of-type")).click();
```

### Expected Result

Selenium identifies one or more elements and interacts with them correctly.

### Best Practices

- Use `findElement` when exactly one element is expected.
- Use `findElements` for lists, counts, and optional elements.
- Use scoped searches inside parent containers.
- Keep locators inside Page Objects.

### Common Mistakes

- Using `findElement` to check optional element existence.
- Using locators that match multiple elements.
- Copying absolute XPath from browser tools.

---

## Module 16 - Cascading Style Sheets CSS Selectors - Advanced Locators

### Deep Dive

CSS selectors are fast, readable, and ideal for many Selenium locators. They work well with IDs, classes, attributes, and hierarchy.

### CSS Selector Reference

| Selector | Example | Meaning |
|---|---|---|
| ID | `#userEmail` | Element with ID. |
| Class | `.btn-primary` | Element with class. |
| Attribute | `input[type='password']` | Element with attribute value. |
| Contains | `input[id*='Email']` | Attribute contains text. |
| Starts with | `input[id^='user']` | Attribute starts with text. |
| Ends with | `input[id$='Email']` | Attribute ends with text. |
| Child | `form button` | Button inside form. |
| Direct child | `form > button` | Button directly under form. |
| nth child | `table tr:nth-child(2)` | Second row. |

### Code Examples

```java
By email = By.cssSelector("#userEmail");
By password = By.cssSelector("input[type='password']");
By productCards = By.cssSelector("div.mb-3");
By addToCartButtons = By.cssSelector(".card-body button:last-of-type");
By toast = By.cssSelector("#toast-container .toast-message");
```

### Parent-Child Example

```java
WebElement card = driver.findElement(By.cssSelector("div.card-body"));
String productName = card.findElement(By.cssSelector("b")).getText();
```

### Expected Result

CSS selectors locate elements through IDs, classes, attributes, and hierarchy.

### Best Practices

- Prefer CSS when ID, class, or attribute selectors are stable.
- Keep selectors short and meaningful.
- Use scoped parent-child searches for repeated components.

### Common Mistakes

- Using generated classes that change every build.
- Overusing nth-child when text-based selection is more reliable.
- Building CSS selectors that depend too heavily on page layout.

---

## Module 17 - XPath - Advanced Locators

### Deep Dive

XPath is powerful for text-based matching and DOM relationship traversal. Use XPath when CSS cannot easily express the required relationship, such as finding a button next to a specific table cell or finding an input associated with a visible label.

### XPath Reference

| Pattern | Example |
|---|---|
| Attribute | `//input[@id='userEmail']` |
| Text | `//button[text()='Login']` |
| Contains text | `//button[contains(text(),'Log')]` |
| Starts with | `//input[starts-with(@id,'user')]` |
| Parent | `//label[text()='Email']/parent::div` |
| Ancestor | `//b[text()='ZARA COAT 3']/ancestor::div[contains(@class,'card-body')]` |
| Following sibling | `//td[text()='Brian']/following-sibling::td/button` |
| Preceding sibling | `//td[text()='Delete']/preceding-sibling::td` |

### Product-Specific Button Example

```java
By addToCartForProduct = By.xpath(
    "//b[text()='ZARA COAT 3']/ancestor::div[contains(@class,'card-body')]//button[contains(text(),'Add To Cart')]"
);
driver.findElement(addToCartForProduct).click();
```

### Table Row Example

```java
WebElement editButton = driver.findElement(By.xpath("//td[text()='Brian']/following-sibling::td/button[text()='Edit']"));
editButton.click();
```

### Expected Result

XPath locates elements based on text and relationships rather than fragile indexes.

### Best Practices

- Use relative XPath, not absolute XPath.
- Use text and stable attributes.
- Use axes when locating related elements.
- Keep XPath readable.

### Common Mistakes

- Using `/html/body/div[2]/div[1]/...` absolute XPath.
- Matching partial text too broadly.
- Using XPath when simple ID/CSS would work better.

---

## Module 18 - Selenium WebDriver - Working with WebElements

### Deep Dive

WebElement methods perform core user interactions and validations. A robust framework wraps repeated actions with wait-aware helper methods while still understanding raw WebElement operations.

### Common WebElement Methods

| Method | Purpose |
|---|---|
| `click()` | Click element. |
| `sendKeys()` | Type text or upload file path. |
| `clear()` | Clear input. |
| `getText()` | Read visible text. |
| `getAttribute()` | Read HTML attribute. |
| `isDisplayed()` | Visibility check. |
| `isEnabled()` | Enabled/disabled check. |
| `isSelected()` | Checkbox/radio selected check. |

### Input and Button Example

```java
WebElement email = driver.findElement(By.id("userEmail"));
email.clear();
email.sendKeys("qa@example.com");

driver.findElement(By.id("userPassword")).sendKeys("Password123");
driver.findElement(By.id("login")).click();
```

### Dropdown Example

```java
Select country = new Select(driver.findElement(By.id("country")));
country.selectByVisibleText("India");
Assert.assertEquals(country.getFirstSelectedOption().getText(), "India");
```

### Checkbox Example

```java
WebElement checkbox = driver.findElement(By.cssSelector("input[type='checkbox']"));
if (!checkbox.isSelected()) {
    checkbox.click();
}
Assert.assertTrue(checkbox.isSelected());
```

### Expected Result

The test enters data, clicks controls, validates dropdowns, and checks element states.

### Best Practices

- Clear fields before typing when appropriate.
- Use `Select` only for real `<select>` elements.
- Validate state before and after interaction.
- Use explicit waits before WebElement actions.

### Common Mistakes

- Using `Select` on custom dropdowns.
- Clicking hidden or disabled elements.
- Reading text before Ajax content loads.

---

## Module 19 - Selenium WebDriver - Useful Methods and Properties

### Deep Dive

WebDriver and WebElement expose methods that help with validation, browser management, page state, cookies, screenshots, and diagnostics.

### Browser Methods

```java
driver.get("https://example.com");
String title = driver.getTitle();
String url = driver.getCurrentUrl();
String source = driver.getPageSource();
driver.manage().window().maximize();
driver.manage().deleteAllCookies();
```

### Cookie Example

```java
driver.manage().addCookie(new Cookie("testMode", "true"));
Cookie cookie = driver.manage().getCookieNamed("testMode");
Assert.assertEquals(cookie.getValue(), "true");
```

### Broken Link Validation Example

```java
String href = driver.findElement(By.cssSelector("a.broken-link")).getAttribute("href");
HttpURLConnection connection = (HttpURLConnection) new URL(href).openConnection();
connection.setRequestMethod("HEAD");
connection.connect();
int statusCode = connection.getResponseCode();
Assert.assertTrue(statusCode < 400, "Broken link status: " + statusCode);
```

### Expected Result

The framework can validate page metadata, cookies, and link status codes.

### Best Practices

- Use HTTP checks for broken links rather than clicking every link.
- Delete cookies between tests when isolation is required.
- Use screenshots for failure evidence.

### Common Mistakes

- Validating page source instead of visible UI when user behavior matters.
- Forgetting that `close()` closes one window but `quit()` ends the full session.

---

## Module 20 - Selenium WebDriver - Wait Types

### Deep Dive

Waits are one of the most important Selenium topics. Flaky tests often come from poor synchronization. A good framework uses explicit waits for known conditions and avoids fixed sleeps.

### Wait Types

| Wait Type | Usage |
|---|---|
| Implicit wait | Global element lookup polling. Use carefully. |
| Explicit wait | Wait for a specific condition. Preferred. |
| FluentWait | Custom polling interval and ignored exceptions. |
| Static sleep | Fixed pause. Avoid unless debugging. |

### Explicit Wait Example

```java
WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
WebElement loginButton = wait.until(ExpectedConditions.elementToBeClickable(By.id("login")));
loginButton.click();
```

### Ajax Toast Example

```java
By toast = By.cssSelector("#toast-container");
wait.until(ExpectedConditions.visibilityOfElementLocated(toast));
Assert.assertTrue(driver.findElement(toast).getText().contains("Product Added"));
wait.until(ExpectedConditions.invisibilityOfElementLocated(toast));
```

### FluentWait Example

```java
Wait<WebDriver> fluentWait = new FluentWait<>(driver)
        .withTimeout(Duration.ofSeconds(20))
        .pollingEvery(Duration.ofMillis(500))
        .ignoring(NoSuchElementException.class)
        .ignoring(StaleElementReferenceException.class);

WebElement result = fluentWait.until(d -> d.findElement(By.id("result")));
```

### Expected Result

The test waits only as long as necessary and proceeds when the condition is true.

### Best Practices

- Prefer explicit waits.
- Wait for business-relevant states such as visibility, clickability, or invisibility of loader.
- Centralize waits in utility classes or abstract components.

### Common Mistakes

- Overusing implicit waits.
- Mixing long implicit waits with explicit waits without understanding side effects.
- Using `Thread.sleep()` in production test code.

---

## Module 21 - Selenium WebDriver – Advanced Interactions

### Deep Dive

Advanced web applications use dynamic UI patterns such as Ajax, scrollable tables, calendars, dynamic dropdowns, overlays, hover menus, and generated totals. These require more than basic click/type commands.

### JavaScript Scroll Example

```java
JavascriptExecutor js = (JavascriptExecutor) driver;
WebElement table = driver.findElement(By.cssSelector(".tableFixHead"));
js.executeScript("arguments[0].scrollTop = arguments[0].scrollHeight", table);
```

### Validate Table Total Example

```java
List<WebElement> amountCells = driver.findElements(By.cssSelector(".tableFixHead td:nth-child(4)"));
int calculatedTotal = amountCells.stream()
        .map(WebElement::getText)
        .mapToInt(Integer::parseInt)
        .sum();

String displayedText = driver.findElement(By.cssSelector(".totalAmount")).getText();
int displayedTotal = Integer.parseInt(displayedText.replaceAll("[^0-9]", ""));
Assert.assertEquals(calculatedTotal, displayedTotal);
```

### Calendar Date Selection Example

```java
String month = "June";
String day = "15";
driver.findElement(By.id("datepicker")).click();
while (!driver.findElement(By.cssSelector(".ui-datepicker-month")).getText().equals(month)) {
    driver.findElement(By.cssSelector(".ui-datepicker-next")).click();
}
driver.findElement(By.xpath("//a[text()='" + day + "']")).click();
```

### Expected Result

The test scrolls, validates numeric table totals, and selects a date dynamically.

### Best Practices

- Use JavaScriptExecutor only when normal WebDriver actions are insufficient.
- Parse table values carefully.
- Make calendar methods reusable.
- Wait for Ajax content before reading it.

### Common Mistakes

- Hardcoding row indexes.
- Not accounting for currency symbols or whitespace.
- Clicking calendar dates without verifying month/year.

---

## Module 22 - Selenium WebDriver - File Upload And Download

### Deep Dive

File upload and download testing validates browser-to-system interaction. Selenium can upload files directly when the web page uses an `<input type="file">`. Native OS dialogs are not controlled by Selenium directly.

### Upload Example

```java
Path uploadFile = Paths.get("src/test/resources/files/upload.xlsx").toAbsolutePath();
WebElement uploadInput = driver.findElement(By.cssSelector("input[type='file']"));
uploadInput.sendKeys(uploadFile.toString());
```

### Download Configuration Example

```java
Path downloadDir = Paths.get("downloads").toAbsolutePath();
Map<String, Object> prefs = new HashMap<>();
prefs.put("download.default_directory", downloadDir.toString());
prefs.put("download.prompt_for_download", false);
prefs.put("plugins.always_open_pdf_externally", true);

ChromeOptions options = new ChromeOptions();
options.setExperimentalOption("prefs", prefs);
WebDriver driver = new ChromeDriver(options);
```

### Download Validation Example

```java
Path downloadedFile = downloadDir.resolve("report.xlsx");
WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(20));
wait.until(d -> Files.exists(downloadedFile));
Assert.assertTrue(Files.size(downloadedFile) > 0);
```

### Expected Result

The file uploads through the web app, downloads into the configured folder, and is validated for existence and non-empty size.

### Best Practices

- Prefer `sendKeys()` to file input over native dialog automation.
- Use relative project paths.
- Clean download folders before tests.
- Validate file name and size.

### Common Mistakes

- Trying to automate OS file picker directly with Selenium.
- Hardcoding local machine paths.
- Not waiting for downloads to finish.

---

## Module 23 - Selenium WebDriver - Switch Window and iframes

### Deep Dive

Selenium always works in the currently selected browser context. When an app opens a new window/tab or places content inside an iframe, the test must switch context before interacting.

### Alert Example

```java
Alert alert = driver.switchTo().alert();
String alertText = alert.getText();
Assert.assertTrue(alertText.contains("Are you sure"));
alert.accept();
```

### Window Switch Example

```java
String parentWindow = driver.getWindowHandle();
driver.findElement(By.id("openwindow")).click();

Set<String> windows = driver.getWindowHandles();
for (String window : windows) {
    if (!window.equals(parentWindow)) {
        driver.switchTo().window(window);
        break;
    }
}

Assert.assertTrue(driver.getTitle().length() > 0);
driver.close();
driver.switchTo().window(parentWindow);
```

### Iframe Example

```java
driver.switchTo().frame("courses-iframe");
driver.findElement(By.linkText("Courses")).click();
driver.switchTo().defaultContent();
```

### Nested Frame Example

```java
driver.switchTo().frame("outerFrame");
driver.switchTo().frame("innerFrame");
driver.findElement(By.id("inside-frame-button")).click();
driver.switchTo().defaultContent();
```

### Expected Result

The test handles alerts, child windows, tabs, and iframes without losing browser focus.

### Best Practices

- Store the parent window handle before opening a child window.
- Switch back to default content after iframe work.
- Use explicit waits before switching to frames.

### Common Mistakes

- Trying to locate iframe elements before switching into the iframe.
- Closing a child window and forgetting to switch back.
- Assuming window handle order is always stable.

---

## Module 24 - Selenium WebDriver - Working with Actions Class

### Deep Dive

The `Actions` class is used for advanced user-like interactions that combine mouse and keyboard actions.

### Hover Example

```java
Actions actions = new Actions(driver);
WebElement menu = driver.findElement(By.id("mousehover"));
actions.moveToElement(menu).perform();
driver.findElement(By.linkText("Top")).click();
```

### Drag and Drop Example

```java
WebElement source = driver.findElement(By.id("draggable"));
WebElement target = driver.findElement(By.id("droppable"));
new Actions(driver).dragAndDrop(source, target).perform();
```

### Keyboard Example

```java
WebElement input = driver.findElement(By.id("search"));
new Actions(driver)
        .click(input)
        .keyDown(Keys.SHIFT)
        .sendKeys("selenium")
        .keyUp(Keys.SHIFT)
        .perform();
```

### Right Click Example

```java
WebElement element = driver.findElement(By.id("context-menu"));
new Actions(driver).contextClick(element).perform();
```

### Expected Result

Selenium performs hover, drag-and-drop, keyboard, right-click, and composite interactions.

### Best Practices

- Use Actions for realistic user interactions.
- Wait for hover menus to appear before clicking submenu items.
- Use JavaScript fallback only when WebDriver actions cannot work.

### Common Mistakes

- Forgetting `.perform()`.
- Using Actions for simple clicks unnecessarily.
- Not waiting for hover-triggered content.

---

## Module 25 - Logging Infrastructure

### Deep Dive

Logging helps explain what happened before a failure. This is especially important in Jenkins or remote cloud runs where developers cannot see the browser.

### Log4j2 Dependencies

```xml
<dependency>
    <groupId>org.apache.logging.log4j</groupId>
    <artifactId>log4j-api</artifactId>
    <version>2.23.1</version>
</dependency>
<dependency>
    <groupId>org.apache.logging.log4j</groupId>
    <artifactId>log4j-core</artifactId>
    <version>2.23.1</version>
</dependency>
```

### `log4j2.xml`

```xml
<Configuration status="WARN">
    <Appenders>
        <Console name="Console" target="SYSTEM_OUT">
            <PatternLayout pattern="%d{HH:mm:ss} %-5level %logger{36} - %msg%n"/>
        </Console>
        <File name="FileLogger" fileName="logs/test-execution.log">
            <PatternLayout pattern="%d{yyyy-MM-dd HH:mm:ss} %-5p %c - %m%n"/>
        </File>
    </Appenders>
    <Loggers>
        <Root level="info">
            <AppenderRef ref="Console"/>
            <AppenderRef ref="FileLogger"/>
        </Root>
    </Loggers>
</Configuration>
```

### Logger Usage

```java
private static final Logger logger = LogManager.getLogger(LoginTests.class);

logger.info("Starting login test");
logger.debug("Entering username");
logger.error("Dashboard was not displayed after login");
```

### Expected Result

Console and file logs show test progress, page actions, and failure context.

### Best Practices

- Log test start, important actions, and test end.
- Log errors with context.
- Archive logs in CI.
- Do not log passwords or tokens.

### Common Mistakes

- Logging too much noise.
- Logging secrets.
- Not saving logs as CI artifacts.

---

## Module 26 - TestNG Infrastructure

### Deep Dive

TestNG is a powerful test framework for Selenium Java. It supports lifecycle annotations, assertions, grouping, dependencies, parameters, data providers, listeners, reports, and parallel execution.

### Annotation Reference

| Annotation | Purpose |
|---|---|
| `@BeforeSuite` | Runs once before suite. |
| `@BeforeTest` | Runs before test block in XML. |
| `@BeforeClass` | Runs before class. |
| `@BeforeMethod` | Runs before each test method. |
| `@Test` | Test method. |
| `@AfterMethod` | Runs after each test method. |
| `@AfterClass` | Runs after class. |
| `@AfterSuite` | Runs after suite. |

### TestNG Example

```java
public class LoginTests extends BaseTest {
    @BeforeMethod(alwaysRun = true)
    public void openLoginPage() {
        driver.get(ConfigReader.get("baseUrl"));
    }

    @Test(groups = {"smoke", "login"}, priority = 1)
    public void validLoginTest() {
        Assert.assertTrue(true);
    }

    @Test(groups = {"login"}, dependsOnMethods = "validLoginTest")
    public void logoutTest() {
        Assert.assertTrue(true);
    }
}
```

### DataProvider Example

```java
@DataProvider(name = "loginData")
public Object[][] loginData() {
    return new Object[][] {
            {"valid@example.com", "Password123", true},
            {"bad@example.com", "wrong", false}
    };
}

@Test(dataProvider = "loginData")
public void loginTest(String email, String password, boolean expectedSuccess) {
    Assert.assertNotNull(email);
    Assert.assertNotNull(password);
}
```

### TestNG XML Example

```xml
<suite name="Regression Suite" parallel="tests" thread-count="2">
    <test name="Chrome Smoke Tests">
        <parameter name="browser" value="chrome"/>
        <groups>
            <run>
                <include name="smoke"/>
            </run>
        </groups>
        <classes>
            <class name="tests.LoginTests"/>
        </classes>
    </test>
</suite>
```

### Expected Result

TestNG controls execution order, grouping, data, and parallelism.

### Best Practices

- Use groups for smoke/regression/login/api.
- Use DataProvider for multiple data rows.
- Use listeners for screenshots/reports.
- Keep dependencies minimal; dependent tests can hide root failures.

### Common Mistakes

- Relying heavily on test priority.
- Sharing WebDriver across parallel tests.
- Putting setup code inside every test instead of annotations.

---

## Module 27 - JUnit/Pytest Equivalents for Java

### Deep Dive

The referenced course includes Python `unittest` and `pytest`. In Java, common equivalents are TestNG and JUnit 5. TestNG is popular in Selenium QA frameworks because of XML suites, groups, DataProvider, and listeners. JUnit 5 is common in Java development teams and integrates well with build systems and Spring projects.

### JUnit 5 Example

```java
public class JUnitLoginTest {
    WebDriver driver;

    @BeforeEach
    void setup() {
        driver = new ChromeDriver();
    }

    @Test
    void titleTest() {
        driver.get("https://example.com");
        Assertions.assertEquals("Example Domain", driver.getTitle());
    }

    @AfterEach
    void teardown() {
        driver.quit();
    }
}
```

### TestNG vs JUnit

| Feature | TestNG | JUnit 5 |
|---|---|---|
| XML suite control | Strong | Less central |
| Groups/tags | Groups | Tags |
| Data-driven tests | DataProvider | Parameterized tests |
| Selenium enterprise use | Very common | Common |
| Spring/Dev unit tests | Common | Very common |

### Expected Result

Java tests can be organized with either TestNG or JUnit depending on team preference.

### Best Practices

- Use TestNG for Selenium framework-heavy suites.
- Use JUnit 5 when aligned with development team standards.
- Do not mix both frameworks in the same test layer unless necessary.

---

## Module 28 - Automation Framework - Part 1

### Deep Dive

Framework Part 1 starts moving from scripts to architecture. It usually includes Maven setup, dependencies, first ecommerce test, product selection, waits, cart validation, and checkout flow.

### First Framework Test Flow

1. Launch browser.
2. Open app URL.
3. Login.
4. Wait for product catalogue.
5. Find product by name.
6. Add product to cart.
7. Validate cart.
8. Checkout.
9. Validate confirmation.
10. Close browser.

### Product Selection Example

```java
List<WebElement> products = driver.findElements(By.cssSelector(".mb-3"));
WebElement targetProduct = products.stream()
        .filter(product -> product.findElement(By.cssSelector("b")).getText().equals("ZARA COAT 3"))
        .findFirst()
        .orElseThrow(() -> new RuntimeException("Product not found"));

targetProduct.findElement(By.cssSelector("button:last-of-type")).click();
```

### Wait for Toast Example

```java
By toast = By.cssSelector("#toast-container");
wait.until(ExpectedConditions.visibilityOfElementLocated(toast));
wait.until(ExpectedConditions.invisibilityOfElementLocated(toast));
```

### Expected Result

The test adds the correct product to cart and proceeds only after UI feedback is complete.

### Best Practices

- Build the flow first, then refactor into page objects.
- Use explicit waits around Ajax events.
- Avoid index-based product selection.
- Keep product names in test data.

### Common Mistakes

- Refactoring too early before flow is understood.
- Ignoring loaders/toasts.
- Hardcoding product button indexes.

---

## Module 29 - Automation Framework - Part 2

### Deep Dive

Framework Part 2 introduces Page Object Model and PageFactory. The test should no longer directly manage every locator. Instead, each page exposes business-level methods.

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

    @FindBy(css = ".toast-message")
    WebElement errorMessage;

    public LandingPage(WebDriver driver) {
        super(driver);
        this.driver = driver;
        PageFactory.initElements(driver, this);
    }

    public void goTo() {
        driver.get(ConfigReader.get("baseUrl"));
    }

    public ProductCataloguePage loginApplication(String email, String pwd) {
        userEmail.sendKeys(email);
        password.sendKeys(pwd);
        loginButton.click();
        return new ProductCataloguePage(driver);
    }

    public String getErrorMessage() {
        return errorMessage.getText();
    }
}
```

### Product Page Example

```java
public class ProductCataloguePage extends AbstractComponent {
    @FindBy(css = ".mb-3")
    List<WebElement> products;

    By productsBy = By.cssSelector(".mb-3");
    By addToCart = By.cssSelector("button:last-of-type");

    public ProductCataloguePage(WebDriver driver) {
        super(driver);
        PageFactory.initElements(driver, this);
    }

    public WebElement getProductByName(String productName) {
        waitForElementToAppear(productsBy);
        return products.stream()
                .filter(product -> product.findElement(By.cssSelector("b")).getText().equals(productName))
                .findFirst()
                .orElseThrow();
    }

    public void addProductToCart(String productName) {
        getProductByName(productName).findElement(addToCart).click();
    }
}
```

### Expected Result

Tests become readable and page-specific locator changes are isolated to page classes.

### Best Practices

- Keep locators private or page-scoped.
- Keep methods business-readable.
- Return page objects after navigation.
- Use abstract components for shared header/cart/wait behavior.

### Common Mistakes

- Returning WebElements to tests unnecessarily.
- Creating page objects inside every small method.
- Putting assertions into every page method.

---

## Module 30 - Automation Framework - Part 3

### Deep Dive

Framework Part 3 adds BaseTest, global properties, driver initialization, TestNG grouping, error validation tests, dependencies, and parallel execution.

### BaseTest Example

```java
public class BaseTest {
    public WebDriver driver;
    public LandingPage landingPage;

    public WebDriver initializeDriver() throws IOException {
        String browserName = ConfigReader.get("browser");
        boolean headless = Boolean.parseBoolean(ConfigReader.get("headless"));
        driver = DriverFactory.createDriver(browserName, headless);
        driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(5));
        driver.manage().window().maximize();
        return driver;
    }

    @BeforeMethod(alwaysRun = true)
    public void launchApplication() throws IOException {
        driver = initializeDriver();
        landingPage = new LandingPage(driver);
        landingPage.goTo();
    }

    @AfterMethod(alwaysRun = true)
    public void tearDown() {
        if (driver != null) driver.quit();
    }
}
```

### Error Validation Test

```java
@Test(groups = {"login", "negative"})
public void loginErrorValidation() {
    landingPage.loginApplication("wrong@example.com", "wrongPassword");
    Assert.assertEquals(landingPage.getErrorMessage(), "Incorrect email or password.");
}
```

### Expected Result

Each test receives a fresh browser, opens the application, runs its scenario, and closes the browser.

### Best Practices

- Use `@BeforeMethod` for independent UI tests.
- Use `alwaysRun=true` for setup/teardown in grouped execution.
- Keep global settings in properties files.
- Support Maven overrides with `System.getProperty()`.

### Common Mistakes

- Static shared driver in parallel tests.
- Missing teardown when tests fail.
- Not separating positive and negative tests.

---

## Module 31 - Automation Framework Practice Exercise

### Deep Dive

The practice exercise validates whether the framework can support a real workflow with login, product selection, cart validation, checkout, country selection, and confirmation.

### End-to-End Test Example

```java
@Test(groups = {"regression", "order"})
public void submitOrderTest() {
    String productName = "ZARA COAT 3";

    ProductCataloguePage productCatalogue = landingPage.loginApplication("user@example.com", "Password123");
    productCatalogue.addProductToCart(productName);

    CartPage cartPage = productCatalogue.goToCartPage();
    Assert.assertTrue(cartPage.verifyProductDisplay(productName));

    CheckoutPage checkoutPage = cartPage.goToCheckout();
    checkoutPage.selectCountry("India");

    ConfirmationPage confirmationPage = checkoutPage.submitOrder();
    Assert.assertEquals(confirmationPage.getConfirmationMessage(), "THANKYOU FOR THE ORDER.");
}
```

### Cart Page Example

```java
public class CartPage extends AbstractComponent {
    @FindBy(css = ".cartSection h3")
    List<WebElement> cartProducts;

    public CartPage(WebDriver driver) {
        super(driver);
        PageFactory.initElements(driver, this);
    }

    public boolean verifyProductDisplay(String productName) {
        return cartProducts.stream().anyMatch(product -> product.getText().equalsIgnoreCase(productName));
    }
}
```

### Expected Result

The test validates a full purchase/order flow using Page Objects and reusable methods.

### Best Practices

- Keep test data at the top of the test or in data files.
- Validate each major page transition.
- Use page methods to express business flow.
- Keep checkout and cart assertions explicit.

---

## Module 32 - Data-Driven Testing

### Deep Dive

Data-driven testing lets the same test logic run with multiple users, products, roles, or expected outcomes. This reduces duplication and expands coverage.

### DataProvider with HashMap

```java
@DataProvider
public Object[][] getData() {
    HashMap<String, String> user1 = new HashMap<>();
    user1.put("email", "user1@example.com");
    user1.put("password", "Password123");
    user1.put("product", "ZARA COAT 3");

    HashMap<String, String> user2 = new HashMap<>();
    user2.put("email", "user2@example.com");
    user2.put("password", "Password123");
    user2.put("product", "ADIDAS ORIGINAL");

    return new Object[][] {{user1}, {user2}};
}

@Test(dataProvider = "getData")
public void submitOrder(HashMap<String, String> input) {
    ProductCataloguePage productCatalogue = landingPage.loginApplication(input.get("email"), input.get("password"));
    productCatalogue.addProductToCart(input.get("product"));
}
```

### JSON Reader Concept

```java
public List<HashMap<String, String>> getJsonDataToMap(String filePath) throws IOException {
    String jsonContent = FileUtils.readFileToString(new File(filePath), StandardCharsets.UTF_8);
    ObjectMapper mapper = new ObjectMapper();
    return mapper.readValue(jsonContent, new TypeReference<List<HashMap<String, String>>>(){});
}
```

### Excel Use Cases

- Login credentials.
- Search terms.
- Product names.
- Expected prices.
- Role-based user data.

### Expected Result

The same test executes multiple times with different data rows.

### Best Practices

- Use JSON for structured data.
- Use Excel when business users maintain data.
- Keep sensitive data out of committed files.
- Avoid huge DataProviders that make failures hard to diagnose.

---

## Module 33 - Running Complete Test Suite

### Deep Dive

A complete framework should support running selected tests from the IDE, Maven terminal, TestNG XML, Jenkins, and CI/CD pipelines.

### Common Commands

```bash
mvn clean test
mvn clean test -Dbrowser=chrome
mvn clean test -Dbrowser=firefox -Dheadless=true
mvn clean test -DsuiteXmlFile=testng.xml
mvn clean test -Dgroups=smoke
```

### TestNG XML Example

```xml
<suite name="Complete Regression Suite" parallel="tests" thread-count="3">
    <test name="Chrome Smoke">
        <parameter name="browser" value="chrome"/>
        <groups>
            <run><include name="smoke"/></run>
        </groups>
        <packages>
            <package name="tests"/>
        </packages>
    </test>
</suite>
```

### Expected Result

Maven executes selected test suites and produces Surefire/TestNG reports.

### Best Practices

- Keep separate XML files for smoke and regression.
- Run smoke on every commit.
- Run regression nightly or before release.
- Archive reports and screenshots.

### Common Mistakes

- Running only from IDE.
- Not testing Maven execution before Jenkins setup.
- Not grouping tests logically.

---

## Module 34 - Git and GitHub - Version Control System

### Deep Dive

GitHub stores framework source code and enables team collaboration, history, pull requests, and CI/CD integration.

### Commands

```bash
git config --global user.name "Brian McCarthy"
git config --global user.email "briansmc@gmail.com"
git init
git status
git add .
git commit -m "Add Selenium framework"
git remote add origin https://github.com/BrianGator/Selenium-Automation-Advanced-Frameworks-Java-Showcase.git
git push -u origin master
```

### Branch Workflow

```bash
git checkout -b feature/login-tests
git add .
git commit -m "Add login tests"
git checkout master
git merge feature/login-tests
git push
```

### `.gitignore` Example

```gitignore
target/
reports/
screenshots/
logs/
downloads/
*.class
.idea/
.env
```

### Expected Result

The framework is versioned, shareable, and ready for CI/CD integration.

### Best Practices

- Commit source, not generated files.
- Use branches for new features.
- Write meaningful commit messages.
- Protect main/master branch in team projects.

---

## Module 35 - Continuous Integration with Jenkins

### Deep Dive

Jenkins automates test execution after code changes, on pull requests, on schedules, or before deployments. CI/CD turns Selenium from a local tool into a quality gate.

### Jenkins Pipeline

```groovy
pipeline {
    agent any
    tools {
        maven 'Maven-3.9'
        jdk 'JDK-17'
    }
    parameters {
        choice(name: 'BROWSER', choices: ['chrome', 'firefox', 'edge'], description: 'Browser to run tests')
        booleanParam(name: 'HEADLESS', defaultValue: true, description: 'Run browser in headless mode')
    }
    stages {
        stage('Checkout') {
            steps { git 'https://github.com/BrianGator/Selenium-Automation-Advanced-Frameworks-Java-Showcase.git' }
        }
        stage('Run Tests') {
            steps { sh "mvn clean test -Dbrowser=${params.BROWSER} -Dheadless=${params.HEADLESS}" }
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

### CI/CD Execution Strategy

| Build Type | Tests to Run |
|---|---|
| Pull request | Smoke tests. |
| Main branch commit | Smoke + key regression. |
| Nightly build | Full regression, cross-browser. |
| Release candidate | Full regression + Grid/cloud + API checks. |

### Expected Result

Jenkins checks out the project, runs Maven tests, publishes JUnit results, and archives logs/screenshots/reports.

### Best Practices

- Use Jenkins credentials for secrets.
- Archive failure evidence.
- Run headless in CI unless visual debugging is needed.
- Use parameters for browser/environment.

### Common Mistakes

- Hardcoding credentials in Jenkinsfile.
- Not archiving screenshots.
- Running long full regression on every small commit.

---

## Module 36 - Conclusion

### Deep Dive

A mature Selenium Java framework should support local execution, CI execution, clean reporting, stable locators, reusable page objects, explicit waits, data-driven tests, API setup, login coverage, and cross-browser strategy.

### Framework Maturity Roadmap

| Level | Capabilities |
|---|---|
| Beginner | Simple scripts, direct locators, basic assertions. |
| Intermediate | TestNG, Maven, Page Objects, explicit waits. |
| Advanced | Data-driven tests, listeners, screenshots, reports, CI/CD. |
| Enterprise | ThreadLocal parallelism, Grid/cloud, API setup, DB validation, BDD, CDP, reporting dashboards. |

### Recommended Next Steps

- Add Selenium Grid execution.
- Add BrowserStack/Sauce Labs cloud runs.
- Add Rest Assured API setup/cleanup.
- Add JDBC validations.
- Add ExtentReports or Allure.
- Add Cucumber BDD wrapper.
- Add Dockerized execution.
- Add GitHub Actions in addition to Jenkins.

---

## Supplemental Module 37 - Selenium Java Streams for Web Tables

### Deep Dive

Java Streams make table validation more readable. They are useful for sorting, filtering, mapping WebElements to text, and validating pagination.

### Sort Validation

```java
List<String> originalList = driver.findElements(By.xpath("//tr/td[1]")).stream()
        .map(WebElement::getText)
        .collect(Collectors.toList());

driver.findElement(By.cssSelector("tr th:nth-child(1)")).click();

List<String> sortedFromUi = driver.findElements(By.xpath("//tr/td[1]")).stream()
        .map(WebElement::getText)
        .collect(Collectors.toList());

List<String> sortedExpected = originalList.stream().sorted().collect(Collectors.toList());
Assert.assertEquals(sortedFromUi, sortedExpected);
```

### Filter Table Example

```java
List<String> price = driver.findElements(By.xpath("//tr/td[1]")).stream()
        .filter(s -> s.getText().contains("Rice"))
        .map(s -> s.findElement(By.xpath("following-sibling::td[1]")).getText())
        .collect(Collectors.toList());

Assert.assertTrue(price.size() > 0);
```

### Pagination Example

```java
List<String> names;
do {
    names = driver.findElements(By.xpath("//tr/td[1]")).stream()
            .filter(s -> s.getText().contains("Rice"))
            .map(WebElement::getText)
            .collect(Collectors.toList());
    if (names.size() < 1) {
        driver.findElement(By.cssSelector("[aria-label='Next']")).click();
    }
} while (names.size() < 1);
```

### Expected Result

The framework validates sort order, filters table values, and searches paginated tables using Java Streams.

---

## Supplemental Module 38 - Selenium 4.0 Latest Features

### Deep Dive

Selenium 4 added features such as relative locators, improved window/tab APIs, element screenshots, better Grid architecture, and CDP integration.

### Relative Locator Example

```java
WebElement label = driver.findElement(By.xpath("//label[text()='Email']"));
WebElement input = driver.findElement(RelativeLocator.with(By.tagName("input")).below(label));
input.sendKeys("qa@example.com");
```

### New Tab Example

```java
driver.switchTo().newWindow(WindowType.TAB);
driver.get("https://example.com");
Assert.assertEquals(driver.getTitle(), "Example Domain");
```

### Element Screenshot Example

```java
WebElement logo = driver.findElement(By.cssSelector("img.logo"));
File logoFile = logo.getScreenshotAs(OutputType.FILE);
FileUtils.copyFile(logoFile, new File("screenshots/logo.png"));
```

### Element Dimension Example

```java
Dimension size = driver.findElement(By.cssSelector("img.logo")).getSize();
Assert.assertTrue(size.getHeight() > 0);
Assert.assertTrue(size.getWidth() > 0);
```

### Expected Result

Selenium 4 features improve readability, tab/window handling, visual evidence, and element-level validation.

---

## Supplemental Module 39 - Framework Part 4 Test Strategy and Parallel Control

### Deep Dive

A framework needs a clear test strategy. Not every test should run all the time. Tests should be grouped by purpose and parallelized safely.

### Recommended Test Groups

| Group | Purpose |
|---|---|
| `smoke` | Critical high-confidence checks. |
| `regression` | Broad functional coverage. |
| `login` | Authentication checks. |
| `api` | Backend/service checks. |
| `negative` | Error handling validation. |
| `e2e` | Full user journeys. |

### Screenshot Utility

```java
public String getScreenshot(String testCaseName, WebDriver driver) throws IOException {
    File source = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
    String path = System.getProperty("user.dir") + "/reports/" + testCaseName + ".png";
    FileUtils.copyFile(source, new File(path));
    return path;
}
```

### Parallel XML Example

```xml
<suite name="Parallel Suite" parallel="classes" thread-count="3">
    <test name="Regression Tests">
        <classes>
            <class name="tests.SubmitOrderTest"/>
            <class name="tests.ErrorValidationTest"/>
            <class name="tests.LoginTest"/>
        </classes>
    </test>
</suite>
```

### Expected Result

Tests run in meaningful groups and parallel-safe structure reduces runtime.

---

## Supplemental Module 40 - Framework Part 5 Extent Reports, Listeners, ThreadLocal and Retry

### Deep Dive

Reporting and listeners provide professional execution evidence. ThreadLocal enables safe parallel execution by giving every test thread its own WebDriver.

### ThreadLocal Driver Manager

```java
public class DriverManager {
    private static ThreadLocal<WebDriver> driver = new ThreadLocal<>();

    public static WebDriver getDriver() {
        return driver.get();
    }

    public static void setDriver(WebDriver webDriver) {
        driver.set(webDriver);
    }

    public static void unload() {
        driver.remove();
    }
}
```

### Retry Analyzer

```java
public class RetryAnalyzer implements IRetryAnalyzer {
    private int count = 0;
    private static final int maxTry = 1;

    @Override
    public boolean retry(ITestResult result) {
        if (count < maxTry) {
            count++;
            return true;
        }
        return false;
    }
}
```

### Listener Example

```java
public class TestListener implements ITestListener {
    @Override
    public void onTestFailure(ITestResult result) {
        System.out.println("FAILED: " + result.getName());
    }

    @Override
    public void onTestSuccess(ITestResult result) {
        System.out.println("PASSED: " + result.getName());
    }
}
```

### Expected Result

Parallel tests do not overwrite each other’s drivers, and failures are logged with evidence.

---

## Supplemental Module 41 - Framework Part 6 Maven and Jenkins CI/CD

### Deep Dive

Maven and Jenkins should allow test execution by environment, browser, group, headless mode, and suite file without code changes.

### Runtime Commands

```bash
mvn clean test -Dbrowser=chrome -Dheadless=true
mvn clean test -Dbrowser=firefox -Dgroups=smoke
mvn clean test -Denv=qa -DsuiteXmlFile=testng.xml
mvn clean test -DbaseUrl=https://qa.example.com
```

### Jenkins Parameter Ideas

| Parameter | Example |
|---|---|
| `BROWSER` | chrome/firefox/edge |
| `ENV` | dev/qa/stage/prod-smoke |
| `HEADLESS` | true/false |
| `GROUPS` | smoke/regression/login |
| `SUITE_XML` | testng.xml/testng-smoke.xml |

### Expected Result

CI/CD can run the same framework across multiple environments and browsers using parameters.

---

## Supplemental Module 42 - Framework Part 7 Cucumber BDD Wrapper

### Deep Dive

Cucumber wraps Selenium tests in business-readable Gherkin syntax. It is useful when BAs, product owners, or nontechnical stakeholders need readable acceptance scenarios.

### Feature File

```gherkin
Feature: Order submission

  Background:
    Given the user opens the ecommerce application

  @smoke @order
  Scenario: Submit order for one product
    When the user logs in with email "user@example.com" and password "Password123"
    And the user adds product "ZARA COAT 3" to the cart
    And the user submits the order for country "India"
    Then the order confirmation message should be "THANKYOU FOR THE ORDER."
```

### Step Definition

```java
@When("the user logs in with email {string} and password {string}")
public void login(String email, String password) {
    productCataloguePage = landingPage.loginApplication(email, password);
}

@When("the user adds product {string} to the cart")
public void addProduct(String productName) {
    productCataloguePage.addProductToCart(productName);
}

@Then("the order confirmation message should be {string}")
public void verifyConfirmation(String expectedMessage) {
    Assert.assertEquals(confirmationPage.getConfirmationMessage(), expectedMessage);
}
```

### Expected Result

Readable Gherkin scenarios execute Selenium Page Object methods.

### Best Practices

- Keep step definitions thin.
- Reuse Page Objects.
- Use tags for smoke/regression.
- Avoid writing overly technical Gherkin.

---

## Supplemental Module 43 - Cross Browser Testing with Selenium Grid and Cloud

### Deep Dive

Selenium Grid and cloud providers allow tests to run on remote browsers and multiple platforms. This is useful for parallel execution and browser coverage.

### RemoteWebDriver Example

```java
ChromeOptions options = new ChromeOptions();
WebDriver driver = new RemoteWebDriver(new URL("http://localhost:4444/wd/hub"), options);
driver.get("https://example.com");
Assert.assertEquals(driver.getTitle(), "Example Domain");
driver.quit();
```

### Cloud Capabilities Concept

```java
MutableCapabilities capabilities = new MutableCapabilities();
capabilities.setCapability("browserName", "Chrome");
capabilities.setCapability("browserVersion", "latest");
capabilities.setCapability("platformName", "Windows 11");

WebDriver driver = new RemoteWebDriver(new URL("https://USERNAME:ACCESS_KEY@hub.browserstack.com/wd/hub"), capabilities);
```

### When Grid/Cloud Is Needed

- Need many browser/OS combinations.
- Need parallel execution beyond local machine limits.
- Need Safari/Windows/Linux coverage.
- Need screenshots/videos/logs from remote sessions.

### Expected Result

Tests execute on remote infrastructure instead of local browsers.

---

## Supplemental Module 44 - Selenium 4 Chrome DevTools Protocol CDP

### Deep Dive

Chrome DevTools Protocol lets Selenium interact with browser internals such as network requests, geolocation, device emulation, performance throttling, console logs, and authentication.

### Network Blocking Example

```java
ChromeDriver driver = new ChromeDriver();
DevTools devTools = driver.getDevTools();
devTools.createSession();
devTools.send(Network.enable(Optional.empty(), Optional.empty(), Optional.empty()));
devTools.send(Network.setBlockedURLs(List.of("*.jpg", "*.png", "*.css")));
driver.get("https://example.com");
```

### Device Emulation Example

```java
Map<String, Object> deviceMetrics = new HashMap<>();
deviceMetrics.put("width", 390);
deviceMetrics.put("height", 844);
deviceMetrics.put("deviceScaleFactor", 3);
deviceMetrics.put("mobile", true);

driver.executeCdpCommand("Emulation.setDeviceMetricsOverride", deviceMetrics);
driver.get("https://example.com");
```

### Console Error Capture Concept

```java
driver.manage().logs().get("browser").forEach(logEntry -> {
    if (logEntry.getLevel().getName().equals("SEVERE")) {
        System.out.println("Browser error: " + logEntry.getMessage());
    }
});
```

### Expected Result

The test can block network calls, emulate mobile devices, inspect status codes, and capture browser-side issues.

---

## Supplemental Module 45 - Database Connection to Selenium Testcases

### Deep Dive

Database validation confirms backend state after UI or API operations. It is useful for order status, user creation, inventory updates, audit records, and cleanup.

### JDBC Dependency

```xml
<dependency>
    <groupId>com.mysql</groupId>
    <artifactId>mysql-connector-j</artifactId>
    <version>8.4.0</version>
</dependency>
```

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

### UI-to-DB Validation Use Case

1. Submit an order in UI.
2. Capture order ID from confirmation page.
3. Query database for the order ID.
4. Assert DB status equals expected status.
5. Clean up test record if needed.

### Expected Result

The test validates that UI action created correct backend database state.

---

## Supplemental Module 46 - File Uploading AutoIT and Downloading with Selenium

### Deep Dive

Selenium cannot directly control OS-level dialogs. For web apps with real file inputs, use `sendKeys`. If the app uses native dialogs or Windows authentication popups, tools like AutoIT may be used, though test design should prefer browser-controllable paths.

### Basic Authentication URL Example

```java
driver.get("https://username:password@the-internet.herokuapp.com/basic_auth");
```

### Preferred Upload Method

```java
driver.findElement(By.cssSelector("input[type='file']"))
        .sendKeys(Paths.get("src/test/resources/file.pdf").toAbsolutePath().toString());
```

### Download Validation

```java
Path file = Paths.get("downloads", "report.pdf");
new WebDriverWait(driver, Duration.ofSeconds(20)).until(d -> Files.exists(file));
Assert.assertTrue(Files.size(file) > 0);
```

### Expected Result

Authentication and upload/download workflows are handled with stable Selenium-compatible methods where possible.

---

## API Tests for Selenium Java Frameworks

### Deep Dive

API tests are faster than UI tests and help create preconditions, validate backend behavior, authenticate users, and clean up data. A strong Selenium framework uses API helpers to reduce brittle UI setup.

### Rest Assured Dependency

```xml
<dependency>
    <groupId>io.rest-assured</groupId>
    <artifactId>rest-assured</artifactId>
    <version>5.4.0</version>
    <scope>test</scope>
</dependency>
```

### GET Example

```java
@Test(groups = {"api"})
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

### POST Setup Example

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

### DELETE Cleanup Example

```java
given()
    .baseUri("https://api.example.com")
    .header("Authorization", "Bearer token")
.when()
    .delete("/orders/" + orderId)
.then()
    .statusCode(anyOf(equalTo(200), equalTo(202), equalTo(204)));
```

### API Test Checklist

| Area | Validation |
|---|---|
| Status code | 200, 201, 204, 400, 401, 403, 404, 409, 422. |
| Body | Required fields, values, types. |
| Headers | Auth, content type, correlation ID. |
| Negative tests | Missing fields, bad IDs, invalid token. |
| Cleanup | Delete generated records. |

### Expected Result

API tests validate backend behavior and support cleaner UI test setup.

---

## Login Tests for Selenium Java Frameworks

### Deep Dive

Login tests validate authentication, session behavior, error handling, and authorization. Because login is a gateway workflow, it should include both positive and negative coverage.

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
        driver.findElement(email).clear();
        driver.findElement(email).sendKeys(userEmail);
        driver.findElement(password).clear();
        driver.findElement(password).sendKeys(userPassword);
        driver.findElement(loginButton).click();
        return new ProductCataloguePage(driver);
    }

    public String getErrorMessage() {
        return driver.findElement(errorMessage).getText();
    }
}
```

### Valid Login Test

```java
@Test(groups = {"smoke", "login"})
public void validLoginTest() {
    ProductCataloguePage page = landingPage.loginApplication(System.getenv("TEST_USER_EMAIL"), System.getenv("TEST_USER_PASSWORD"));
    Assert.assertTrue(page.isProductCatalogueDisplayed());
}
```

### Invalid Login Test

```java
@Test(groups = {"login", "negative"})
public void invalidLoginTest() {
    landingPage.loginApplication("bad@example.com", "wrong-password");
    Assert.assertEquals(landingPage.getErrorMessage(), "Incorrect email or password.");
}
```

### Login Coverage Matrix

| Scenario | Expected Result |
|---|---|
| Valid login | User reaches product catalogue/dashboard. |
| Invalid password | Error message appears. |
| Invalid username | Error message appears. |
| Empty username/password | Required field validation appears. |
| Locked user | Locked account message appears. |
| Logout | User returns to login screen. |
| Expired session | User is redirected to login. |
| Role-based login | User sees role-specific menu/features. |

### Best Practices

- Keep only a few UI login tests; use API/session setup for the rest if possible.
- Use environment variables for credentials.
- Never commit real passwords.
- Test authorization separately from authentication.

---

## Locator Reference Guide

### Locator Priority

| Priority | Locator | Example | Notes |
|---:|---|---|---|
| 1 | ID | `By.id("userEmail")` | Best when stable and unique. |
| 2 | Test attribute | `By.cssSelector("[data-testid='login']")` | Excellent for automation. |
| 3 | Name | `By.name("email")` | Good for forms. |
| 4 | CSS | `By.cssSelector("button[type='submit']")` | Fast and readable. |
| 5 | XPath | `By.xpath("//button[text()='Login']")` | Good for text/relationships. |
| 6 | Link text | `By.linkText("Forgot Password?")` | Good for exact links. |
| 7 | Class name | `By.className("btn-primary")` | Often not unique. |
| 8 | Tag name | `By.tagName("a")` | Useful for lists/counts. |

### Locator Anti-Patterns

- Absolute XPath.
- Generated dynamic class names.
- Index-heavy locators.
- Locators that match many elements accidentally.
- Locators based only on styling.
- Locators stored directly in test methods.

### Robust Locator Examples

```java
By loginButton = By.cssSelector("button[type='submit']");
By productCard = By.xpath("//b[text()='ZARA COAT 3']/ancestor::div[contains(@class,'card-body')]");
By checkoutButton = By.cssSelector("button.checkout");
By errorToast = By.cssSelector("#toast-container .toast-message");
```

---

## Building a Selenium Java Framework from Scratch

### Deep Dive

A custom framework is justified when repeated test complexity requires reusable architecture. A complete Selenium Java framework includes test setup, driver factory, configuration, page objects, reusable waits, test data, logging, reporting, screenshots, listeners, API helpers, CI/CD, and parallel execution support.

### Required Files and Folders

```text
selenium-java-framework/
├── pom.xml
├── testng.xml
├── Jenkinsfile
├── README.md
├── .gitignore
├── src/test/java/base/BaseTest.java
├── src/test/java/factory/DriverFactory.java
├── src/test/java/components/AbstractComponent.java
├── src/test/java/pages/LandingPage.java
├── src/test/java/pages/ProductCataloguePage.java
├── src/test/java/pages/CartPage.java
├── src/test/java/pages/CheckoutPage.java
├── src/test/java/pages/ConfirmationPage.java
├── src/test/java/tests/SubmitOrderTest.java
├── src/test/java/tests/ErrorValidationTest.java
├── src/test/java/tests/LoginTest.java
├── src/test/java/api/ApiClient.java
├── src/test/java/listeners/TestListener.java
├── src/test/java/retry/RetryAnalyzer.java
├── src/test/java/utils/ConfigReader.java
├── src/test/java/utils/ElementUtils.java
├── src/test/java/utils/ExcelUtils.java
├── src/test/java/utils/JsonUtils.java
├── src/test/java/utils/ScreenshotUtils.java
├── src/test/resources/GlobalData.properties
├── src/test/resources/log4j2.xml
├── src/test/resources/testdata/orders.json
├── src/test/resources/testdata/login-data.xlsx
├── reports/
├── screenshots/
├── logs/
└── downloads/
```

### Framework Build Steps

1. Create Maven project.
2. Add dependencies.
3. Create `GlobalData.properties`.
4. Build `ConfigReader`.
5. Build `DriverFactory`.
6. Build `BaseTest`.
7. Build `AbstractComponent`.
8. Build Page Objects.
9. Build test classes.
10. Add DataProvider support.
11. Add JSON/Excel data utilities.
12. Add listeners and screenshots.
13. Add reports.
14. Add retry analyzer.
15. Add ThreadLocal for parallel execution.
16. Add API helper for setup/cleanup.
17. Add Jenkinsfile.
18. Add GitHub repository and CI hooks.

### DriverFactory Example

```java
public class DriverFactory {
    public static WebDriver createDriver(String browser, boolean headless) {
        if (browser.equalsIgnoreCase("firefox")) {
            FirefoxOptions options = new FirefoxOptions();
            if (headless) options.addArguments("--headless");
            return new FirefoxDriver(options);
        }
        ChromeOptions options = new ChromeOptions();
        if (headless) options.addArguments("--headless=new");
        options.addArguments("--window-size=1920,1080");
        return new ChromeDriver(options);
    }
}
```

### BaseTest Example

```java
public class BaseTest {
    protected WebDriver driver;
    protected LandingPage landingPage;

    @BeforeMethod(alwaysRun = true)
    public void launchApplication() {
        driver = DriverFactory.createDriver(ConfigReader.get("browser"), Boolean.parseBoolean(ConfigReader.get("headless")));
        landingPage = new LandingPage(driver);
        landingPage.goTo();
    }

    @AfterMethod(alwaysRun = true)
    public void tearDown() {
        if (driver != null) driver.quit();
    }
}
```

### Best Practices

- Keep tests readable and business-focused.
- Keep locators in Page Objects.
- Keep waits reusable.
- Use API setup/cleanup.
- Use screenshots and logs on failure.
- Use TestNG groups.
- Run smoke tests in CI.
- Use ThreadLocal for parallel execution.

---

## Build from Scratch vs Pre-Built Frameworks

### When to Build From Scratch

| Scenario | Why Custom Helps |
|---|---|
| Large enterprise app | Needs custom architecture, test data, reporting, and roles. |
| Complex workflows | Needs reusable pages, API setup, DB validation, and cleanup. |
| Multi-QA team | Needs standards and shared utilities. |
| Parallel execution | Needs ThreadLocal and safe lifecycle. |
| CI/CD quality gate | Needs reports, logs, screenshots, and parameters. |

### When to Use Pre-Built or Simpler Frameworks

| Scenario | Recommended Approach |
|---|---|
| Learning Selenium | Simple Maven + Selenium + TestNG project. |
| Small smoke suite | Minimal BaseTest + Page Objects. |
| BDD requirement | Cucumber + Selenium Java. |
| Rich reports needed quickly | Serenity BDD or ExtentReports template. |
| Cloud testing | BrowserStack/Sauce Labs/LambdaTest sample framework. |
| Concise syntax preferred | Selenide. |

### Popular Selenium Java Framework Stacks

| Stack | Best Use Case |
|---|---|
| Selenium + Java + TestNG + Maven | Standard QA automation framework. |
| Selenium + Java + JUnit 5 | Dev-aligned Java teams. |
| Selenium + Cucumber + Java | BDD acceptance testing. |
| Selenium + Serenity BDD | Rich reports and living documentation. |
| Selenide | Shorter syntax and built-in waits. |
| Selenium Grid | Local distributed execution. |
| BrowserStack/Sauce Labs/LambdaTest | Cloud cross-browser coverage. |
| Selenium + Rest Assured | UI plus backend setup/cleanup. |

### Decision Rule

Build custom only when the project’s repeated complexity justifies the maintenance. Use simpler or pre-built tools when speed, learning, or a small scope matters more than custom architecture.

---

## Top 30 Selenium Java Technical Interview Questions

### 1. What is Selenium WebDriver?

Selenium WebDriver is a browser automation API that controls browsers through browser drivers.

```java
WebDriver driver = new ChromeDriver();
driver.get("https://example.com");
driver.quit();
```

### 2. What is WebDriver architecture?

Test code sends commands through WebDriver APIs to browser drivers, and browser drivers control browsers.

### 3. What is Selenium Grid?

Grid distributes tests across remote browsers, nodes, operating systems, and containers.

### 4. What locator strategies does Selenium support?

ID, name, class name, tag name, link text, partial link text, CSS selector, and XPath.

### 5. Which locator is best?

Stable ID or test-specific attribute is best. CSS is strong for attributes and hierarchy. XPath is strong for text and DOM relationships.

### 6. Difference between `findElement` and `findElements`?

`findElement` returns one element or throws. `findElements` returns a list and can return an empty list.

### 7. What is implicit wait?

A global wait applied to element lookup.

```java
driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10));
```

### 8. What is explicit wait?

A targeted wait for a specific condition.

```java
new WebDriverWait(driver, Duration.ofSeconds(10))
        .until(ExpectedConditions.elementToBeClickable(By.id("login")));
```

### 9. What is FluentWait?

A wait with custom timeout, polling interval, and ignored exceptions.

### 10. Why avoid `Thread.sleep()`?

It creates fixed delays and flaky/slow tests.

### 11. How do you handle dropdowns?

Use `Select` for native select elements.

```java
new Select(driver.findElement(By.id("country"))).selectByVisibleText("India");
```

### 12. How do you handle dynamic dropdowns?

Type text, wait for suggestions, loop through results, and click the matching value.

### 13. How do you handle checkboxes?

Check `isSelected()` before clicking.

```java
WebElement checkbox = driver.findElement(By.id("agree"));
if (!checkbox.isSelected()) checkbox.click();
```

### 14. How do you handle alerts?

```java
Alert alert = driver.switchTo().alert();
alert.accept();
```

### 15. How do you handle iframes?

```java
driver.switchTo().frame("frameName");
driver.switchTo().defaultContent();
```

### 16. How do you switch windows?

Use `getWindowHandles()` and `switchTo().window(handle)`.

### 17. What is Actions class?

A Selenium class for mouse and keyboard interactions.

### 18. How do you take screenshots?

```java
File src = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
```

### 19. What is JavaScriptExecutor?

It executes JavaScript in the browser.

```java
((JavascriptExecutor) driver).executeScript("window.scrollTo(0, document.body.scrollHeight)");
```

### 20. What is Page Object Model?

POM stores page locators and actions in page classes.

### 21. What is PageFactory?

PageFactory initializes elements annotated with `@FindBy`.

### 22. What is TestNG?

A Java testing framework supporting annotations, groups, XML suites, DataProvider, listeners, and parallel execution.

### 23. What is DataProvider?

A TestNG feature that runs the same test with multiple input data rows.

### 24. How do you run tests in parallel?

Use TestNG XML parallel settings and ThreadLocal WebDriver.

### 25. Why use ThreadLocal WebDriver?

It isolates each thread’s WebDriver instance during parallel execution.

### 26. What is ExtentReports?

A reporting library that creates HTML reports with status, logs, and screenshots.

### 27. How do you run tests from Maven?

Use `mvn clean test` with Surefire and TestNG XML.

### 28. How do you integrate Selenium with Jenkins?

Configure Jenkins to pull source code, run Maven tests, publish JUnit results, and archive artifacts.

### 29. How can API testing support Selenium?

API calls create data, authenticate users, validate backend state, and clean up records.

### 30. What makes a framework maintainable?

Clear package structure, Page Objects, reusable waits/utilities, data-driven tests, logging, reporting, screenshots, ThreadLocal, CI/CD, and readable tests.

---

## Summary

This README now shows all module information directly on the page and expands the content for each module with deeper explanations, additional Java Selenium examples, expected results, best practices, common mistakes, API testing, login testing, locator strategy, framework construction, framework selection guidance, and interview preparation.
