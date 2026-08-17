# Bug Reports – SauceDemo

## BUG-001: Product button remains "Remove" after Reset App State

**Environment:**
- Application: SauceDemo
- Browser: Safari
- Operating System: macOS

**Preconditions:**
- User is logged in.
- Products page is displayed.
- Cart is empty.

**Steps to Reproduce:**
1. Add "Sauce Labs Backpack" to the cart.
2. Verify that the cart badge displays "1".
3. Verify that the product button changes from "Add to cart" to "Remove".
4. Open the navigation menu.
5. Click "Reset App State".
6. Close the navigation menu.
7. Check the cart badge.
8. Check the button for "Sauce Labs Backpack".

**Expected Result:**
- The cart is cleared.
- The cart badge disappears.
- The product button returns to "Add to cart".

**Actual Result:**
- The cart is cleared and the cart badge disappears.
- The "Sauce Labs Backpack" button incorrectly remains "Remove".

**Severity:**
- Minor

**Priority:**
- Medium

**Reproducibility:**
- 100% (reproduced multiple times)

**Related Test Case:**
- TC-014 – Reset App State after adding a product to the cart

**Status:**
- Open
