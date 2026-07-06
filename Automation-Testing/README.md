# Selenium Data-Driven Testing (DDT) Automation Framework

## Project Overview

This project is a Selenium-based Data-Driven Testing (DDT) Automation Framework developed using Python. It automates the user registration process by reading test data from an Excel file, executing the test cases, validating the application responses, updating the test results back into Excel, and capturing screenshots for failed test cases.

The framework is designed to minimize manual testing effort and improve test execution efficiency.

---

## Features

- Data-Driven Testing using Excel
- Selenium WebDriver Automation
- Automatic Result Validation
- PASS/FAIL Status Update in Excel
- Screenshot Capture for Failed Test Cases
- Exception Handling
- Explicit Wait Implementation
- Reusable Screenshot Function
- Easy Test Data Maintenance

---

## Project Structure

```
TichiAutomation/
│
├── data/
│   └── Automation_testing_ddt_data.xlsx
│
├── test_login_ddt.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Technologies Used

- Python 3.x
- Selenium
- OpenPyXL
- Google Chrome
- ChromeDriver

---

## Prerequisites

Before running the project, install:

- Python 3.10 or later
- Google Chrome Browser
- ChromeDriver compatible with your Chrome version

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/TichiAutomation.git
```

Move into the project directory

```bash
cd TichiAutomation
```

Install all dependencies

```bash
pip install -r requirements.txt
```

---

## Test Data

The framework reads test data from

```
data/Automation_testing_ddt_data.xlsx
```

The Excel sheet contains:

| Column | Description                             |
| ------ | --------------------------------------- |
| A      | First Name                              |
| B      | Last Name                               |
| C      | Phone Number                            |
| D      | Email                                   |
| E      | Password                                |
| F      | Confirm Password                        |
| G      | Expected Result                         |
| H      | Actual Result (Generated Automatically) |
| I      | Status (PASS/FAIL)                      |

---

## Running the Project

Execute the automation script

```bash
python test_login_ddt.py
```

---

## Framework Workflow

1. Open Application
2. Click Sign In
3. Enter Email
4. Continue to Registration
5. Fill Registration Form
6. Submit Form
7. Validate Response
8. Update Excel
9. Capture Screenshot if Failed
10. Repeat for All Test Data

---

## Output

After execution:

- Excel sheet is updated automatically.
- PASS/FAIL status is generated.
- Actual results are written into Excel.
- Failed test cases are stored inside the screenshots folder.

---

## Exception Handling

The framework handles:

- TimeoutException
- InvalidSessionIdException
- Unexpected Exceptions

---

## Future Enhancements

- PyTest Integration
- HTML Reports
- Allure Reports
- Logging
- Parallel Execution
- Cross Browser Testing
- Jenkins CI/CD Integration

---

## Author

Akshay B

Department of Artificial Intelligence and Data Science

Automation Testing Project

---

## License

This project is developed for educational and learning purposes.
