# Atlas Database & Data Model

Version: 1.0

---

# 1. Purpose

This document defines the core data model of Atlas.

It specifies:

- Core entities
- Relationships
- Ownership
- Data boundaries

This document is the foundation for database design, backend APIs, and future scaling.

---

# 2. Design Principles

Atlas follows these rules:

1. Every entity has a single owner.
2. IDs are immutable.
3. Soft deletes are preferred over hard deletes where business data must be retained.
4. Auditability is required for sensitive operations.
5. Personally identifiable information (PII) is isolated where practical and protected.
6. Business logic lives in services, not in the database schema.

---

# 3. Core Entities

## Identity

- User
- Professional Profile
- Verification
- Session
- Device

---

## Marketplace

- Post
- Story
- Collection
- Saved Item
- Follow

---

## Booking

- Booking
- Availability Slot
- Calendar Event
- Service
- Cancellation

---

## Payments

- Payment
- Refund
- Payout
- Transaction
- Escrow Hold (planned)

---

## Communication

- Conversation
- Message
- Notification

---

## Reputation

- Review
- Rating
- Report
- Dispute

---

## Business

- Analytics Snapshot
- Dashboard Metrics
- Earnings

---

## Administration

- Admin User
- Audit Log
- Moderation Action

---

# 4. High-Level Relationships

User
 ├── Professional Profile (optional)
 ├── Bookings
 ├── Reviews
 ├── Messages
 ├── Saved Items
 └── Notifications

Professional
 ├── Services
 ├── Posts
 ├── Availability
 ├── Calendar
 ├── Earnings
 ├── Reviews
 └── Verification

Booking
 ├── Payment
 ├── Client
 ├── Professional
 ├── Service
 ├── Calendar Event
 ├── Review
 └── Dispute

Payment
 ├── Booking
 ├── Refund
 ├── Payout
 └── Escrow Hold (future)

Post
 ├── Media
 ├── Likes
 ├── Comments
 ├── Saves
 └── Professional

Conversation
 ├── Participants
 └── Messages

## 5. Ownership Rules

| Entity | Owner Service |
|----------|--------------|
| User | Authentication |
| Professional | Profiles |
| Booking | Booking |
| Payment | Payments |
| Review | Reviews |
| Post | Feed |
| Message | Messaging |
| Notification | Notifications |
| Report | Trust & Safety |
| Dispute | Trust & Safety |

---

## 6. Global Fields

Every major entity should include standardized metadata where appropriate.

```text
id
created_at
updated_at
created_by
status
version
```

This improves consistency across all services and simplifies auditing, debugging, and future migrations.

---

## 7. Data Lifecycle

Every entity follows a predictable lifecycle.

```text
Created
   ↓
Updated
   ↓
Archived (when applicable)
   ↓
Soft Deleted (where supported)
   ↓
Retention Policy
```

Not every entity requires every lifecycle stage, but all services should follow the same lifecycle philosophy whenever applicable.

---

## 8. Scalability Principles

Atlas follows these scalability principles:

- Separate read-heavy and write-heavy workloads where appropriate.
- Support future service decomposition without changing entity ownership.
- Avoid cross-service database writes.
- Prefer asynchronous communication for non-critical updates.
- Design entities to support horizontal scaling.
- Keep business logic outside the database schema.

---

## 9. Future Expansion

The data model is intentionally designed to support future Atlas products without redesigning existing ownership boundaries.

Future entities may include:

- Atlas Capital
- Atlas Card
- Atlas Supply
- Atlas Ads
- Atlas Academy
- Atlas API

---

## 10. Success Criteria

A new engineer should be be able to determine:

- where data belongs,
- which service owns it,
- how it relates to other entities,
- how changes propagate through the platform.

The document should remain the single source of truth for Atlas core data ownership.

---

# Appendix A

Detailed Entity Relationship Diagrams (ERD) will be maintained in separate documentation and updated alongside implementation.

This document defines concepts and ownership.

The ER diagrams define physical relationships.
