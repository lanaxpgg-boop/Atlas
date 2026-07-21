# Ranking System PRD

Version: 1.0

---

# 1. Purpose

The Atlas Ranking System determines which content, professionals, and search results are shown to users.

Its purpose is to maximize successful matches between clients and professionals by ranking results based on relevance, trust, quality, and intent.

Ranking is a core platform capability used across the Feed, Search, Discovery, and Recommendations.

---

# 2. Problem Statement

Clients are overwhelmed by choice and fragmented information.

Showing every post or every professional in chronological order produces poor results.

Professionals also need a fair opportunity to be discovered.

Atlas requires a ranking system that balances personalization, trust, quality, and marketplace health.

---

# 3. Goals

The ranking system should:

- Show the most relevant professionals.
- Match user intent.
- Reward quality work.
- Reward trust.
- Promote healthy local marketplaces.
- Give new professionals a fair opportunity to be discovered.
- Increase successful bookings.

---

# 4. Non-Goals

The ranking system is not designed to:

- Maximize time spent in the app.
- Reward clickbait.
- Reward fake engagement.
- Prioritize paid promotion over relevance.
- Create "winner takes all" visibility.

---

# 5. User Stories

## Client

As a client I want to:

- See professionals that match my style.
- Discover nearby professionals.
- Trust the recommendations.
- Find available professionals quickly.

## Professional

As a professional I want to:

- Be rewarded for high-quality work.
- Have a chance to grow even if I'm new.
- Know that rankings are based on merit rather than follower count.

---

# 6. Ranking Signals

Atlas combines multiple categories of signals.

## Relevance

- Style match
- Service match
- Search intent
- Category
- Saved preferences

---

## Location

- Distance
- City
- Neighborhood
- Service area

---

## Trust

- Reviews
- Rating quality
- Portfolio quality
- Verification status
- Profile completeness

---

## Activity

- Recent posts
- Recent bookings
- Response speed
- Calendar freshness

---

## Quality

- Save rate
- Profile visits
- Booking conversion
- Repeat bookings
- Client satisfaction

---

## Personalization

- Saved posts
- Previous bookings
- Followed professionals
- Preferred styles

---

## Marketplace Health

- Diversity of professionals
- New professional exposure
- Geographic balance
- Category balance

---

# 7. User Flow

User opens Feed or Search

↓

Intent is identified

↓

Eligible content and professionals are retrieved

↓

Ranking signals are evaluated

↓

Results are scored

↓

Results displayed

↓

User interactions become future ranking signals

---

# 8. Success Metrics

Primary:

- Search → Profile conversion
- Feed → Profile conversion
- Profile → Booking conversion

Secondary:

- Save rate
- Repeat bookings
- Client satisfaction
- Professional retention

---

# 9. Edge Cases

- Cold-start users
- Cold-start professionals
- Fake reviews
- Fake engagement
- Purchased followers
- Spam
- Duplicate portfolios
- Seasonal demand spikes

---

# 10. Future Improvements

Potential future capabilities:

- AI style recognition
- Visual similarity search
- Context-aware ranking
- Demand prediction
- Availability prediction
- Real-time ranking optimization
