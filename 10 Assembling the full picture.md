ASSEMBLING THE FULL PICTURE:

**Introduction:**

Before Process Mining can reconstruct a business process, it must gather all important information.

The Event Log contains the three core elements:

- Case ID
- Activity
- Timestamp

But in real business systems, there is often more useful information available.

To understand the full process clearly, Process Mining also uses additional business data stored in something called a **Case** **Table**.

**Event Log + Case Table = Data Model**

This is called: Assembling the Full Picture

This gives a complete picture of the business process.

---

The Event Log stores the basic activity history of a process (Core Process Data).

- what happened
- when it happened
- for which case it happened

Example:

|Case ID| Activity        | Timestamp|
|-------|-----------------|----------|
|PO001  | Order Created   | 10:00 AM |
|PO001  | Approval Done   | 2:00 PM  |
|PO001  | Payment Released| Next Day |

This helps Process Mining reconstruct the process flow.

---

IT systems also store other useful information such as: (Additional Business Information Exists)

- vendor name
- customer name
- location
- order value
- invoice amount
- department name
- product category

This information is not usually stored inside the Event Log.

**It is stored in: Case Table**

---

**What is a Case Table?**

A Case Table stores extra details related to each case.

Example:

|Case ID| Vendor Name | Location| Order Value|
|-------|--------------|--------|------------|
|PO001  | ABC Supplier| Mumbai  | ₹50,000    |

This gives more business context to the process.

It helps answer deeper questions like:

- Which vendor causes delays?
- Which location has more bottlenecks?
- Which orders create the most rework?

---

Case ID Connects Both Tables

The most important part is: Case ID

Case ID exists in:

- Event Log
- Case Table

It acts as the: Mapping Key -This key connects both tables.

Because of this, Process Mining can combine process steps with business details.

---

Why This Is Important

Without the Case Table: -we only see process steps.

With the Case Table: -we understand business reasons behind the process.

This improves:

- root cause analysis
- bottleneck detection
- decision-making
- process optimization
- business insights

This is where real business value increases.

---

Example:

If invoice approval is delayed:

Event Log shows:

     Approval took 5 days

Case Table shows:

     Vendor = New Supplier

Now management understands the reason behind the delay.

This is powerful Process Mining.

---

**Event Log shows process activities, Case Table adds business details, and together they form the Data Model that gives the full picture in Process Mining**
