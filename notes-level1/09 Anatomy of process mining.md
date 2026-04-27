ANATOMY OF PROCESS MINING -- DIGITAL FOOTPRINT AND EVENT LOG:

**Introduction:**

The foundation of Process Mining is built on these digital records called digital footprints.

When these digital footprints are structured correctly, they form an event log, which is the main input for Process Mining.

ANATOMY:
DIGITAL FOOTPRINT = Activity + Timestamp + Case ID

EVENT LOG = MANY DIGITAL FOOTPRINTS ARE COLLECTED AND STORED IN A TABLE FORMAT.

It stores digital footprints of business processes and helps Process Mining tools reconstruct and analyze the real process flow.

---

**What is a Digital Footprint?**

A data created when one activity happens in a system.

Examples:

- receiving a customer order
- creating an invoice
- approving a payment
- shipping goods
- updating a support ticket

Every interaction creates system data automatically.

---

**Three Important Parts of a Digital Footprint:**

Every digital footprint contains three key elements:

**1. Activity:--What happened?**

Examples:

- Order Created
- Payment Completed
- Invoice Generated
- Delivery Confirmed

Activity represents the actual process step.

---

**2. Timestamp:--When did it happen?**

Examples:

- 10:00 AM
- 2:30 PM
- Next Day

Timestamp helps calculate delays, waiting time, and total process duration.

---

**3. Case ID:--For which process instance did it happen?**

Examples:

- Order Number
- Invoice Number
- Service Ticket Number
- Candidate ID

Case ID connects all activities belonging to the same process.

(It must always be unique.)

Without a unique Case ID, Process Mining cannot work correctly.

---

**Example** – Food Delivery App

Imagine ordering dinner using a delivery app.

Order Number = Case ID (unique)

Activities may :

- Food Selection
- Payment
- Meal Preparation
- Pickup
- Delivery

Each activity gets a timestamp showing exactly when it happened.

This creates the full digital footprint of your order.

---

**What is an Event Log?**

When all digital footprints are stored together in a structured table, it becomes an Event Log.

An event log is the main input used by Process Mining tools like Celonis.

Simple Example:

|Case ID| Activity      | Timestamp|
|-------|---------------|----------|
|ORD001 | Payment Done  | 7:00 PM  |
|ORD001 | Meal Prepared | 7:20 PM  |
|ORD001 | Delivered     | 7:45 PM  |

This table helps the system understand the complete process flow.

---

**Why Unique Case ID is Important?**

Every case must have its own unique identifier.

For example:

- each food order needs a unique order number
- each invoice needs a unique invoice number

Without uniqueness, activities can get mixed between different cases.-->This creates incorrect analysis -->Just like receiving the wrong food delivery.

---

**How Process Mining Uses Event Logs?**

Once event logs are available, tools like Celonis can:

- reconstruct the actual process flow
- identify bottlenecks
- detect delays
- find repeated steps
- discover compliance issues
- visualize the complete workflow

This gives companies a transparent and objective view of how processes actually run.

---

Order-to-Cash Example

In an online retail company, the Order-to-Cash process includes:

Order Received → Goods Shipped → Invoice Created → Payment Received

Every step creates digital footprints.

These footprints show:

- what was done
- when it was done
- for which sales order it was done

This helps Process Mining discover the real business process.

---

One photo = Digital footprint

Full photo album = Event log

---

One-Line Summary

Digital Footprints become Event Logs, and Event Logs are the foundation of Process Mining.
