# 📄 DEF-603-SauceDemo-Checkout-Postal-Code-Format.md

## Summary  
During the checkout process, the "Postal Code" field accepts alphabetic characters and strings instead of restricting input to numeric values or alphanumeric postal code formats. The user is allowed to proceed to the next checkout step with invalid data.

## Related Test Case  
TC-CO-009 – Verify Postal Code Input Formatting

## Steps to reproduce  
1. Navigate to https://www.saucedemo.com/ 
2. Log in using valid credentials.  
3. Add at least one item to the cart and proceed to Checkout by clicking the checkout button.
4. Input valid data for "First Name" and "Last Name".
5. Input an alphabetic string into the "Postal Code" field.
6. Click the "Continue" button.  

## Expected Result  
The system should prevent progression and display an error message stating "Error: Invalid Input: Postal Code must be a number".

## Actual Result  
The error message does not appear, and the system incorrectly navigates the user to the checkout-step-one page.

## Priority  
🟡 Low  

## Severity  
Medium  

## Status  
Open  

## Environment  
- Platform: Web App (saucedemo.com)  
- Browser: Chrome 116  
- OS: Windows 11  

## Labels  
Web, Checkout, Data Validation

## Affected version  
v1.0.0