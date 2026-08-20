# Expense Tracker CLI

> Records what I spent, on what and when — and answers **"where did the money go
> last month?"**

**Project 1 · Weeks 1–4** · Plain Node · JSON file · no database

---

## Context

|             |                                           |
| ----------- | ----------------------------------------- |
| **User**    | Only me, for now                          |
| **Surface** | Terminal on my laptop                     |
| **Usage**   | Opened every day, usually in the evenings |

---

## Features

- [ ] **Add** an expense — amount, category, date, optional note
- [ ] **List** all expenses, newest first
- [ ] **Filter** by category, and by date range
- [ ] **Edit** an expense
- [ ] **Delete** an expense
- [ ] **Totals** — monthly total, and a total per category
- [ ] **Persistence** — data survives between runs in a JSON file
- [ ] **Failure handling** — every failure handled explicitly: file missing,
      corrupt JSON, bad input

---

## Out of scope

Users · login · database · UI · any framework beyond Express

---

## Data model

| Field      | Type    | Rules            |
| ---------- | ------- | ---------------- |
| `id`       | string  | UUID             |
| `amount`   | number  | Must be positive |
| `category` | string  | Required         |
| `date`     | string  | ISO string       |
| `note`     | string? | Optional         |

```json
{
	"id": "3f9a1c8e-5b2d-4e77-9a10-6c4f2b8d0e13",
	"amount": 24.9,
	"category": "groceries",
	"date": "2026-08-20",
	"note": "week shop"
}
```

---

## Done means

The project is **deleted locally and rebuilt from an empty folder** — timed, and
the time recorded.

- [ ] Rebuild done in **one sitting**
- [ ] Old repo **closed** throughout
- [ ] Time recorded: `___ min`

Until that time is written down, this is practice — not evidence.
