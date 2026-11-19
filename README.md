# SaveFood — Team Prototype & Learning Journey

**CSIS 3175-004 · Group 3 · Fall 2026**

This public repository hosts two companion resources for the **SaveFood Food Wastage Reduction Android final project**. Both were reviewed on **November 19, 2026** against the private Android repository's `main` commit [`bc346393`](https://github.com/user09022022/SaveFood-CSIS3175/commit/bc346393897ee6985be9e0ce94398cae8dab75d0) (merged PR #12, Room / SQLite integration).

## Open the resources

- **[Interactive SaveFood prototype](https://user09022022.github.io/SaveFood-Prototype/)** — browser recreation of customer, manager, authentication/profile screens and order workflows.
- **[SaveFood Learning Journey](https://user09022022.github.io/SaveFood-Prototype/learning/)** — 12 guided lessons, 15 source-code excerpts, Room schema, practice order lab, 18 questions, readiness checklist and a [five-scenario demo rehearsal](https://user09022022.github.io/SaveFood-Prototype/learning/#demo).
- [Android source (private repository)](https://github.com/user09022022/SaveFood-CSIS3175/tree/bc346393897ee6985be9e0ce94398cae8dab75d0/SaveFood) — requires teammate authorization.

## Prototype credentials (browser only)

| Role | Email | Password |
| --- | --- | --- |
| Customer | `customer@savefood.test` | `Demo123!` |
| Restaurant Manager | `manager@savefood.test` | `Demo123!` |

Run the manager and customer sides **in the same browser** so they share demo data. These credentials are sample accounts for the HTML simulation **only** and are **not** accounts in the actual Android Room database.

## Demonstration route

1. Manager creates/configures a restaurant, posts discounted food and sets quantity.
2. Customer searches by city, opens food details, adds a product and confirms Pickup or Delivery.
3. Manager accepts the order, marks it Ready, records a reminder, then completes Pickup/Delivery.
4. Customer sees updated status, reminder and order history.
5. Independently test rejection and customer cancellation of separate Pending orders; verify returned quantity.

Use the Learning Journey's **Demo rehearsal** section for expected evidence, limits, persistence checks and the report/presentation requirements.

## Scope and safeguards

- The public prototype uses **browser local storage**, not Android Java / Room / SQLite. It contains illustrative demo records. A browser demonstration does not prove Android runtime behavior.
- The actual Android project uses **Room on SQLite** for users, restaurants, foods, orders, order lines and reminders. The in-memory cart is not persistent, and session keys use SharedPreferences.
- Password recovery, guest browsing, email/push messaging, cross-device sync and a full profile-photo workflow are not claimed as completed Android features.
- **This repository changes only teaching/prototype material.** No files in the private Android project were edited during this update.

## Course checkpoints

- **November 26, 2026:** final Android application and PDF technical report.
- **November 24 / December 3:** presentations (confirm the team's allocated slot); 15–20 minutes including questions.
- Include team contributions, features, use-case/sequence/class/ER diagrams, layout screenshots and citations for features/tools beyond class. The Android application must use SQLite (Room is permitted).

Source implementation is the private [SaveFood-CSIS3175](https://github.com/user09022022/SaveFood-CSIS3175) repository; this public repo is an educational companion, not the final deliverable.
