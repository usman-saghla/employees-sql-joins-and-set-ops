# Employees SQL — Joins Deep-Dive (MySQL)

This repo is a hands-on tour of SQL join patterns using the classic **`employees`** sample database.  
You’ll build a small “messy” sandbox (dup tables with NULLs/missing keys) and then practice:

- INNER / LEFT / RIGHT / (emulated) FULL OUTER joins
- CROSS JOIN (Cartesian)
- SELF JOIN (same table twice)
- Multi-table chains (4+ tables)
- Semi-join (`EXISTS`) and Anti-join (`LEFT … IS NULL`)
- Aggregation with joins (`GROUP BY`)
- Practical pitfalls (`ON` vs `WHERE`, duplicate blow-ups)
- Performance tips (basic indexing strategy)

> **Script:** `02_joins.sql`  
> (Name it whatever you like; this README assumes you’re running everything inside that one script.)

---

## 1) Prerequisites

- **MySQL** 8.x (or 5.7+)  
- **`employees`** sample DB installed
  ```sql
  SHOW DATABASES;
  USE employees;
