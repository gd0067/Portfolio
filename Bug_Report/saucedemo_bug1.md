# 📄 DEF-601-SauceDemo-Broken-Product-Images.md

## Summary  
When logging into the Swag Labs application as a "problem user", all product images on the inventory page fail to load and instead display an identical placeholder dog image. 

## Related Test Case  
TC-UI-045 – Verify Product Catalog Image Rendering

## Steps to reproduce  
1. Navigate to https://www.saucedemo.com/  
2. Enter the username: `problem_user`  
3. Enter the password: `secret_sauce`  
4. Click the "Login" button.  
5. Observe the product images on the `/inventory.html` page.

## Expected Result  
Each product card should display its unique, corresponding product image (e.g., a backpack image for the Sauce Labs Backpack).

## Actual Result  
Every product card displays the same incorrect fallback image (a dog file named `sl-404.jpg`). The correct product image URLs are not being fetched.

## Priority  
🔴 High  

## Severity  
Major  

## Status  
Open  

## Environment  
- Platform: Web App (saucedemo.com)  
- Browser: Chrome 116  
- OS: Windows 11  

## Labels  
UI, Frontend, Assets, Product Catalog  

## Affected version  
v1.0.0 (Problem User Profile)