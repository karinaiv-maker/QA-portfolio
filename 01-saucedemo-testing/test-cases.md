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

## TC-004: Remove product from cart

**Preconditions:**
- User is logged in.
- A product is added to the cart.
- User is on the Cart page.

**Steps:**
1. Locate the product in the cart.
2. Click the "Remove" button.

**Expected Result:**
- The product is removed from the cart.
- The cart badge is updated accordingly.
- The removed product is no longer displayed in the cart.

**Actual Result:**
- The product was successfully removed from the cart.
- The cart badge was updated and disappeared.
- The cart was empty after removing the product.

**Status:**
- Pass

- ## TC-005: Sort products by name from A to Z

**Preconditions:**
- User is logged in.
- Products page is displayed.

**Steps:**
1. Open the sorting dropdown.
2. Select "Name (A to Z)".

**Expected Result:**
- Products are displayed in ascending alphabetical order by product name.

**Actual Result:**
- Products were displayed in ascending alphabetical order by product name.

**Status:**
- Pass

- ## TC-006: Sort products by name from Z to A

**Preconditions:**
- User is logged in.
- Products page is displayed.

**Steps:**
1. Open the sorting dropdown.
2. Select "Name (Z to A)".

**Expected Result:**
- Products are displayed in descending alphabetical order by product name.

**Actual Result:**
- Products were displayed in descending alphabetical order by product name.

**Status:**
- Pass

- ## TC-007: Sort products by price from low to high

**Preconditions:**
- User is logged in.
- Products page is displayed.

**Steps:**
1. Open the sorting dropdown.
2. Select "Price (low to high)".

**Expected Result:**
- Products are displayed in ascending order by price, from the lowest to the highest.

**Actual Result:**
- Products were displayed in ascending order by price, from the lowest to the highest.

**Status:**
- Pass

- ## TC-008: Sort products by price from high to low

**Preconditions:**
- User is logged in.
- Products page is displayed.

**Steps:**
1. Open the sorting dropdown.
2. Select "Price (high to low)".

**Expected Result:**
- Products are displayed in descending order by price, from the highest to the lowest.

**Actual Result:**
- Products were displayed in descending order by price, from the highest to the lowest.

**Status:**
- Pass
