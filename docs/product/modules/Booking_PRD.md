# Booking PRD

Version: 1.0

---

# 1. Purpose

Booking is the core transaction system of Atlas.

Its purpose is to make scheduling beauty appointments fast, reliable, transparent, and stress-free for both clients and professionals.

Every successful booking strengthens trust in the platform.

---

# 2. Problem Statement

Booking beauty appointments today is often fragmented.

Clients frequently:

- Send direct messages
- Wait for replies
- Ask for available times
- Negotiate appointments manually
- Forget appointments
- Receive late confirmations

Professionals spend valuable time managing conversations instead of serving clients.

Atlas replaces manual coordination with a structured booking workflow.

---

# 3. Goals

Booking should:

- Reduce booking friction.
- Show real availability.
- Prevent double bookings.
- Minimize cancellations.
- Increase completed appointments.
- Encourage repeat bookings.

---

# 4. Non-Goals

Booking is not intended to:

- Replace professional consultation when required.
- Replace messaging for complex requests.
- Handle every business workflow in Version 1.

Its primary responsibility is appointment management.

---

# 5. User Stories

## Client

As a client I want to:

- View available appointment slots.
- Choose a service.
- Select a date and time.
- Add notes or inspiration photos.
- Receive confirmation.
- Receive reminders.
- Cancel or reschedule when allowed.
- Rebook previous appointments easily.

## Professional

As a professional I want to:

- Control my availability.
- Prevent scheduling conflicts.
- Confirm appointments.
- Manage cancellations.
- View my upcoming schedule.
- Block unavailable time.
- Receive booking notifications.

---

# 6. Functional Requirements

## Appointment Creation

Clients can:

- Select a professional
- Select a service
- Choose date
- Choose available time
- Add appointment notes
- Upload reference images (future)
- Confirm booking

---

## Calendar

Professionals can:

- Define working hours
- Add breaks
- Block vacation days
- Block personal time
- Set appointment duration
- Configure booking rules

---

## Booking Status

Possible statuses:

- Draft
- Pending Confirmation
- Confirmed
- Rescheduled
- Cancelled
- Completed
- No Show

---

## Notifications

Clients receive:

- Booking confirmation
- Reminder notifications
- Schedule changes
- Cancellation updates

Professionals receive:

- New booking
- Cancellation
- Reschedule request
- Upcoming appointments

---

## Rescheduling

Clients can request a new appointment.

Professionals may approve or reject according to their booking policy.

---

## Cancellation

Each professional defines:

- Cancellation window
- Late cancellation policy
- No-show policy

Atlas enforces those rules consistently.

---

## Repeat Booking

After appointment completion clients should be able to:

- Book the same service again
- Book with the same professional
- Choose a new date quickly

Repeat booking should require as few steps as possible.

---

# 7. User Flow

Client opens professional profile

↓

Chooses service

↓

Chooses date

↓

Chooses available time

↓

Adds notes

↓

Confirms booking

↓

Professional receives notification

↓

Appointment confirmed

↓

Appointment completed

↓

Client leaves review

↓

Client rebooks

---

# 8. Success Metrics

Primary

- Booking completion rate
- Booking confirmation rate
- Repeat booking rate

Secondary

- Cancellation rate
- No-show rate
- Average booking time
- Time from profile view to booking
- Reminder open rate

---

# 9. Edge Cases

- Double booking attempts
- Time zone differences
- Last-minute cancellations
- Fully booked schedules
- Internet interruptions
- Client no-show
- Professional no-show
- Deleted accounts with future bookings

---

# 10. Future Improvements

Potential enhancements:

- Instant booking
- Waitlists
- Group bookings
- Recurring appointments
- Smart scheduling suggestions
- AI appointment optimization
- Integrated payments
- Deposit handling
- Calendar synchronization
