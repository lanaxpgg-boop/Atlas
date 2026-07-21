# Messaging PRD

Version: 1.0

---

# 1. Purpose

Messaging enables secure and efficient communication between clients and beauty professionals before and after a booking.

Its purpose is to reduce uncertainty, improve trust, and resolve appointment-related questions without leaving Atlas.

---

# 2. Problem Statement

Today, communication usually happens outside the booking platform.

Clients and professionals move to:

- Instagram DMs
- WhatsApp
- Facebook Messenger
- SMS
- Phone calls

This creates fragmented conversations, lost information, slower response times, and a poor user experience.

Atlas centralizes communication in one place.

---

# 3. Goals

Messaging should:

- Support the booking process.
- Reduce unnecessary friction.
- Keep appointment communication organized.
- Increase trust.
- Reduce no-shows.
- Improve customer satisfaction.

---

# 4. Non-Goals

Messaging is not intended to:

- Compete with WhatsApp or Telegram.
- Become a general-purpose chat application.
- Replace social messaging.

Its responsibility is communication related to services and appointments.

---

# 5. User Stories

## Client

As a client I want to:

- Ask questions before booking.
- Clarify service details.
- Send inspiration photos.
- Receive appointment updates.
- Contact my professional easily.
- View previous conversations.

## Professional

As a professional I want to:

- Answer client questions.
- Share preparation instructions.
- Confirm appointment details.
- Notify clients about schedule changes.
- Keep all conversations linked to bookings.

---

# 6. Functional Requirements

## Conversations

Each conversation is linked to:

- Professional
- Client
- Booking (if applicable)

---

## Supported Messages

Users can send:

- Text messages
- Emojis
- Photos
- Appointment links
- Service information

Future:

- Voice messages
- Video messages
- Documents

---

## Booking Context

When a booking exists, the chat displays:

- Booking status
- Appointment date
- Appointment time
- Selected service

This gives both users context without switching screens.

---

## Notifications

Users receive notifications for:

- New messages
- Booking updates
- Appointment reminders
- Reschedule requests

---

## Safety

Messaging includes:

- Reporting
- Blocking
- Spam detection
- Abuse prevention

---

# 7. User Flow

Client opens professional profile

↓

Client sends question

↓

Professional replies

↓

Client books appointment

↓

Conversation remains linked to booking

↓

Both parties receive updates until appointment completion

---

# 8. Success Metrics

Primary

- Response rate
- Response time
- Booking conversion after conversation

Secondary

- Conversation completion
- Client satisfaction
- Professional satisfaction
- Reduced cancellation rate

---

# 9. Edge Cases

- Unanswered conversations
- Spam messages
- Blocked users
- Deleted accounts
- Bookings cancelled during conversation
- Multiple simultaneous conversations

---

# 10. Future Improvements

Potential enhancements:

- AI-powered quick replies
- Automatic translation
- Smart FAQs
- Appointment preparation templates
- Voice and video calls
- Shared inspiration boards
