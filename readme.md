# Zap Shift Resources

Welcome to **Zap Shift Resources**!  
A curated collection of tools, guides, and assets for developing robust parcel management systems.

---

## 📊 System Overview Table

| Role            | Key Responsibilities                                                                      | Earnings/Benefits                              |
| --------------- | ----------------------------------------------------------------------------------------- | ---------------------------------------------- |
| **User**        | - Book parcels<br>- Pay charges<br>- Track status<br>- Review service                     | - Real-time tracking<br>- Feedback opportunity |
| **Admin**       | - Assign agents<br>- Manage routing<br>- Oversee warehouses<br>- Monitor operations       | - System control<br>- Operational oversight    |
| **Agent/Rider** | - Collect/Deliver parcels<br>- Update status<br>- OTP confirmation<br>- Warehouse handoff | - ৳20 per delivery                             |

---

## 🛒 Pricing Structure

| Parcel Type      | Weight    | Within City | Outside City/District |
| ---------------- | --------- | ----------- | --------------------- |
| **Document**     | Any       | ৳60         | ৳80                   |
| **Non-Document** | Up to 3kg | ৳110        | ৳150                  |
| **Non-Document** | >3kg      | +৳40/kg     | +৳40/kg +৳40 extra    |

---

## 🚚 Delivery Workflow

```mermaid
flowchart TD
    A[User Adds Parcel to System] -->|Status: Unpaid| B[User Pays for Parcel Delivery]
    B -->|Status: Paid| C[Admin Assigns Pickup & Delivery Riders]
    C -->|Status: Ready-to-Pickup| D[Rider Picks Up Parcel]
    D -->|Status: In-Transit| E{Within City?}

    E -- Yes --> F1[Rider Out for Delivery]
    F1 -->|Status: Ready-for-Delivery| G1[Rider Delivers Parcel]
    G1 -->|Status: Delivered| H1[Parcel Delivery Completed]

    E -- No --> F2[Parcel Reaches Warehouse]
    F2 -->|Status: Reached-Warehouse| G2[Parcel Shipped to Destination]
    G2 -->|Status: Shipped| H2[Rider Out for Delivery]
    H2 -->|Status: Ready-for-Delivery| I2[Rider Delivers Parcel]
    I2 -->|Status: Delivered| J2[Parcel Delivery Completed]

```

---

## 🗂️ Key Features

- **Automated Pricing & Tracking**
- **Role-based Access & Workflow**
- **OTP-based Secure Delivery**
- **Nationwide Coverage (64 districts)**
- **Transparent Commission Structure**

---

---
