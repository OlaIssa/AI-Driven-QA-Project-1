# Case Study: E-Commerce Checkout System

## Project Overview
A web-based checkout system for a premium electronics retailer. The goal is to ensure a bug-free experience for high-value transactions.

## Functional Requirements
1. **Cart Validation:** Users must be able to review items, quantities, and prices before proceeding.
2. **Guest vs. Registered Checkout:** System must allow guest checkout but prompt for account creation.
3. **Shipping Logic:** 
   - Free shipping for orders over $100.
   - Standard shipping ($10) for orders under $100.
   - International shipping ($25) for addresses outside Canada.
4. **Payment Processing:** 
   - Must support Credit Card (Visa, Mastercard) and PayPal.
   - Must validate expiry dates and CVV.
5. **Order Summary:** Final total must include Tax (HST/GST based on province).

## Constraints
- Payment must be processed within 30 seconds.
- User must receive an email confirmation immediately upon success.
