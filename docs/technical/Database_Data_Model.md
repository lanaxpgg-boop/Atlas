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
