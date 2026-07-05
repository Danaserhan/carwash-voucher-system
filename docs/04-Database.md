# Database Design

## Tables

### offers
- id
- public_id
- title_en
- title_de
- description_en
- description_de
- original_price
- sale_price
- image_path
- start_date
- end_date
- is_active
- created_at
- updated_at
- deleted_at

### orders
- id
- public_id
- order_number
- offer_id
- offer_title_en
- offer_title_de
- customer_name
- customer_email
- quantity
- unit_price
- total_amount
- payment_status
- stripe_session_id
- stripe_payment_intent_id
- voucher_code
- paid_at
- redeemed_at
- created_at
- updated_at
- deleted_at

## Relationships

- Offer has many Orders.
- Order belongs to Offer.

## Payment Status Values

- pending
- paid
- failed
- cancelled
- refunded

## Business Rules

- Public IDs must be unique.
- Order numbers must be unique.
- Voucher codes must be unique.
- Quantity must be at least 1.
- Sale price cannot be greater than original price.
- Expired offers cannot be purchased.
- Inactive offers cannot be purchased.
- Orders are marked as paid only after Stripe webhook confirmation.
- Redeemed vouchers cannot be redeemed again.
- Old orders must keep the offer title and price from the purchase time.