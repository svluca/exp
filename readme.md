# MyMon — v1 Overview

MyMon is a simple personal expense tracker focused on clarity, not complexity.

---

## What MyMon v1 Is

- A small tool to track personal expenses
- Focused on monthly spending clarity
- Built to grow later, without overengineering now
- Not a social network (yet)
- Not a full finance system

---

## Target & Scope

- Initial users: me and close friends
- Language: English
- Focus: expenses only (no income in v1)

---

## Pages

- Landing Page
  - Visible only to non-authenticated users
- App / Dashboard
  - Default page after login

---

## User Flow

- User enters the site
- If not logged in, sees the landing page
- If logged in, goes directly to the dashboard
- User sees:
  - name or nickname
  - a clear message:
    - “This month you’ve spent $X”
    - or “Last month you spent $X”
- User clicks “Add expense”
- User fills the form
- Totals and statistics update instantly

---

## Transaction Definition (v1)

A transaction contains:
- category
- amount
- date
- optional comment

Validation rules:
- amount must be greater than 0.01
- amount cannot be negative
- date cannot be in the future
- date can be from:
  - current month
  - previous month
- comment is optional

---

## Month Logic

- Months are calendar-based
- Month is derived from transaction date (YYYY-MM)
- No month closing logic
- No background jobs
- No custom salary cycles in v1

---

## Categories

- Fixed list of categories
- Includes an “Other” category
- Users cannot create custom categories in v1

---

## Statistics Displayed (v1)

For a selected month:
- total amount spent
- total per category (sum)
- percentage per category
- simple visual diagram (no external chart libraries)

---

## UI / UX Principles

- Minimal text
- Plenty of white space
- Clean overview
- Details only on demand
- One main action: “Add expense”

---

## Technical Approach

- Start with clear structure
- Build functional frontend first
- Simulate backend locally
- Add real backend and database later

---

## Explicitly Out of Scope for v1

- income tracking
- refunds or loans
- friend
