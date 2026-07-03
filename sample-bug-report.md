# Sample Bug Report

## Bug Title

Checkout button is not clickable after adding product to cart

## Environment

| Field | Value |
|---|---|
| Application | Demo E-commerce App |
| Browser | Chrome |
| OS | Windows 11 |
| Test Type | UI Regression |
| Automation Tool | Playwright |

## Severity

High

## Priority

P1

## Preconditions

- User account exists
- User is logged in
- Product is available in inventory

## Steps to Reproduce

1. Open the application.
2. Login with a valid user account.
3. Search for an available product.
4. Add the product to cart.
5. Open the cart page.
6. Click the checkout button.

## Expected Result

The user should be redirected to the checkout page.

## Actual Result

The checkout button does not respond when clicked. No navigation occurs.

## Evidence

- Screenshot attached in report
- Playwright trace available
- Console logs checked

## Business Impact

Users may be blocked from completing purchases, which can directly affect revenue.

## Suggested Investigation

- Check whether the checkout button is disabled by frontend state.
- Verify cart API response after product addition.
- Check JavaScript console errors.
- Validate locator stability and button visibility.
