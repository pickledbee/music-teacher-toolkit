# Music Teacher Toolkit

A zero-dependency, browser-based prototype for independent violin, piano, guitar, and other private music teachers.

## Features
- Student profiles and lesson rates
- Lesson scheduling (date/time list)
- Attendance statuses
- Payment recording
- Practice assignments
- Dashboard with student, lesson, and payment totals
- JSON backup and restore

## Run
Open index.html in a browser. To publish: Settings → Pages → Deploy from a branch → main / root.

## Important limitations
This prototype stores data in localStorage on each browser/device. It has **no accounts, secure database, sync, recurring scheduling, invoices, subscription billing, or multi-tenant isolation**. Do not enter real student personal data until proper security and privacy controls are implemented. Payments are recorded, not processed; dashboard revenue is all-time recorded payments, not profit.

## Roadmap
Authentication, private per-teacher cloud storage, recurring calendar, invoices, payment reconciliation, and Stripe subscriptions.
