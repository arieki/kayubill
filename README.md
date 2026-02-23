# 🪵 KayuBill

> Headless billing engine for subscriptions, invoicing, and payment orchestration.

> 🚧 **Status:** Early development (v0.x). APIs and interfaces may change.

---

## What Problem Does KayuBill Solve?

Payment gateways process transactions. They do not manage billing lifecycle.

Modern SaaS systems still need to handle:

- Subscription state transitions (active, past_due, canceled)
- Invoice generation and consistency
- Idempotent webhook handling
- Payment retry logic
- Billing event emission
- Separation between payment processing and billing logic

KayuBill focuses purely on billing infrastructure.

It sits between your application and your payment provider, acting as the billing brain of your system.

KayuBill is not a payment gateway. KayuBill persists billing state in its own datastore and does not require access to your application database.

**What you get:** an HTTP API to manage subscriptions, invoices, and payment lifecycle.  
Your application owns product logic; KayuBill owns billing consistency.

---

## License

[Apache License 2.0](LICENSE)