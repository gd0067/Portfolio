# 📄 DEF-602-SauceDemo-Checkout-Missing-Fields-Error.md

## Summary  
When a user attempts to proceed through the checkout flow without entering any information into the mandatory fields (First Name, Last Name, and Postal Code), the system only returns an error message for the First Name field, rather than aggregating all missing field errors.

## Related Test Case  
TC-CO-005 – Verify Checkout Validation Messages

## Steps to reproduce  
1. Navigate to https://www.saucedemo.com/ 
2. Log in using the credentials `standard_user` or `error_user`.  
3. Add at least one item to the cart and navigate to the Cart page.
4. Click the "Checkout" button.
5. Leave the First Name, Last Name, and Postal Code fields blank.
6. Click the "Continue" button.  

## Expected Result  
The system should display a comprehensive error message indicating all missing mandatory fields: "Error: First Name, Last Name and Postal Code are required".

## Actual Result  
The system only displays the error message: "Error: First Name is required".

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
Web, Checkout, Form Validation

## Affected version  
v1.0.0