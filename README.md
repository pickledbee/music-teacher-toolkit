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

## Voice and check-photo entry
- Click **Start speaking** and allow microphone access. Browser speech recognition support varies (Chrome is recommended).
- Spoken student details are parsed into a confirmation form. Payments can also be dictated.
- Upload a check image to attempt OCR of the amount, written date, and check number. The OCR engine loads from a third-party CDN and runs recognition in the browser; no check image is intentionally stored in the app.
- **Always verify the check amount, student, and payment date before saving.** OCR can be inaccurate and written dates are not automatically applied.
- Routing and account numbers are not extracted into the app.
- This is not bank deposit, check processing, or automated reconciliation.
- Voice recognition may use a browser/vendor speech service, so do not dictate sensitive personal or financial information without understanding your browser's privacy behavior.
