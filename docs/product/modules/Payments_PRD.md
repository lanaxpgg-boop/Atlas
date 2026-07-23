# Payments PRD

Version: 1.0

---

# 1. Purpose

Payments enable secure, reliable, and transparent financial transactions between clients and professionals on Atlas.

Payments are a foundational platform capability that supports bookings today and future financial products such as Atlas Capital, Atlas Card, and supplier payments.

---

# 2. Problem Statement

Many independent beauty professionals currently accept payments through:

- Cash
- Bank transfer
- PayPal
- Venmo
- Cash App
- Revolut
- Card terminals
- Payment links

This fragmented experience creates friction for clients, weak financial records for professionals, and prevents Atlas from becoming the operating system of the business.

---

# 3. Goals

Payments should:

- Make paying simple.
- Increase completed bookings.
- Reduce payment disputes.
- Support refunds.
- Build transaction history.
- Create the financial foundation of Atlas.

---

# 4. Non-Goals

Payments are not intended to:

- Replace traditional banking.
- Offer lending in Version 1.
- Become a cryptocurrency platform.

Those capabilities may be introduced later.

---

# 5. User Stories

## Client

As a client I want to:

- Pay securely.
- Save payment methods.
- Receive receipts.
- Request refunds when appropriate.
- View payment history.

## Professional

As a professional I want to:

- Receive payments quickly.
- Track earnings.
- View transaction history.
- Handle refunds.
- Reduce unpaid appointments.

---

# 6. Functional Requirements

## Payment Methods

Supported methods:

- Credit cards
- Debit cards
- Apple Pay
- Google Pay

Future:

- PayPal
- Local payment methods
- Buy Now, Pay Later

---

## Payment Timing

Atlas supports:

- Pay after appointment
- Deposit before appointment
- Full prepayment

Each professional chooses their preferred policy.

---

## Refunds

Professionals may:

- Issue full refunds
- Issue partial refunds
- Reject refund requests according to policy

Atlas records all refund activity.

---

## Receipts

Clients receive:

- Digital receipts
- Payment confirmations
- Refund confirmations

Professionals receive:

- Transaction records
- Settlement reports

---

## Payment History

Users can view:

- Completed payments
- Pending payments
- Refunded payments
- Failed payments

---

## Security

Payments include:

- PCI-compliant processing
- Fraud detection
- Secure tokenization
- Encryption of sensitive data

Atlas does not store raw card details.

---

# 7. User Flow

Client books appointment

↓

Payment policy displayed

↓

Client completes payment (if required)

↓

Appointment confirmed

↓

Service completed

↓

Funds settled to professional

↓

Transaction added to payment history

---

# 8. Success Metrics

Primary

- Payment success rate
- Booking-to-payment conversion
- Settlement success rate

Secondary

- Refund rate
- Failed payment rate
- Average transaction value
- Payment method adoption

---

# 9. Edge Cases

- Failed payments
- Expired cards
- Chargebacks
- Partial refunds
- Cancelled bookings after payment
- Currency conversion
- Offline payment confirmation

---

# 10. Future Improvements

Potential enhancements:

- Atlas Wallet
- Instant payouts
- Split payments
- Tips
- Gift cards
- Subscription billing
- Multi-currency support
- Invoice generation
