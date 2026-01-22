# Phase 1: Manual Test Case Baseline (The Traditional Way)

**Objective:** To establish a baseline of test cases designed manually. This includes Positive (Happy Path) and Negative (Boundary/Error) testing.

| TC-ID | Title | Test Steps | Expected Result |
|-------|-------|------------|-----------------|
| 001 | Guest Checkout Flow | 1. Add item to cart <br> 2. Select 'Checkout as Guest' <br> 3. Enter shipping & payment <br> 4. Click 'Place Order' | Order is successful; User is NOT prompted to log in; Confirmation email sent. |
| 002a | Free Shipping Threshold (Positive) | 1. Add items totaling $105 to cart <br> 2. Proceed to shipping section | Shipping cost displays as $0.00. |
| 002b | Shipping Fee < $100 (Negative) | 1. Add items totaling $50 to cart <br> 2. Proceed to shipping section | Shipping cost displays as $10.00. |
| 003a | International Shipping (Boundary) | 1. Enter shipping address in USA/UK <br> 2. Calculate shipping | Shipping cost displays as $25.00. |
| 003b | Domestic Shipping (Canada) | 1. Enter shipping address in Ontario, Canada <br> 2. Calculate shipping | Shipping cost reflects domestic rate ($0 or $10 based on total). |
| 004 | Credit Card Validation (Expired) | 1. Enter valid CC number <br> 2. Enter expired date (e.g., 01/2024) <br> 3. Submit payment | System displays "Card Expired" error; Order is not processed. |
| 005 | Tax Calculation (HST) | 1. Set shipping address to Ontario <br> 2. Review order summary | Total reflects 13% HST on the subtotal. |
