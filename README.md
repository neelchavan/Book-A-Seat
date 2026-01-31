# 🪑 Seat Booking System (Learning Project)

A simple backend booking system built to understand **how seat booking works at a system-design level**.

This project focuses on the **core booking flow**:
- Users request a seat booking using a `userId`
- The system checks seat availability
- Seats are either **confirmed** or the booking **fails**
- Booking status is returned to the user

---

## 🎯 Purpose

The goal of this project is **learning**, not feature completeness.

The system intentionally avoids:
- User management
- Payments
- Authentication

This keeps the domain small and helps focus on:
- Entity modeling (`Seat`, `Booking`)
- State transitions
- Transaction management
- Avoiding double booking
- Writing clean service-layer logic

---

## 🧠 Design Choices

- `userId` is treated as an **external reference**, not a stored User entity
- Minimal entities to avoid over-engineering
- Business-first design over database-first modeling
- Easily extensible for future additions like users, payments, or cancellations
