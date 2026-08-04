# Test Cases – SauceDemo

## TC-001: Login with valid credentials

**Preconditions:**
- User is on the SauceDemo login page.

**Test Data:**
- Username: standard_user
- Password: secret_sauce

**Steps:**
1. Enter a valid username.
2. Enter a valid password.
3. Click the Login button.

**Expected Result:**
- User is successfully logged in.
- Products page is displayed.

**Actual Result:**
- - User was successfully logged in and redirected to the Products page.

**Status:**
- Pass
## TC-002: Login with invalid password

**Preconditions:**
- User is on the SauceDemo login page.

**Test Data:**
- Username: standard_user
- Password: wrong_password

**Steps:**
1. Enter a valid username.
2. Enter an invalid password.
3. Click the Login button.

**Expected Result:**
- User is not logged in.
- An error message is displayed.

**Actual Result:**
- - User was not logged in.
- Error message "Epic sadface: Username and password do not match any user in this service" was displayed.

**Status:**
- Pass
- ## TC-003: Add product to cart

**Preconditions:**
- User is logged in.
- Products page is displayed.

**Steps:**
1. Select a product.
2. Click the "Add to cart" button.
3. Open the cart.

**Expected Result:**
- The selected product is added to the cart.
- The cart badge is updated.
- The correct product is displayed in the cart.

**Actual Result:**
- - Sauce Labs Backpack was successfully added to the cart.
- The cart badge displayed "1".
- The correct product and product information were displayed in the cart.


**Status:**
- Pass
