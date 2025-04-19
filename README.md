# 📊 Hotel Booking Analytics Dashboard – Business Analyst Portfolio

This project demonstrates my ability as a Business Analyst to gather requirements, analyze booking data, and deliver actionable insights using Excel and SQL.

---

## 🎯 Objective

To create a visual, data-driven Excel dashboard using simulated hotel booking data and identify key performance metrics for business decision-making.

---

## 📈 Features of the Dashboard

- Total Bookings and Revenue by Month
- Cancellation Rate
- Most Booked Room Types
- Booking Source Analysis
- Interactive Filters (Room Type, Date Range, Booking Status)

---

## 🗃️ Dataset Overview

**File:** `/Data/hotel_booking_data.csv`  
**Fields:**
- booking_id
- booking_date
- check_in_date
- check_out_date
- room_type
- booking_status
- booking_source
- price
- guest_count

---

## 🧾 Sample SQL Query

```sql
SELECT room_type, COUNT(*) AS total_bookings
FROM hotel_bookings
WHERE booking_status = 'Confirmed'
GROUP BY room_type
ORDER BY total_bookings DESC
LIMIT 5;
