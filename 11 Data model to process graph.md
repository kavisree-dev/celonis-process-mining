DATA MODEL TO PROCESS GRAPH:

**Introduction**

The Event Log and Case Table gather all data that exists for all existing Case IDs into one Data Model but this is only half the work.

This data needs to be assembled according to their Case IDs to make chronological sense of it and organize the activities in sequence so it can be analyzed. 

The Event Log and Case Tables simply form the data-based nucleus from which Process Mining technologies reconstruct workflows and process flows.

One of the biggest strengths of Process Mining is transparency.

Companies often believe their processes follow one standard path, but in reality, many cases follow different paths.

Some processes have extra steps, missing approvals, delays, or repeated work.

**Process Mining helps identify these real activity flows and shows how often each one happens.**

**These different paths are called Process Variants.**

This gives companies full visibility into how processes actually run.

---

1 - First Step...

All activities and other relevant information are aggregated by Case ID.

For example, 

|Case ID| Activity        | Timestamp|
|-------|-----------------|----------|
|PO001  | Order Created   | 10:00 AM |
|PO001  | Approval Done   | 2:00 PM  |
|PO001  | Payment Released| Next Day |

Case ID 10001 undergoes the activities - 
 "create purchase order", "print and sent purchase order", "goods receipt", "scan invoice" and "book invoice".
 
This allows you to reconstruct exactly what has happened to this particular Case ID with a sequence of corresponding events.

2 - second Step...

We aggregate the activities for all Case IDs across the Data Models. 

Activity flows (which are also known as "traces") start to repeat and we can find recurring patterns.

For Example,

|Case ID| Activity        | Timestamp|
|-------|-----------------|----------|
|PO001  | Order Created   | 10:00 AM |
|PO001  | Approval Done   | 2:00 PM  |
|PO001  | Payment Released| Next Day |

|Case ID| Activity        | Timestamp|
|-------|-----------------|----------|
|PO002  | Scan invoice    | 10:00 AM |
|PO002  | Approval Done   | 2:00 PM  |
|PO002  | Payment Released| Next Day |

3 - final step...

Finally we Gain Transparency

This makes it possible to reconstruct and visualize traces (activity flows) by frequency using a tool such as the Celonis Variant and Process Explorer (see screenshot below).

We can finally achieve transparency at a scalable level across all Case IDs!

For Example,

|       Activity        |
|-----------------------|
| Order Created         |       *1450 times
| Scan invoice          |

|       Activity        |
|-----------------------|
| Approval Done         |       *3554 times
| Payment Released      |
| Payment Released      |



---

**What is a Process Variant?**

A Process Variant is a different version of the same business process.

Even if the process goal is the same, the sequence of activities may differ between cases.

Example:

Expected process: Create Purchase Order → Goods Receipt → Invoice → Payment

Actual process may have multiple variants.

---

Example of Process Variants

Variant 1

Create Purchase Order
→ Print and Send Purchase Order
→ Goods Receipt
→ Scan Invoice
→ Book Invoice

This may happen:

x1450 Case IDs

Meaning this exact activity flow happened 1450 times.

---

Variant 2

Create Purchase Requisition
→ Create Purchase Order
→ Print and Send Purchase Order
→ Goods Receipt
→ Scan Invoice
→ Book Invoice

This may happen:

x2647 Case IDs

This means another variation of the same process happened 2647 times.

---

Variant 3

Scan Invoice
→ Create Purchase Order
→ Print and Send Purchase Order
→ Goods Receipt
→ Book Invoice

This may happen:

x1082 Case IDs

This shows that some cases followed an unusual order.

This may indicate inefficiency or process problems.

---

**What is a Case ID?**

Each individual process instance has a unique identifier called: Case ID

Examples:

- Purchase Order Number
- Invoice Number
- Order Number
- Service Ticket Number

Each Case ID represents one complete journey of the process.

Process Mining groups activities using this Case ID.

---

**Why Frequency Matters?**

Process Mining does not only show the process path.

It also shows:

How often each variant happens

This helps answer:

- Which process flow is most common?
- Which variant causes delays?
- Which unusual path creates compliance risk?
- Which process needs improvement first?

Frequency helps prioritize business decisions.

---

**Celonis Variant Explorer":**

Tools like Celonis use features such as:

      Variant Explorer and Process Explorer

These tools help companies:

- reconstruct real process flows
- group similar cases together
- count process variants
- detect bottlenecks
- improve process transparency

This creates scalable visibility across thousands of Case IDs.

---

**Why Transparency Matters?**

Without Process Mining: companies depend on assumptions.

With Process Mining: they can clearly see:

- delays
- rework
- skipped approvals
- unusual process behavior
- process inefficiencies

This is called:**Process Transparency**

And this is where major business value is created.

---

Real Example:

Expected:

      Order → Approval → Payment

Actual:

     Most common:

      Order → Approval → Payment
      (2000 cases)

      Problematic variant:

      Order → Rework → Delay → Approval → Payment
      (500 cases)

Now management can focus on fixing the real issue.

---

**Process Mining groups Case IDs into Process Variants, counts how often each path occurs, and provides full transparency into real business workflows.**
