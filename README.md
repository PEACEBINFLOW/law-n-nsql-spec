# 🟪 N-SQL Specification  
### Network SQL for the Law-N Network Renaissance

N-SQL is the **query language for live networks**.

Unlike SQL (tables and rows) or GraphQL (typed APIs),  
**N-SQL queries the real-time state of signals, towers, frequencies, and routes.**

This repo defines:

### ✔ The N-SQL grammar (EBNF)  
### ✔ Semantic rules (how queries behave)  
### ✔ Reference schemas for devices, towers, routes, frequencies  
### ✔ Query examples used in tower simulators, CLSI, and Law-N engines  
### ✔ Migration guide for developers coming from SQL, GraphQL, or SNMP  

---

# What is N-SQL?

**N-SQL is a live, network-native query language designed for Law-N.**

It lets you run queries like:

```sql
SELECT tower_id, pattern, latency
FROM network.routes
WHERE device = "0xA4C1"
AND frequency MATCHES "MidBand-*"
AND signal_quality > 0.85;
