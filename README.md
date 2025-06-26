# CucumberSample

This project automates the login and logout scenarios on [Automation Exercise](http://automationexercise.com) using **Cucumber**, **Selenium WebDriver**, and **Java**. It validates successful login, error handling for invalid credentials, and proper logout functionality.

## 📌 Project Overview

This automation suite covers the following test scenarios:

1. ✅ **Login with valid credentials**  
2. ❌ **Login with invalid credentials**  
3. 🔁 **Login and Logout flow verification**

# Feauture file using gherkin language.
**Feature: User Login and Logout Functionality**

  Scenario: Login User with correct email and password
   
    Given I should see the home page is visible
    And I click on the Signup Login button
    Then I should see 'Login to your account'
    When I enter correct email address "shubhamtesting12345@gmail.com" and password "Shubham@12345"
    And I click the login button
    Then I should see Logged in as username
    Then Close the browser

  Scenario: Login User with correct email and password
   
    Given I should see the home page is visible
    And I click on the Signup Login button
    Then I should see 'Login to your account'
    When I enter incorrect email address "wrongemail@Testing.com" and password "EnteredWrongPassword"
    And I click the login button
    Then I should see error message 'Your email or password is incorrect!'
    Then Close the browser

    Scenario: Verify user can log in and log out successfully
    
    Given I should see the home page is visible
    And I click on the Signup Login button
    Then I should see 'Login to your account'
    When I enter correct email address "shubhamtesting12345@gmail.com" and password "Shubham@12345"
    And I click the login button
    Then I should see Logged in as username
    When I click on the Logout button
    Then I should be navigated to the login page
    Then Close the browser



    
    
