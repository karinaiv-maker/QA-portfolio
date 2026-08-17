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

## TC-009: Complete checkout with valid information

**Preconditions:**
- User is logged in.
- A product is added to the cart.

**Test Data:**
- First Name: Test
- Last Name: User
- ZIP/Postal Code: 4000

**Steps:**
1. Open the cart.
2. Click the "Checkout" button.
3. Enter a valid first name.
4. Enter a valid last name.
5. Enter a valid ZIP/Postal Code.
6. Click the "Continue" button.
7. Review the order information.
8. Click the "Finish" button.

**Expected Result:**
- Checkout information is accepted.
- Order overview is displayed with the selected product and price information.
- The order is completed successfully.
- An order confirmation message is displayed.

**Actual Result:**
- Checkout information was accepted successfully.
- Order overview displayed the correct product and price information.
- The order was completed successfully.
- Confirmation message "Thank you for your order!" was displayed.

**Status:**
- Pass

- ## TC-010: Checkout with empty required fields

**Preconditions:**
- User is logged in.
- A product is added to the cart.
- User is on the Checkout: Your Information page.

**Steps:**
1. Leave First Name empty.
2. Leave Last Name empty.
3. Leave ZIP/Postal Code empty.
4. Click the "Continue" button.

**Expected Result:**
- User is not allowed to continue to the Checkout Overview page.
- An error message for the required First Name field is displayed.

**Actual Result:**
- User was not allowed to continue to the Checkout Overview page.
- Error message "Error: First Name is required" was displayed.

**Status:**
- Pass

## TC-011: Checkout with empty Last Name

**Preconditions:**
- User is logged in.
- A product is added to the cart.
- User is on the Checkout: Your Information page.

**Test Data:**
- First Name: Test
- Last Name: [empty]
- ZIP/Postal Code: 4000

**Steps:**
1. Enter a valid First Name.
2. Leave the Last Name field empty.
3. Enter a valid ZIP/Postal Code.
4. Click the "Continue" button.

**Expected Result:**
- User is not allowed to continue to the Checkout Overview page.
- An error message for the required Last Name field is displayed.

**Actual Result:**
- User was not allowed to continue to the Checkout Overview page.
- Error message "Error: Last Name is required" was displayed.

**Status:**
- Pass

- ## TC-012: Checkout with empty ZIP/Postal Code

**Preconditions:**
- User is logged in.
- A product is added to the cart.
- User is on the Checkout: Your Information page.

**Test Data:**
- First Name: Test
- Last Name: User
- ZIP/Postal Code: [empty]

**Steps:**
1. Enter a valid First Name.
2. Enter a valid Last Name.
3. Leave the ZIP/Postal Code field empty.
4. Click the "Continue" button.

**Expected Result:**
- User is not allowed to continue to the Checkout Overview page.
- An error message for the required ZIP/Postal Code field is displayed.

**Actual Result:**
- User was not allowed to continue to the Checkout Overview page.
- Error message "Error: Postal Code is required" was displayed.

**Status:**
- Pass

- ## TC-013: Logout from the application

**Preconditions:**
- User is logged in.
- Products page is displayed.

**Steps:**
1. Open the navigation menu.
2. Click the "Logout" option.

**Expected Result:**
- User is successfully logged out.
- User is redirected to the SauceDemo Login page.

**Actual Result:**
- User was successfully logged out.
- User was redirected to the SauceDemo Login page.

**Status:**
- Pass

- ## TC-014: Reset App State after adding a product to the cart

**Preconditions:**
- User is logged in.
- Products page is displayed.
- The application is in its initial state.

**Steps:**
1. Add a product to the cart.
2. Verify that the product button changes from "Add to cart" to "Remove".
3. Open the navigation menu.
4. Click "Reset App State".
5. Close the navigation menu.
6. Check the cart.
7. Check the button of the previously added product on the Products page.

**Expected Result:**
- The cart is cleared.
- The cart badge disappears.
- The product button returns from "Remove" to "Add to cart".
**Actual Result:**
- Reset App State cleared the product from the cart.
- The cart badge disappeared.
- The previously added product still displayed the "Remove" button instead of "Add to cart".

**Status:**
- Fail
