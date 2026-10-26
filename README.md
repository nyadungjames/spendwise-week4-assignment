# SpendWise Dashboard Shell

A clean, responsive financial dashboard UI built as the foundation for my capstone project. This week focuses on visual structure only using realistic static content - no JavaScript functionality.

Live Demo: Open `index.html` in browser

## What I Built
Modern SpendWise dashboard shell containing:

- **Sidebar / Navigation Menu**: Brand logo "SpendWise", 6 nav links (Dashboard, Transactions, Analytics, Budgets, Savings, Settings), and user mini-profile
- **Header**: Title "Overview", date range, and action buttons (Export, Add Expense)
- **Summary Strip**: Total Balance KES 84,250 / Spent KES 32,400 / Saved KES 12,800
- **6 Category Cards** with realistic financial info:
    1. Food - KES 8,450 - 65% of budget
    2. Transport - KES 3,200 - 40% of budget
    3. Rent - KES 15,000 - Paid
    4. Entertainment - KES 2,750 - 55% of budget
    5. Savings - KES 12,800 - 75% goal
    6. Utilities - KES 3,000 - 30% of budget

## Tech Stack & What Each Part Does

### index.html
- Semantic HTML5 structure
- `.dashboard` is the main Grid container
- `<aside class="sidebar">` for navigation
- `<header class="header">` for top bar
- `<main class="main">` contains `.stats-summary` and `.cards-grid`
- Each card is `<article class="card" tabindex="0">` - tabindex allows keyboard focus to test micro-interactions
- `aria-label` on sidebar for accessibility

### style.css

**1. Theme using CSS Custom Properties (Requirement #3)**
Defined on `:root`:
```css
--brand-color: #4F46E5;
--accent-color: #10B981;
--surface-color: #F8FAFC;
--card-surface: #FFFFFF;
--sidebar-bg: #111827;
--primary-text: #0F172A;
--secondary-text: #64748B;
--border-color: #E2E8F0;