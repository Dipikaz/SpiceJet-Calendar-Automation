SpiceJet Calendar Automation ✈️

Overview

This project contains a Java-based Selenium automation script designed to interact with the SpiceJet website. The primary function of this script is to automate the process of selecting a departure date from the flight search calendar. It demonstrates how to handle dynamic web elements, calendar pop-ups, and SVG elements using Selenium WebDriver.

Features ✨

Browser Launch: Opens a new instance of Google Chrome in maximized mode.
Site Navigation: Navigates to the official SpiceJet website (https://www.spicejet.com/).
Form Input: Automatically enters departure ("From") and destination ("To") city codes.
Calendar Interaction:
Opens the date picker calendar.
Navigates to a future month (specifically, two months from the current date).
Selects a specific day (the 9th) of that month.
Explicit Waits: Uses WebDriverWait to ensure page elements are loaded and intractable before performing actions, improving script reliability.

Tech Stack 🛠️

Language: Java

Automation Framework: Selenium WebDriver

Browser Driver: ChromeDriver

Build Tool (optional): Maven or Gradle

IDE: Eclipse, IntelliJ IDEA, or VS Code

Table of Contents

1. Project Structure

2. Prerequisites

3. Installation

4. Expected Outcome

Project Structure

The project consists of a single Java class:

src

   └── com

       └── SpiceJet

            └── SpiceJetCalenderAutomation.java


Prerequisites

1. Before you begin, ensure you have the following installed on your system:

2. Java Development Kit (JDK): Version 8 or higher.

3. Selenium WebDriver: Java client library.

4. ChromeDriver: The version must correspond to your installed Google Chrome browser version.

5. An IDE (optional but recommended): Such as Eclipse, IntelliJ IDEA, or VS Code with Java extensions.

Installation

1. Follow these steps to set up and run the project:
Clone the repository (or download the SpiceJetCalenderAutomation.java file).
git clone <your-repository-url>

2. Set up your Java Project:
Open your IDE and create a new Java project.
Place SpiceJetCalenderAutomation.java into the appropriate package structure (com.SpiceJet).

3. Add Dependencies:
Add the Selenium WebDriver JAR files to your project's build path. If you are using a build tool like Maven, add the following dependency to your pom.xml:
<dependency>
    <groupId>org.seleniumhq.selenium</groupId>
    <artifactId>selenium-java</artifactId>
    <version>4.22.0</version> </dependency>

4. Configure ChromeDriver:

Download the ChromeDriver executable that matches your Chrome browser version.
Ensure the path to chromedriver.exe is included in your system's PATH environment variable. Alternatively, you can specify its path directly in the code using System.setProperty("webdriver.chrome.driver", "path/to/chromedriver.exe");.


5. Run the Script:

Execute the main method in the SpiceJetCalenderAutomation.java class.

Expected Outcome

1. When the script is executed successfully, you will observe the following automated actions:

2. A new Google Chrome window opens and maximizes.

3. The browser navigates to https://www.spicejet.com/.

4. The script waits for the "From" and "To" fields to be visible and enters "Mum" and "Pun" respectively.

5. The departure date calendar is clicked and becomes visible.

6. Based on the current date of July 2025, the script clicks the "next month" button to navigate to September 2025.

7. Finally, it selects the 9th day of that future month, and the script finishes its execution.


