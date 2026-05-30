# Selenium Automation Advanced Frameworks with Java

A comprehensive Selenium WebDriver automation learning repository focused on **Java**, **Selenium WebDriver**, **TestNG**, advanced Selenium concepts, framework design, data-driven testing, Excel integration, Selenium Grid concepts, database testing, file upload/download automation, synchronization, locators, alerts, windows, frames, Java Streams, and real-world automation problem solving.

**Written by Brian McCarthy**

---

## Table of Contents

- [Project Overview](#project-overview)
- [Languages Used](#languages-used)
- [Technologies and Tools Used](#technologies-and-tools-used)
- [Methodologies Used](#methodologies-used)
- [Repository Structure](#repository-structure)
- [Project File Links](#project-file-links)
- [How the Project Works](#how-the-project-works)
- [Core Selenium Functions and Concepts](#core-selenium-functions-and-concepts)
- [Code Methodology Summary](#code-methodology-summary)
- [Sample Code from This Project](#sample-code-from-this-project)
  - [Browser Launch and Basic WebDriver Flow](#browser-launch-and-basic-webdriver-flow)
  - [Alert Handling](#alert-handling)
  - [Explicit Wait Synchronization](#explicit-wait-synchronization)
  - [Child Window Handling](#child-window-handling)
  - [Java Streams with Selenium WebTables](#java-streams-with-selenium-webtables)
  - [TestNG Annotations](#testng-annotations)
  - [Excel Upload and Data-Driven Validation](#excel-upload-and-data-driven-validation)
  - [File Upload and Download Automation](#file-upload-and-download-automation)
  - [Database Testing with Selenium](#database-testing-with-selenium)
- [Tutorial: Selenium Automation in Java](#tutorial-selenium-automation-in-java)
- [Guide: Building a Selenium Java Framework](#guide-building-a-selenium-java-framework)
- [Recommended Maven Framework Structure](#recommended-maven-framework-structure)
- [Common Commands](#common-commands)
- [Best Practices and Tips](#best-practices-and-tips)
- [Troubleshooting](#troubleshooting)
- [Suggested Improvements](#suggested-improvements)
- [Author](#author)

---

## Project Overview

This repository is organized as a section-by-section Selenium WebDriver training and framework-building project. The content starts with core Selenium and Java concepts, then progresses into advanced automation topics such as synchronization, web element handling, Ajax calls, child windows, iframes, Java Streams, TestNG, Maven, Jenkins, Log4j, Extent Reports, parallel execution, Cucumber, Page Object Model, data-driven frameworks, hybrid frameworks, Excel integration, database testing, file upload/download, AutoIT integration, Selenium Grid concepts, performance testing concepts, cloud automation concepts, and mobile automation basics.

The project is useful as a QA automation portfolio repository because it demonstrates practical hands-on Selenium skills across common real-world testing problems:

- Opening browsers and driving web applications with Selenium WebDriver
- Finding elements with `By.id`, `By.cssSelector`, `By.xpath`, and other locator strategies
- Automating forms, dropdowns, alerts, web tables, calendar widgets, Ajax loading, iframes, and child windows
- Using explicit waits instead of unreliable sleeps
- Validating behavior with TestNG assertions
- Creating repeatable tests using TestNG annotations
- Reading and writing Excel data with Apache POI
- Uploading and downloading files with Selenium and browser preferences
- Connecting Selenium tests to database records through JDBC
- Applying framework design concepts such as Page Object Model and data-driven testing

---

## Languages Used

| Language | Purpose |
|---|---|
| Java | Main automation language for Selenium WebDriver examples, TestNG tests, utility methods, Excel handling, JDBC, and framework design |
| XML | Commonly used for TestNG suite files, Maven `pom.xml`, and framework configuration patterns |
| SQL | Database testing examples using JDBC queries against MySQL-style data sources |
| HTML/CSS/XPath Concepts | Used for locator identification and UI automation targeting |
| Shell/Command Line | Used for running Maven, TestNG, Grid, Jenkins, and automation commands |

---

## Technologies and Tools Used

| Tool / Framework | Purpose |
|---|---|
| Selenium WebDriver | Browser automation and UI testing |
| Java | Test automation programming language |
| TestNG | Test runner, annotations, assertions, grouping, setup, teardown, and framework control |
| Maven | Build management and dependency management pattern |
| ANT | Legacy build automation pattern covered by the training material |
| Jenkins | CI/CD execution pattern for automated Selenium tests |
| Apache POI | Excel read/write support for data-driven testing |
| JDBC | Database connectivity for database-backed Selenium tests |
| ChromeDriver / FirefoxDriver | Browser-specific WebDriver implementations |
| Selenium Grid | Distributed and parallel browser execution concept |
| Log4j | Logging concept for framework diagnostics |
| Extent Reports | Rich HTML test execution reporting concept |
| Cucumber | BDD framework concept for Gherkin-based test scenarios |
| AutoIT | Desktop dialog integration for file upload workflows |
| Sauce Labs / Cloud Grid Concepts | Cloud execution pattern for browser testing |

---

## Methodologies Used

### 1. Functional UI Automation

The repository uses Selenium WebDriver to simulate real user actions: launching browsers, entering data, clicking elements, selecting dropdown options, accepting alerts, switching windows, switching frames, uploading files, downloading files, and validating page behavior.

### 2. Locator-Driven Test Design

The examples show how to identify UI elements with Selenium locators such as `By.id`, `By.cssSelector`, `By.xpath`, `By.linkText`, and table-related XPath expressions.

### 3. Synchronization and Wait Strategy

The project demonstrates the difference between unreliable static waits and better synchronization with `WebDriverWait` and `ExpectedConditions`.

### 4. TestNG-Based Test Organization

TestNG annotations such as `@BeforeMethod`, `@BeforeTest`, `@AfterMethod`, `@AfterTest`, and `@Test` are used to control setup, teardown, and test execution order.

### 5. Data-Driven Testing

Excel examples use Apache POI to download data, modify workbook values, upload updated data, and validate UI changes based on the edited file.

### 6. Framework Design

The repository covers framework design concepts including TestNG, Maven, ANT, Page Object Model, data-driven frameworks, hybrid frameworks, Jenkins, Extent Reports, Cucumber, Log4j, and Selenium Grid.

### 7. Database-Driven Testing

JDBC examples connect to a database, query credentials, and use database results as test input for Selenium workflows.

### 8. Real-World Automation Problem Solving

The repository includes practical examples for alerts, child windows, iframes, Ajax calls, calendar widgets, dynamic tables, streams, uploads, downloads, and browser profile preferences.

---

## Repository Structure

This repository is organized into numbered training sections. The files are primarily section folders containing Java snippets, notes, and code-download text files.

```text
Selenium-Automation-Advanced-Frameworks-Java/
├── S01 - Selenium Introduction/                              # Syllabus and course/topic overview
├── S05 - Adv. Locators Identification & Questions on Parsing Text/
├── S06 - Automate Web Elements/                              # Alerts, dropdowns, autosuggestive fields, element exercises
├── S07 - Functional testing with Selenium/                   # Functional Selenium test examples
├── S08 - Synchronization usage/                              # Implicit/explicit waits and synchronization examples
├── S09 - Automate Ajax Calls, Child Windows, iFrames/        # Window handles, Ajax, frame-related examples
├── S10 - Real Time Exercises/                                # Real-time UI exercises including calendar handling
├── S11 - Practical problems and Methods to Handle with Selenium/
├── S12 - Miscellaneous Topics/
├── S13 - Selenium Java Streams/                              # Java Stream usage with Selenium web tables
├── S14 - Selenium 4.0 - Latest Features/                     # Selenium 4 concepts and examples
├── S15 - Framework Part 1 -  TestNG/                         # TestNG annotations and execution flow
├── S28 - Upload Download functionalities using excel files/  # Apache POI, Excel update, upload/download testing
├── S31 - DataBase connection to Selenium Testcases/          # JDBC and Selenium database-driven testing
├── S32 - File Uploading & Downloading with Selenium/         # Browser preferences, AutoIT, file validation
└── README.md                                                 # Project documentation
```

---

## Project File Links

### Main Repository Files

- [README.md](README.md)
- [Selenium Syllabus](S01%20-%20Selenium%20Introduction/Selenium%20Syllabus.txt)

### Important Section Folders

- [S01 - Selenium Introduction](S01%20-%20Selenium%20Introduction/)
- [S05 - Advanced Locators Identification & Parsing Text](S05%20-%20Adv.%20Locators%20Identification%20%26%20Questions%20on%20Parsing%20Text/)
- [S06 - Automate Web Elements](S06%20-%20Automate%20Web%20Elements/)
- [S07 - Functional Testing with Selenium](S07%20-%20Functional%20testing%20with%20Selenium/)
- [S08 - Synchronization Usage](S08%20-%20Synchronization%20usage/)
- [S09 - Ajax Calls, Child Windows, iFrames](S09%20-%20Automate%20Ajax%20Calls%2C%20Child%20Windows%2C%20iFrames/)
- [S10 - Real Time Exercises](S10%20-%20Real%20Time%20Exercises/)
- [S11 - Practical Selenium Problems](S11%20-%20Practical%20problems%20and%20Methods%20to%20Handle%20with%20Selenium/)
- [S12 - Miscellaneous Topics](S12%20-%20Miscellaneous%20Topics/)
- [S13 - Selenium Java Streams](S13%20-%20Selenium%20Java%20Streams/)
- [S14 - Selenium 4.0 Latest Features](S14%20-%20Selenium%204.0%20-%20Latest%20Features/)
- [S15 - Framework Part 1 - TestNG](S15%20-%20Framework%20Part%201%20-%20%20TestNG/)
- [S28 - Upload Download Functionalities Using Excel Files](S28%20-%20Upload%20Download%20functionalities%20using%20excel%20files/)
- [S31 - Database Connection to Selenium Testcases](S31%20-%20DataBase%20connection%20to%20Selenium%20Testcases/)
- [S32 - File Uploading & Downloading with Selenium](S32%20-%20File%20Uploading%20%26%20Downloading%20with%20Selenium/)

### Key Example Files

- [Alert Handling Example](S06%20-%20Automate%20Web%20Elements/Alerts%20code%20download.txt)
- [Synchronization Example](S08%20-%20Synchronization%20usage/code.txt)
- [Child Window Handling Example](S09%20-%20Automate%20Ajax%20Calls%2C%20Child%20Windows%2C%20iFrames/Code%20download.txt)
- [Calendar UI Example](S10%20-%20Real%20Time%20Exercises/Code%20-%20Calendar%20UI.txt)
- [Java Streams WebTable Example](S13%20-%20Selenium%20Java%20Streams/Code%20Download.txt)
- [TestNG Annotation Example](S15%20-%20Framework%20Part%201%20-%20%20TestNG/doc.txt)
- [Excel Upload/Download Example](S28%20-%20Upload%20Download%20functionalities%20using%20excel%20files/Code%20download.txt)
- [Database Connection Example](S31%20-%20DataBase%20connection%20to%20Selenium%20Testcases/doc%20(2).txt)
- [File Upload/Download Example](S32%20-%20File%20Uploading%20%26%20Downloading%20with%20Selenium/Full%20Code%20download.txt)

---

## How the Project Works

This repository works as a progressive Selenium automation reference:

1. **Start with Selenium fundamentals.** The syllabus introduces Java, Selenium WebDriver, Selenium 4, TestNG, Maven, Jenkins, Log4j, reports, Cucumber, data-driven frameworks, Page Object Model, database testing, performance testing, mobile basics, cloud automation, AutoIT, and defect management.

2. **Practice element automation.** The web element sections demonstrate locating elements, filling fields, clicking controls, selecting dropdowns, handling alerts, and validating text.

3. **Handle synchronization.** The synchronization examples show how to wait for dynamic content using `WebDriverWait` and `ExpectedConditions`.

4. **Automate complex browser behavior.** Ajax calls, child windows, and iframes are handled through Selenium switching APIs such as `driver.switchTo().window()`.

5. **Use Java language features.** Java Streams are used to collect, sort, filter, and validate web table data.

6. **Organize tests with TestNG.** TestNG annotations control before/after execution and define independent test methods.

7. **Apply data-driven concepts.** Excel examples use Apache POI to find rows/columns, update data, upload files, and assert the UI reflects updated values.

8. **Connect to databases.** JDBC examples retrieve data from a database and use that data inside browser tests.

9. **Automate files.** File upload/download examples configure browser preferences, execute upload tools, wait for results, and verify downloaded files exist.

---

## Core Selenium Functions and Concepts

| Function / Concept | Purpose |
|---|---|
| `new ChromeDriver()` | Launches Chrome browser through Selenium WebDriver |
| `new FirefoxDriver()` | Launches Firefox browser through Selenium WebDriver |
| `driver.get(url)` | Opens a web application URL |
| `driver.findElement(By.id(...))` | Finds one element by ID |
| `driver.findElement(By.cssSelector(...))` | Finds one element by CSS selector |
| `driver.findElement(By.xpath(...))` | Finds one element by XPath |
| `driver.findElements(...)` | Finds multiple matching elements |
| `sendKeys()` | Types text into an input or sends keyboard keys |
| `click()` | Clicks an element |
| `getText()` | Reads visible text from an element |
| `getAttribute()` | Reads an HTML attribute value |
| `driver.switchTo().alert()` | Switches Selenium focus to an alert |
| `alert.accept()` | Accepts an alert |
| `alert.dismiss()` | Dismisses a confirmation alert |
| `driver.getWindowHandles()` | Gets all browser window handles |
| `driver.switchTo().window(id)` | Switches focus to another browser window |
| `WebDriverWait` | Explicit wait helper for dynamic pages |
| `ExpectedConditions` | Prebuilt conditions for explicit waits |
| `Assert.assertTrue()` | TestNG assertion for true/false validation |
| `Assert.assertEquals()` | TestNG assertion for expected vs actual values |
| `@BeforeTest` | Runs setup before all tests in a TestNG test scope |
| `@BeforeMethod` | Runs setup before each TestNG test method |
| `@Test` | Marks a method as a TestNG test |
| `@AfterMethod` | Runs cleanup/reporting after each test method |
| `@AfterTest` | Runs cleanup after all tests in a TestNG test scope |
| `XSSFWorkbook` | Apache POI object for Excel `.xlsx` workbooks |
| `DriverManager.getConnection()` | Creates a JDBC database connection |

---

## Code Methodology Summary

The code examples follow a hands-on learning style. Many examples use a `main()` method to demonstrate the concept directly, while framework sections introduce TestNG annotations and scalable framework ideas.

The repository emphasizes these automation methodologies:

- **Direct WebDriver scripting** for learning core browser automation
- **Locator strategy practice** with ID, CSS, XPath, link text, and table XPath expressions
- **Explicit wait synchronization** for dynamic pages
- **TestNG lifecycle management** for structured setup, test execution, and teardown
- **Assertion-driven validation** with TestNG
- **Data-driven testing** using Excel and Apache POI
- **Database-backed testing** using JDBC query results as input data
- **File-system validation** for download verification
- **Browser preference configuration** for download locations
- **Framework design concepts** such as Page Object Model, hybrid framework design, reports, logging, Grid, Jenkins, and Cucumber

---

## Sample Code from This Project

### Browser Launch and Basic WebDriver Flow

```java
System.setProperty("webdriver.chrome.driver", "C://chromedriver.exe");
WebDriver driver = new ChromeDriver();
driver.get("https://rahulshettyacademy.com/AutomationPractice/");
driver.findElement(By.id("name")).sendKeys("Rahul");
driver.findElement(By.cssSelector("[id='alertbtn']")).click();
```

**How it works:**

- Sets the path to ChromeDriver.
- Launches a Chrome browser.
- Opens a test site.
- Locates the name input by ID.
- Types text into the field.
- Finds a button with a CSS selector and clicks it.

---

### Alert Handling

```java
String text = "Rahul";

System.setProperty("webdriver.chrome.driver", "C://chromedriver.exe");
WebDriver driver = new ChromeDriver();

driver.get("https://rahulshettyacademy.com/AutomationPractice/");
driver.findElement(By.id("name")).sendKeys(text);
driver.findElement(By.cssSelector("[id='alertbtn']")).click();

System.out.println(driver.switchTo().alert().getText());
driver.switchTo().alert().accept();

driver.findElement(By.id("confirmbtn")).click();
System.out.println(driver.switchTo().alert().getText());
driver.switchTo().alert().dismiss();
```

**How it works:**

- Enters text into a page field.
- Triggers a JavaScript alert.
- Switches Selenium focus from the page to the alert.
- Reads the alert message.
- Accepts the alert.
- Opens a confirmation alert and dismisses it.

---

### Explicit Wait Synchronization

```java
System.setProperty("webdriver.chrome.driver", "C:\\work\\chromedriver.exe");
WebDriver driver = new ChromeDriver();

driver.get("https://alaskatrips.poweredbygps.com/g/pt/hotels?MDPCID=ALASKA-US.TPS.BRAND.hotels.HOTEL");
driver.findElement(By.id("H-destination")).sendKeys("nyc");
driver.findElement(By.id("H-destination")).sendKeys(Keys.TAB);
driver.findElement(By.id("H-fromDate")).sendKeys(Keys.ENTER);

WebDriverWait wait = new WebDriverWait(driver, 20);
wait.until(ExpectedConditions.elementToBeClickable(By.xpath("//div[@id='resultsContainer']/section/article[1]")));

driver.findElement(By.xpath("//div[@id='resultsContainer']/section/article[1]")).click();
```

**How it works:**

- Opens a dynamic travel/hotel page.
- Enters search data.
- Uses `WebDriverWait` to wait until the first result is clickable.
- Clicks only after Selenium confirms the element is ready.
- This is more reliable than using `Thread.sleep()`.

---

### Child Window Handling

```java
WebDriver driver = new ChromeDriver();
driver.get("https://rahulshettyacademy.com/loginpagePractise/#");

driver.findElement(By.cssSelector(".blinkingText")).click();

Set<String> windows = driver.getWindowHandles();
Iterator<String> it = windows.iterator();
String parentId = it.next();
String childId = it.next();

driver.switchTo().window(childId);
String emailId = driver.findElement(By.cssSelector(".im-para.red"))
    .getText()
    .split("at")[1]
    .trim()
    .split(" ")[0];

driver.switchTo().window(parentId);
driver.findElement(By.id("username")).sendKeys(emailId);
```

**How it works:**

- Clicks a link that opens a child window.
- Gets all window handles.
- Stores parent and child window IDs.
- Switches to the child window.
- Extracts an email address from the child window text.
- Switches back to the parent window.
- Uses the extracted email in the login field.

---

### Java Streams with Selenium WebTables

```java
List<WebElement> elementsList = driver.findElements(By.xpath("//tr/td[1]"));

List<String> originalList = elementsList.stream()
    .map(s -> s.getText())
    .collect(Collectors.toList());

List<String> sortedList = originalList.stream()
    .sorted()
    .collect(Collectors.toList());

Assert.assertTrue(originalList.equals(sortedList));

List<String> price;
do {
    List<WebElement> rows = driver.findElements(By.xpath("//tr/td[1]"));
    price = rows.stream()
        .filter(s -> s.getText().contains("Rice"))
        .map(s -> getPriceVeggie(s))
        .collect(Collectors.toList());

    price.forEach(a -> System.out.println(a));

    if (price.size() < 1) {
        driver.findElement(By.cssSelector("[aria-label='Next']")).click();
    }
} while (price.size() < 1);
```

**How it works:**

- Captures table cells into a list of Selenium `WebElement` objects.
- Converts web elements into visible text with Java Streams.
- Sorts the text list.
- Compares the UI list against the sorted list.
- Searches paginated table rows for a product.
- Clicks next page until the target product is found.

---

### TestNG Annotations

```java
@BeforeMethod
public void UseridGeneration() {
    System.out.println("This block executes before each Test");
}

@BeforeTest
public void Cookies() {
    System.out.println("This block executes Before all Testcases");
    // delete cookies
}

@AfterTest
public void Cookiesclose() {
    System.out.println("This block executes after all Testcases");
    // close the browsers
}

@AfterMethod
public void Reportadding() {
    System.out.println("This block executes after each Test");
}

@Test
public void OpeningBrowser() {
    System.out.println("Executing Test 2");
}

@Test
public void FlightBooking() {
    System.out.println("Executing Test 1");
}
```

**How it works:**

- `@BeforeTest` runs once before test execution.
- `@BeforeMethod` runs before each `@Test` method.
- `@Test` marks executable test cases.
- `@AfterMethod` runs after each test method.
- `@AfterTest` runs once after all tests complete.

---

### Excel Upload and Data-Driven Validation

```java
String fruitName = "Apple";
String updatedValue = "603";
String fileName = "/Users/rahulshetty/downloads/download.xlsx";

WebDriver driver = new ChromeDriver();
driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(7));
driver.get("https://rahulshettyacademy.com/upload-download-test/index.html");

driver.findElement(By.cssSelector("#downloadButton")).click();

int col = getColumnNumber(fileName, "price");
int row = getRowNumber(fileName, "Apple");
Assert.assertTrue(updateCell(fileName, row, col, updatedValue));

WebElement upload = driver.findElement(By.cssSelector("input[type='file']"));
upload.sendKeys("/Users/rahulshetty/downloads/download.xlsx");

By toastLocator = By.cssSelector(".Toastify__toast-body div:nth-child(2");
WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
wait.until(ExpectedConditions.visibilityOfElementLocated(toastLocator));

String toastText = driver.findElement(toastLocator).getText();
Assert.assertEquals("Updated Excel Data Successfully.", toastText);
```

**How it works:**

- Downloads an Excel file from the application.
- Uses Apache POI helper methods to find a row and column.
- Updates a cell value.
- Uploads the modified Excel file back into the application.
- Waits for the success message.
- Asserts that the upload was processed successfully.

---

### File Upload and Download Automation

```java
String downloadPath = System.getProperty("user.dir");

HashMap<String, Object> chromePrefs = new HashMap<String, Object>();
chromePrefs.put("profile.default_content_settings.popups", 0);
chromePrefs.put("download.default_directory", downloadPath);

ChromeOptions options = new ChromeOptions();
options.setExperimentalOption("prefs", chromePrefs);

WebDriver driver = new ChromeDriver(options);
driver.get("https://altoconvertpdftojpg.com/");

driver.findElement(By.cssSelector("[class*='btn--choose']")).click();
Runtime.getRuntime().exec("C:\\Users\\rahul\\Documents\\check\\fileupload.exe");

WebDriverWait wait = new WebDriverWait(driver, 10);
wait.until(ExpectedConditions.visibilityOfElementLocated(By.cssSelector("button[class*='medium']")));
driver.findElement(By.cssSelector("button[class*='medium']")).click();

wait.until(ExpectedConditions.visibilityOfElementLocated(By.linkText("Download Now")));
driver.findElement(By.linkText("Download Now")).click();

File file = new File(downloadPath + "/converted.zip");
Assert.assertTrue(file.exists());
```

**How it works:**

- Sets Chrome download preferences.
- Opens a PDF conversion site.
- Uses AutoIT executable integration for desktop file chooser automation.
- Waits for conversion controls.
- Downloads the converted file.
- Verifies the downloaded file exists locally.

---

### Database Testing with Selenium

```java
String host = "localhost";
String port = "3306";

Connection con = DriverManager.getConnection(
    "jdbc:mysql://" + host + ":" + port + "/demo",
    "root",
    "root"
);

Statement statement = con.createStatement();
ResultSet rs = statement.executeQuery(
    "select * from credentials where scenario ='rewardscard'"
);

while (rs.next()) {
    WebDriver driver = new FirefoxDriver();
    driver.get("https://login.salesforce.com");
    driver.findElement(By.xpath(".//*[@id='username']")).sendKeys(rs.getString("username"));
    driver.findElement(By.xpath(".//*[@id='password']")).sendKeys(rs.getString("password"));
}
```

**How it works:**

- Opens a JDBC connection to a local database.
- Runs a SQL query to retrieve test credentials.
- Iterates through database results.
- Uses the returned username and password in a Selenium login flow.

---

## Tutorial: Selenium Automation in Java

### 1. Install Java JDK

Install a current Java JDK and confirm it works:

```bash
java -version
javac -version
```

### 2. Install an IDE

Recommended IDEs:

- IntelliJ IDEA
- Eclipse
- VS Code with Java extensions

### 3. Create a Maven Project

A modern Selenium project should usually use Maven instead of manually managing JAR files.

```bash
mvn archetype:generate -DgroupId=com.brian.selenium -DartifactId=selenium-java-framework -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

### 4. Add Dependencies

Example `pom.xml` dependencies:

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
        <groupId>org.apache.poi</groupId>
        <artifactId>poi-ooxml</artifactId>
        <version>5.2.5</version>
    </dependency>
</dependencies>
```

### 5. Create a Basic Selenium Test

```java
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.Assert;
import org.testng.annotations.Test;

public class LoginTest {

    @Test
    public void loginPageShouldLoad() {
        WebDriver driver = new ChromeDriver();
        driver.get("https://example.com/login");

        Assert.assertTrue(driver.findElement(By.id("username")).isDisplayed());

        driver.quit();
    }
}
```

### 6. Run Tests

```bash
mvn test
```

---

## Guide: Building a Selenium Java Framework

A strong Selenium Java framework should include these layers:

### 1. Base Test Layer

Handles WebDriver setup, browser selection, teardown, screenshots, and environment configuration.

```java
public class BaseTest {
    protected WebDriver driver;

    @BeforeMethod
    public void setUp() {
        driver = new ChromeDriver();
        driver.manage().window().maximize();
    }

    @AfterMethod
    public void tearDown() {
        if (driver != null) {
            driver.quit();
        }
    }
}
```

### 2. Page Object Layer

Keeps locators and page actions out of test classes.

```java
public class LoginPage {
    private WebDriver driver;
    private By username = By.id("username");
    private By password = By.id("password");
    private By loginButton = By.id("loginBtn");

    public LoginPage(WebDriver driver) {
        this.driver = driver;
    }

    public void login(String user, String pass) {
        driver.findElement(username).sendKeys(user);
        driver.findElement(password).sendKeys(pass);
        driver.findElement(loginButton).click();
    }
}
```

### 3. Test Layer

Tests should describe business behavior and use page objects.

```java
public class LoginTest extends BaseTest {

    @Test
    public void validUserCanLogin() {
        driver.get("https://example.com/login");
        LoginPage loginPage = new LoginPage(driver);
        loginPage.login("standard_user", "secret");

        Assert.assertTrue(driver.getCurrentUrl().contains("dashboard"));
    }
}
```

### 4. Utility Layer

Common utility classes should handle:

- Excel reads/writes
- Config properties
- Screenshots
- Waits
- Database connections
- File download checks
- Reporting
- Logging

### 5. Reporting Layer

Use Extent Reports or another reporting tool to capture:

- Passed tests
- Failed tests
- Screenshots
- Execution time
- Browser/environment details

### 6. CI Layer

Use Jenkins or GitHub Actions to:

- Checkout code
- Install dependencies
- Run tests
- Publish reports
- Archive screenshots/logs

---

## Recommended Maven Framework Structure

```text
selenium-java-framework/
├── pom.xml
├── testng.xml
├── src/
│   ├── main/
│   │   └── java/
│   │       └── framework/
│   │           ├── base/
│   │           │   └── BaseTest.java
│   │           ├── pages/
│   │           │   ├── LoginPage.java
│   │           │   └── HomePage.java
│   │           ├── utils/
│   │           │   ├── ConfigReader.java
│   │           │   ├── ExcelUtils.java
│   │           │   ├── WaitUtils.java
│   │           │   └── ScreenshotUtils.java
│   │           └── reporting/
│   │               └── ExtentReportManager.java
│   └── test/
│       └── java/
│           └── tests/
│               ├── LoginTest.java
│               ├── CheckoutTest.java
│               └── DatabaseLoginTest.java
├── src/test/resources/
│   ├── config.properties
│   ├── testdata.xlsx
│   └── log4j.properties
└── test-output/
```

---

## Common Commands

| Command | Purpose |
|---|---|
| `java -version` | Check installed Java version |
| `mvn -version` | Check Maven installation |
| `mvn clean` | Clean build output |
| `mvn test` | Run Maven tests |
| `mvn test -DsuiteXmlFile=testng.xml` | Run a TestNG suite through Maven Surefire |
| `mvn clean test` | Clean and execute tests |
| `mvn test -Dbrowser=chrome` | Example browser parameter pattern |
| `mvn test -Denv=qa` | Example environment parameter pattern |

---

## Best Practices and Tips

### Prefer Explicit Waits

Avoid relying on `Thread.sleep()` except for temporary debugging. Use `WebDriverWait` and `ExpectedConditions`.

```java
WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
wait.until(ExpectedConditions.visibilityOfElementLocated(By.id("successMessage")));
```

### Always Quit the Browser

Use `driver.quit()` in teardown to close all browser windows and end the WebDriver session.

### Use Page Object Model

Avoid duplicating locators across tests. Put locators and page actions inside page classes.

### Keep Tests Independent

Each test should set up its own state and not depend on the execution order of another test.

### Store Test Data Separately

Use Excel, CSV, JSON, properties files, or a database for test data when the same flow must run with many inputs.

### Avoid Hardcoded Driver Paths

Modern Selenium can use Selenium Manager, WebDriverManager, or project-level configuration instead of hardcoded local paths such as `C://chromedriver.exe`.

### Use Stable Locators

Preferred locator order:

1. ID
2. Name
3. CSS selector
4. XPath only when needed
5. Avoid brittle absolute XPath

### Validate with Assertions

Do not only print values to the console. Use `Assert.assertEquals()`, `Assert.assertTrue()`, or framework assertions.

### Capture Screenshots on Failure

Add screenshot capture in `@AfterMethod` when a test fails. This helps debug CI failures.

### Keep Secrets Out of Source Code

Do not commit database passwords, usernames, API keys, or cloud-grid credentials. Use environment variables or secure CI credentials.

---

## Troubleshooting

### Browser Does Not Launch

Check:

- Browser is installed
- WebDriver version matches browser version, if manually managed
- Driver path is correct
- Selenium dependency version is compatible

### Element Not Found

Check:

- Locator is correct
- Element is inside an iframe
- Element appears after Ajax loading
- Page has fully loaded
- Test is using the correct environment URL

### Stale Element Reference

Re-locate the element after a page refresh, table update, or DOM change.

### Timing Failures

Replace hard waits with explicit waits.

### File Upload Fails

For standard HTML file inputs, prefer:

```java
driver.findElement(By.cssSelector("input[type='file']")).sendKeys(filePath);
```

Use AutoIT only when the upload control opens a native Windows dialog that Selenium cannot control directly.

### Excel File Is Locked

Close the workbook and file streams after reading or writing:

```java
workbook.close();
fis.close();
```

### Database Connection Fails

Check:

- Database host and port
- Credentials
- JDBC driver dependency
- Schema/table name
- Network/firewall access

---

## Suggested Improvements

Future improvements that would make this repository stronger as a professional automation portfolio:

1. Convert text snippets into a standard Maven project.
2. Add a root-level `pom.xml` with Selenium, TestNG, Apache POI, WebDriverManager, Log4j, and reporting dependencies.
3. Add `src/main/java` and `src/test/java` package structure.
4. Add a `testng.xml` suite file.
5. Add Page Object Model classes for repeated pages.
6. Add reusable wait, screenshot, Excel, file, and database utility classes.
7. Add Extent Reports or Allure Reports.
8. Add Jenkinsfile or GitHub Actions workflow for CI execution.
9. Add browser parameterization for Chrome, Firefox, and Edge.
10. Add Selenium Grid or cloud execution examples.
11. Add README screenshots of reports and test execution output.
12. Add `.gitignore` rules for target folders, reports, logs, downloaded files, and credentials.
13. Add `.env.example` or `config.properties.example` for safe configuration.

---

## Author

**Written by Brian McCarthy**

This project demonstrates Selenium WebDriver automation knowledge in Java, including locators, waits, alerts, windows, web tables, Java Streams, TestNG, Excel data-driven testing, file upload/download automation, database testing with JDBC, and advanced framework design concepts.
