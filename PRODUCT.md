# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Independent business owners (including traders, tailors, caterers, and event
managers) who need to show products or services and coordinate customer orders.
Customers browse listings, request a product for a preferred time, and contact
the business directly.

## Product Purpose

BizFlow helps local businesses present their offers and helps owners move an
order from customer request to accepted work to completion. Success means
owners can make an explicit decision about each request and both parties can
see the requested time, price, contact details, and current order state.

## Positioning

BizFlow treats an order as work with a decision, requested time, and completion
state—not just a public product listing. Owners, rather than the app, confirm
availability and the final arrangement.

## Operating Context

Customers discover public business profiles, view prices and public business
phone numbers, then submit an order request for pickup, delivery, or discussion.
The prototype prepares a WhatsApp deep link for the customer to send to the
owner. Owners accept or decline requests, message customers using a prepared
WhatsApp link, and mark accepted work done.

## Capabilities and Constraints

- Web is an implementation inference from the supplied single-file HTML
  project, not a separately confirmed launch target.
- The current implementation is a single-file browser prototype with
  synthetic sample businesses and orders.
- New owner profiles, offers, and customer-created orders persist only in that
  browser's local storage; there is no server, shared account, or cross-device
  synchronization.
- Owner passwords are not stored in plaintext. The prototype derives a
  PBKDF2 password verifier and AES-GCM key in the browser; registered payment
  details are encrypted locally and unlocked for the active sign-in.
- Public profiles show the business phone and offers, never payment details.
  An unlocked owner can include payment details in a manually sent, direct
  WhatsApp acceptance message.
- WhatsApp links are handoffs requiring the visitor to review and send the
  pre-filled message. There is no WhatsApp API integration, automatic inbound
  order synchronization, payment processing, or delivery booking.
- Due dates can be viewed in the owner's open studio; background alerts,
  scheduled reminders, and automatic customer notifications are not
  implemented.
- Completed-order profit is an estimate based on optional owner-entered costs.
  The prototype cannot read or report a bank balance.
- Treat the prototype as a test-data demonstration, not production
  authentication, accounting, secure payment-detail storage, or a service
  with a demonstrated scale or availability commitment.

## Evidence on Hand

The configured folder contains the `index.html` prototype and two unrelated
wardrobe image assets; there are no production data, real customer
testimonials, backend endpoints, payment integrations, or verified capacity
claims. BizFlow demonstration businesses, people, and prices are synthetic.

## Product Principles

- Make each request's next owner-controlled step clear.
- Show prices, requested times, and public contact details before a customer
  reaches out.
- Keep private payment details out of public listings.
- Represent estimates and handoffs honestly; do not imply that a message,
  payment, or booking happened when the owner has not confirmed it.
- Do not claim production-scale capacity, security, or availability without
  evidence.
