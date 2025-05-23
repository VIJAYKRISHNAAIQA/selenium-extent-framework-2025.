

# 🛠️ Selenium-Extent-Framework-2025.

This is a **Selenium WebDriver** automation framework integrated with **TestNG** and **ExtentReports**. It is designed to run automated tests, generate detailed HTML reports, and capture screenshots on test failures.

## 🚀 Features

- **TestNG Integration**: For test execution and reporting.
- **ExtentReports**: For generating rich, interactive HTML reports.
- **Screenshot on Failure**: Automatically takes screenshots for failed tests.
- **Easy Setup**: Uses Maven for dependency management.

## 📋 Prerequisites

- **Java 17 or higher** installed.
- **Maven** installed.
- **Chrome Driver** or WebDriver of your choice.
- **TestNG** for test execution.

## 📦 Getting Started

To get started with this framework, follow the steps below:

### 1. Clone the Repository


git clone https://github.com/YOUR_USERNAME/selenium-extent-framework.git
cd selenium-extent-framework


### 2. Install Dependencies

If you haven’t installed Maven yet, you can download it from [here](https://maven.apache.org/download.cgi). If Maven is already installed, run the following to install the dependencies:


mvn clean install


## 🔧 Running Tests

You can run the tests with the following command:


mvn test


This will trigger TestNG to execute all the tests, and **ExtentReports** will generate an HTML report in the `test-output` directory.

## 🖥️ Test Report Location

After running the tests, you will find the **Extent Reports** HTML report in:


test-output/ExtentReport.html


You can open this file in any browser to view the detailed test execution report.

## 🖼️ Screenshots on Failure

If a test fails, a screenshot will be automatically captured and included in the **ExtentReports** HTML file.

The screenshots will be stored in:


test-output/screenshots/


## ⚙️ Project Structure

selenium-extent-framework/


├── pom.xml                # Maven dependencies

├── testng.xml             # TestNG configuration

└── src/
    ├── main/
    │   └── java/
    │       └── utils/     # Utility classes (ExtentManager, ScreenshotUtil, etc.)
    
    └── test/
        └── java/
            ├── base/      # BaseTest class for setup and teardown
            ├── pages/     # Page Object classes
            └── tests/     # Test classes
            

## 🛠️ Files & Classes

* **pom.xml**: Contains the Maven dependencies for TestNG, ExtentReports, and WebDriverManager.
* **testng.xml**: TestNG configuration file to define the suite of tests.
* **ExtentManager.java**: Manages the ExtentReports instance.
* **ExtentTestManager.java**: Manages the ExtentTest instances for each test.
* **ScreenshotUtil.java**: Utility class to capture screenshots on failure.
* **BaseTest.java**: Base test class that handles WebDriver setup and teardown.
* **LoginPage.java**: Page Object Model for the login page.
* **LoginTest.java**: Example test class for logging into a web application.

## 💡 Customizing the Framework

* **Add New Tests**: Create new classes under the `tests` directory and use the **Page Object Model** approach to organize your tests.
* **Extend Reporting**: Modify the `ExtentManager.java` to add custom logs, steps, and other details to your reports.
* **Add More Utilities**: Enhance the framework with additional utility methods for waiting, handling pop-ups, etc.

## 📝 Example of an Extent Report

After executing the tests, you can view detailed execution logs and screenshots in the **ExtentReports** HTML report, which provides:

* **Test pass/fail status**.
* **Test duration**.
* **Detailed logs** for each step.
* **Screenshots** attached to each failed test.

## 🔄 CI/CD Integration

This framework can easily be integrated into CI/CD pipelines such as **GitHub Actions**, **Jenkins**, or **Docker**. For GitHub Actions integration, see the example `.github/workflows/test.yml` file in the repository.

## 🧑‍💻 Contributing

If you would like to contribute to this project, feel free to fork the repository and submit a pull request with your changes.

## 🔑 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📬 Contact

* **GitHub**: 
* **Email**: 



### How to Add the README to Your GitHub Repository

1. Create a `README.md` file in the root of your project directory.
2. Copy the contents above into your `README.md` file.
3. Add, commit, and push the changes:


git add README.md

git commit -m "Added README for Selenium ExtentReports Framework"

git push origin main

 😊
