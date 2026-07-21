# Reviews PRD

Version: 1.0

---

# 1. Purpose

Reviews build trust between clients and professionals.

They help future clients make informed booking decisions while rewarding professionals who consistently deliver high-quality services.

Reviews are one of the primary trust signals used throughout Atlas.

---

# 2. Problem Statement

Clients often struggle to determine whether a professional is trustworthy.

Existing reviews are frequently:

- Spread across multiple platforms
- Outdated
- Easy to manipulate
- Missing photos
- Missing service context

Professionals also struggle because excellent work is not always reflected in their online reputation.

Atlas provides verified, service-based reviews directly linked to completed appointments.

---

# 3. Goals

Reviews should:

- Increase trust.
- Reward quality work.
- Help clients choose confidently.
- Improve marketplace transparency.
- Feed reliable signals into the Ranking System.

---

# 4. Non-Goals

Reviews are not intended to:

- Become a social discussion platform.
- Encourage popularity contests.
- Replace customer support.

Their responsibility is evaluating completed services.

---

# 5. User Stories

## Client

As a client I want to:

- Rate my experience.
- Write a review.
- Upload photos of the final result.
- Edit my review for a limited period.
- Read reviews before booking.
- Filter reviews by service.

## Professional

As a professional I want to:

- Build a trustworthy reputation.
- Respond to reviews.
- Learn from feedback.
- Showcase satisfied clients.

---

# 6. Functional Requirements

## Verified Reviews

Only clients with completed appointments may leave reviews.

Each review is linked to:

- Professional
- Service
- Appointment
- Date

---

## Rating

Clients provide:

- Overall rating (1–5 stars)
- Written feedback (optional)
- Photos (optional)

---

## Professional Response

Professionals may:

- Respond publicly
- Thank clients
- Clarify misunderstandings

Responses remain attached to the original review.

---

## Review Display

Reviews can be filtered by:

- Service
- Rating
- Most recent
- Most helpful
- With photos

---

## Moderation

Atlas supports:

- Reporting reviews
- Abuse detection
- Fraud detection
- Manual moderation

---

# 7. User Flow

Appointment completed

↓

Client receives review request

↓

Client submits rating and review

↓

Review appears on professional profile

↓

Review contributes to Ranking System

↓

Future clients use reviews when deciding to book

---

# 8. Success Metrics

Primary

- Review submission rate
- Average rating
- Profile trust score

Secondary

- Reviews with photos
- Professional response rate
- Review helpfulness votes
- Review-to-booking influence

---

# 9. Edge Cases

- Fake reviews
- Abusive language
- Duplicate reviews
- Review disputes
- Deleted bookings
- Professionals changing business names

---

# 10. Future Improvements

Potential enhancements:

- Verified photo badges
- Service-specific ratings
- AI review summaries
- Review translations
- Quality badges
- Repeat-client indicators
- Reputation insights
