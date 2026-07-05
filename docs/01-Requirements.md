# Requirements

## Project Summary
A Laravel-based voucher purchase system for a car wash business. The system allows customers to view car wash coupon offers, purchase a voucher online, and receive confirmation after payment.

## Main User Flow
1. Customer opens coupon page.
2. Customer selects an offer.
3. Customer enters name and email.
4. Customer pays online.
5. Customer receives voucher confirmation.
6. Owner/admin sees the order.
7. Owner/admin can mark voucher as redeemed.

## MVP Features
- Public coupon/offers page
- Offer details
- Checkout/payment flow
- Success page
- Cancel/failed payment page
- Voucher code generation
- Customer email confirmation
- Admin login
- Admin order list
- Mark voucher as redeemed
- Multi-language support: German and English
- German as the default language
- Language switcher on the public coupon page

## Out of Scope for MVP
- Appointment booking
- Customer accounts
- Promo codes
- Reviews
- QR code voucher
- Advanced reports

## Open Questions
- Which payment provider will the client use? Stripe or PayPal?
- Does the voucher expire?
- Can one customer buy multiple vouchers?
- Does the owner need a printable voucher?
- What exact offers/prices should be displayed?
- Who will provide the German translation?
- Should the admin dashboard also be bilingual, or only the public customer pages?
- Should voucher emails be sent in German, English, or based on the selected language?