# Selenium-JAVA

A comprehensive **Selenium WebDriver automation learning/training project** built with Java. This project documents a progressive learning journey from basic WebDriver interactions to advanced Page Object Model (POM) and Data-Driven Testing (DDT) using Apache POI.

> **Author:** Swapnil Chhabilwad  
> **GitHub:** [https://github.com/swapnilchhabilwad/Selenium-JAVA.git](https://github.com/swapnilchhabilwad/Selenium-JAVA.git)  
> **IDE:** Eclipse  
> **Java Version:** JavaSE-1.8  
> **Selenium Version:** 4.16.1 / 4.17.0  

---

## Table of Contents

- [Project Structure](#project-structure)
- [Module Overview](#module-overview)
  - [1. Practice00 — Selenium Basics](#1-practice00--selenium-basics)
  - [2. SeleniumPractice — Data-Driven Testing (Beginner)](#2-seleniumpractice--data-driven-testing-beginner)
  - [3. SeleniumPractice0 — Comprehensive Automation](#3-seleniumpractice0--comprehensive-automation)
- [Topics Covered](#topics-covered)
- [Framework & Design Patterns](#framework--design-patterns)
- [Dependencies](#dependencies)
- [How to Run](#how-to-run)
- [Code Quality Notes](#code-quality-notes)

---

## Project Structure

```
Selenium-JAVA/
├── README.md
├── Practice00/                  # Selenium Basics module
│   ├── src/
│   ├── Jarfiles/
│   ├── Drivers/
│   ├── Photo/
│   └── bin/
├── SeleniumPractice/            # DDT (Beginner) module
│   ├── src/
│   ├── JarFiles/
│   ├── Drviers/
│   ├── Book1.xlsx               # Excel test data
│   ├── data.properties          # Configuration properties
│   └── bin/
├── SeleniumPractice0/           # Comprehensive module (POM + DDT + POI)
│   ├── src/
│   ├── JarFiles/
│   ├── Drviers/
│   ├── poi/                     # Apache POI JARs
│   ├── Photo/
│   ├── Book1.xlsx
│   ├── data.properties
│   └── bin/
└── seleniumpractice1/           # (deleted - consolidated module)
```

---

## Module Overview

### 1. Practice00 — Selenium Basics

**Purpose:** Foundational Selenium WebDriver concepts and basic browser automation.

**Topics Covered:**

| Package | Files | Concepts |
|---------|-------|----------|
| `Actionsclass/` | Doubleclick, Draganddrop, Mouseclick, Mousehover, Rightclick | Actions class interactions |
| `autosuggestion/` | AutoGoogle | Google search auto-suggestions |
| `chapter1p/` | Instalogin, Isdisplayed, Isenabled, Isselected, SelectDeselect, TraversingXpath, VerificationLogin | Element state verification, XPath traversal, login forms |
| `chapter2p/` | Dropdown, DropdownEbay, ScreenShots, Scrollbar, ScrollbarLocation | Select dropdowns, screenshots, scroll bars |
| `frames/` | Snapdeal | Handling iframes |
| `getters/` | getlocation, Getsize, Gettext | WebElement getter methods |
| `popups/` | AlertPopups, Hiddenorcalender, NewTab, Redbuscalender, WindowHandles | Alerts, calendar popups, window/tab handling |
| *(root)* | Test00 | Mixed exercise combining multiple concepts |

**Dependencies:**
- `selenium-server-4.17.0.jar`
- `commons-io-2.15.1.jar`

---

### 2. SeleniumPractice — Data-Driven Testing (Beginner)

**Purpose:** Introduction to Data-Driven Testing (DDT) using Excel and properties files.

**Packages:**
- `SeleniumBasics/` — Launch skeleton (ChromeDriver instantiation)
- `datadriven/` — DDT test files (Facebook login, Test01, Test02)

**Data Files:**
- `Book1.xlsx` — Excel test data
- `data.properties` — Configuration properties

**Dependencies:**
- `selenium-server-4.16.1.jar`

---

### 3. SeleniumPractice0 — Comprehensive Automation

**Purpose:** Most advanced module combining Page Object Model (POM), Data-Driven Testing (DDT), and comprehensive UI interactions.

**Packages:**

| Package | Files | Concepts |
|---------|-------|----------|
| `Actions/` | Selectoptions | Select options via Actions class |
| `Autosuggestion/` | Test00, Test01 | Google auto-suggest (variants) |
| `Chapter3/` | Actitime, ActitimeTest1, ddt, excelfile, facebooklogin, FacebookTest1, googlepage, Instagram, InstagramTest1, Skillrary, SkillraryTest1, staleelement | **POM implementation** — Each website has a page class + test class + DDT integration |
| `Multipleselect/` | multipleselect | Multi-select dropdown handling |
| `Popups/` | Alertconfirmation, Downloadpopups, Fileuploadpopup, Frames, prompt, Timealert | Comprehensive popup handling |
| `SeleniumLocators/` | Launch | Locator exploration skeleton |
| `webelement/` | Test1–7, TestP1–6 | Extensive WebElement interaction tests |
| *(root)* | takescreenshots, Windowhandle | Screenshots + window handling |

**Data Files:**
- `Book1.xlsx` — Excel test data
- `data.properties` — Configuration properties

**Dependencies:**
- `selenium-server-4.16.1.jar`
- `commons-io-2.15.0.jar`
- **Apache POI 5.2.2** (full suite: poi, poi-ooxml, poi-scratchpad, plus supporting libraries)

---

## Topics Covered

| Topic | Description | Module(s) |
|-------|-------------|-----------|
| **Basic Navigation** | Opening URLs, browser maximize, navigation | Practice00, SeleniumPractice0 |
| **Locators** | ID, Name, XPath, CSS selectors | Practice00, SeleniumPractice0 |
| **Element State Verification** | isDisplayed(), isEnabled(), isSelected() | Practice00 |
| **Dropdowns (Select class)** | Single and multi-select dropdowns | Practice00, SeleniumPractice0 |
| **Actions Class** | Double click, drag-and-drop, mouse hover, right click | Practice00 |
| **Auto-Suggestion** | Handling Google search suggestions | Practice00, SeleniumPractice0 |
| **Frames / iframes** | Switching between frames | Practice00, SeleniumPractice0 |
| **Window Handles** | Switching between tabs/windows | Practice00, SeleniumPractice0 |
| **Alert Popups** | Handling JavaScript alerts, confirmation, prompts | Practice00, SeleniumPractice0 |
| **Calendar / Hidden Popups** | Date pickers, hidden elements | Practice00 |
| **Scroll Bars** | Scrolling by pixel and to elements | Practice00 |
| **Screenshots** | Taking full-page and element screenshots | Practice00, SeleniumPractice0 |
| **File Upload/Download** | Handling file upload and download popups | SeleniumPractice0 |
| **Getter Methods** | getLocation(), getSize(), getText() | Practice00 |
| **Stale Elements** | Handling StaleElementReferenceException | SeleniumPractice0 |
| **Apache POI (Excel)** | Reading data-driven test data from .xlsx files | SeleniumPractice0 |
| **Page Object Model (POM)** | @FindBy + PageFactory.initElements() | SeleniumPractice0 |

---

## Framework & Design Patterns

### Page Object Model (POM)
The project implements POM using the **Declaration → Initialization → Utilization** pattern:
```java
// Declaration
@FindBy (id="email")
private WebElement usernametb;

// Initialization (Constructor)
public facebooklogin(WebDriver driver) {
    PageFactory.initElements(driver, this);
}

// Utilization
public void usernametextbox(String user) {
    usernametb.sendKeys(user);
}
```

### Data-Driven Testing (DDT)
Apache POI is used to read test data from Excel files (`.xlsx`), combined with `.properties` files for configuration:
```java
FileInputStream fis = new FileInputStream("./Book1.xlsx");
Workbook wb = WorkbookFactory.create(fis);
```

### Wait Strategies
- **Implicit Waits:** `driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10))`
- **Thread.sleep():** Used extensively (should be replaced with Explicit Waits)

---

## Dependencies

### All Modules
| Dependency | Version | Used In |
|-----------|---------|---------|
| Selenium Server | 4.16.1 / 4.17.0 | All modules |
| Commons IO | 2.15.0 / 2.15.1 | Practice00, SeleniumPractice0 |
| Apache POI | 5.2.2 | SeleniumPractice0 |
| Commons Codec | 1.15 | SeleniumPractice0 |
| Commons Collections4 | 4.4 | SeleniumPractice0 |
| Commons Compress | 1.21 | SeleniumPractice0 |
| XMLBeans | 5.0.3 | SeleniumPractice0 |
| Log4j API | 2.17.2 | SeleniumPractice0 |
| SLF4J API | 1.7.36 | SeleniumPractice0 |

> **Note:** Dependencies are managed manually via Eclipse build path (JAR files). The project does not use Maven or Gradle.

### Browser Driver
- **Browser:** Google Chrome (exclusively)
- **Driver Path:** Currently hardcoded to `C:\Users\swapn\Downloads\Selenium supportive files\chromedriver-win32\chromedriver.exe`

> **Important:** Selenium 4.6+ includes **Selenium Manager**, which automatically manages browser drivers. The `System.setProperty(...)` calls for ChromeDriver are no longer necessary and should be removed for portability.

---

## How to Run

### Prerequisites
1. **Java Development Kit (JDK) 8** or later installed
2. **Eclipse IDE** (or any Java IDE)
3. **Google Chrome** browser installed

### Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/swapnilchhabilwad/Selenium-JAVA.git
   ```

2. **Import into Eclipse:**
   - File → Import → General → Existing Projects into Workspace
   - Select the cloned directory
   - Import the desired module(s): `Practice00`, `SeleniumPractice`, `SeleniumPractice0`

3. **Update ChromeDriver path** (if using Selenium < 4.6):
   - Open any `.java` file
   - Replace the path in `System.setProperty("webdriver.chrome.driver", "...")` with the path to your local `chromedriver.exe`
   - Or simply **remove the line** and let Selenium Manager handle it automatically (Selenium 4.6+)

4. **Run a test:**
   - Right-click on any `.java` file with a `main()` method
   - Select **Run As → Java Application**

---

## Code Quality Notes

This is a **learning/training project** and the code reflects an educational progression. Below are observations for anyone reviewing or contributing:

### Areas for Improvement
1. **Hardcoded ChromeDriver paths** — Replace with Selenium Manager (already available in Selenium 4.6+)
2. **No test framework** — No JUnit or TestNG; tests run via `main()` methods. Adding TestNG would enable assertions, test suites, and reporting
3. **`Thread.sleep()` usage** — Should be replaced with **Explicit Waits** (`WebDriverWait` + `ExpectedConditions`) for more reliable and faster tests
4. **No assertions** — Tests print "Pass"/"Fail" to console instead of using proper assertion libraries
5. **Excessive whitespace** — Many files end with 50–80+ blank lines
6. **No exception handling** — Most methods throw exceptions rather than handling them with try-catch
7. **No build tool** — Switching to Maven/Gradle would simplify dependency management significantly
8. **Incomplete files** — Some files are empty skeletons (e.g., some files in SeleniumPractice)

### Best Practices Demonstrated
- ✅ Page Object Model pattern with `@FindBy` and `PageFactory`
- ✅ Data-Driven Testing with Apache POI
- ✅ Implicit waits for synchronization
- ✅ Modular package organization by concept

---

## License

This project is for educational and learning purposes.