# Automation Framework - RestAssured API Testing

This repository contains an automation framework for testing REST APIs using **RestAssured** and **TestNG** in Java. The framework performs functional tests on the **Restful Booker API** and includes positive and negative test cases for booking creation and retrieval.

## Project Overview

The framework consists of:
- **API Tests**: Automated tests for the booking API, including creating a booking and retrieving a booking by ID.
- **Negative Test Cases**: Tests to handle errors like missing fields or non-existent booking IDs.
- **Reporting**: TestNG reports in HTML format generated after running the tests.

## Prerequisites

- **Java**
- **Maven**: For managing dependencies and running tests.
- **Git**: To clone the repository.
- **IDE**: Preferably IntelliJ IDEA or Eclipse.

## Setup Instructions

1. **Clone the repository**:
   Clone this repository to your local machine using the following command:
   git clone https://github.com/Pawan9096/Automation_Framework
   Navigate to the project folder: Change directory to the cloned repository folder.

cd Automation_Framework
Install dependencies: This project uses Maven for dependency management. Run the following command to download all dependencies:

mvn install
Configure your IDE (Optional): If you're using an IDE like IntelliJ IDEA or Eclipse, you can import the project directly as a Maven project to ensure all dependencies are managed.

Running Tests
Run the tests using Maven: You can execute the tests with Maven by running the following command:

mvn test
TestNG Report: After the tests are executed, TestNG generates an HTML report. You can find the report under the target/surefire-reports directory.

Run Tests from IDE: If you're using an IDE, you can also run the tests directly from there by right-clicking the test classes and selecting the option to run them with TestNG.

Framework Details
Test Cases:
Positive Test Cases:

Add a new booking: Sends a POST request to create a booking and validates the response.
Get a booking by ID: Sends a GET request to retrieve a booking by its ID and validates the data.
Negative Test Cases:

Add booking with missing fields: Tests how the API responds when mandatory fields are missing.
Get booking with invalid ID: Tests how the API responds to a non-existent booking ID.
Test Framework:
RestAssured: For making HTTP requests and validating API responses.
TestNG: For test execution and report generation.
Maven: For dependency management and build automation.
Directory Structure
src/
 └── test/
     └── java/
         └── com/
             └── automation/
                 ├── BookingTest.java       # Test for adding a booking
                 ├── GetBookingTest.java    # Test for getting a booking by ID
                 └── NegativeTest.java      # Negative test cases
     └── resources/
         └── testng.xml                 # TestNG configuration (optional)


