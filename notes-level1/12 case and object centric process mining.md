CASE CENTRIC AND OBJECT CENTRIC PROCESS MINING:

**Introduction:**

Celonis mainly explains two types of Process Mining:

1. Case-Centric Process Mining
2. Object-Centric Process Mining

Both are used to understand business processes, but they work differently.

The main difference is:

Case-Centric = focuses on one single case

Object-Centric = focuses on multiple connected objects

---

**Part 1: Case-Centric Process Mining**

**What is Case-Centric Process Mining?**

Case-Centric Process Mining tracks one case (one object) per process.

It is linear and maps all events into one sequential Event Log.

This means: every activity is connected to one chosen Case ID only.

---

Example:

In Order Management:

Case = Sales Order Item

Example:

Order #1001

All activities connected to this order:

- Create Order
- Approve Order
- Ship Product
- Send Invoice
- Receive Payment

All these events are mapped to one single case.

---

Formula: Event = Case + Activity + Timestamp

Example:

Case ID = Order 1001
Activity = Invoice Created
Timestamp = 10:30 AM

This becomes one event in the Event Log.

---

One process usually has:

One Event Log - For more detailed analysis, companies may use multiple event logs.

But the focus is still: One chosen case

---

Benefits of Case-Centric Process Mining

It helps businesses by:

- providing insight into processes from one case perspective
- finding value opportunities
- tracking performance using KPIs
- identifying delays and bottlenecks
- supporting automation decisions

This is simple and easy to analyze.

---

**Part 2: Object-Centric Process Mining**

**What is Object-Centric Process Mining?**

Object-Centric Process Mining tracks: Multiple connected objects together instead of only one case.

This gives a more complete and realistic business view.

---

Example:

In a Purchase Process:

There may be multiple objects:

- Purchase Order
- Invoice
- Vendor
- Payment
- Delivery

These are all connected.

Object-Centric Process Mining studies all of them together.

---

**Why It Is Needed?**

Real business processes are often complex.

One invoice may connect to:- multiple orders

One order may connect to:- multiple deliveries

Case-Centric sometimes misses these relationships.

Object-Centric solves this problem.

---

Example:

Case-Centric View:

      Only track:

      Purchase Order #5001

Object-Centric View:

      Track together:

         - Purchase Order #5001
         - Vendor ABC
         - Invoice #7001
         - Payment #9001
         - Delivery #3001

This gives the full business picture.

---

**Benefits of Object-Centric Process Mining**

It helps businesses by:

- understanding complex relationships
- improving cross-process visibility
- reducing blind spots
- finding hidden inefficiencies
- supporting better business decisions
- improving end-to-end process transparency

This is more advanced and powerful.

---

Easy Comparison

|Feature     | Case-Centric      | Object-Centric                    | 
|------------|-------------------|-----------------------------------|
|Focus       | One single case   | Multiple connected objects        |
|Structure   | Linear            | Network-based                     |
|Example     | One Sales Order   | Order + Invoice + Vendor + Payment|
|Complexity  | Simple            | Advanced                          |
|Visibility  | Limited           | Full picture                      |

---

Simple Memory Trick:

Case-Centric--->"Follow ONE item"

Example: Follow one food delivery order

---

Object-Centric--->"Follow EVERYTHING connected"

Example: Order + Restaurant + Delivery Partner + Payment + Customer

---

**Case-Centric Process Mining follows one case at a time, while Object-Centric Process Mining connects multiple related business objects to provide a complete process view.**
