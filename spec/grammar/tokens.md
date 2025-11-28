# N-SQL Tokens

This document defines the **lexical tokens** that appear in N-SQL queries.

It is a companion to `nsql-ebnf.md`.

---

## 1. Keywords

The following keywords are reserved and **case-insensitive**:

- `SELECT`
- `FROM`
- `WHERE`
- `AND`
- `OR`
- `NOT`
- `INSPECT`
- `OPTIMIZE`
- `ROUTE`
- `ANALYZE`
- `PATTERN`
- `PREFER`
- `MINIMIZE`
- `MAXIMIZE`
- `TRACE`
- `SIMULATE`
- `RETURN`
- `AS`
- `LIMIT`
- `OFFSET`
- `ORDER`
- `BY`
- `GROUP`
- `MATCHES`

Implementations may add more keywords, but these form the **minimum set**.

---

## 2. Identifiers

Identifiers name:

- tables (`network.routes`)
- columns (`latency_ms`)
- functions (future)
- aliases

Rules:

- start with a letter (`A–Z`, `a–z`) or underscore `_`
- followed by letters, digits, or underscores
- examples:
  - `tower_id`
  - `g_layer`
  - `signal_quality`
  - `network.routes`

A dotted name like `network.routes` is treated as a qualified identifier.

---

## 3. Literals

### 3.1 String Literals

- delimited by double quotes `"`  
- internal quotes are escaped as `\"`

Examples:

```sql
"0xA4C1"
"mid-band-5G"
"PulseShift-*"
