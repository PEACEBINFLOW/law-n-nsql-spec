# N-SQL Overview

N-SQL (Network SQL) is the declarative query language of **Law-N**.

Its goal is simple:

> “Give developers a way to see and manipulate the live network.”

Not logs.  
Not metrics.  
Not APIs.  
**The network itself.**

---

## Core Concepts

### 1. Network Tables
Logical network tables exposed by Law-N:

- `network.devices`
- `network.routes`
- `network.frequencies`
- `network.towers`
- `network.patterns`

### 2. Operators
N-SQL introduces new primitives:

- `INSPECT`
- `OPTIMIZE`
- `TRACE`
- `ANALYZE`
- `SIMULATE`
- `MATCHES` (pattern)
- `HARMONIC OF`
- `DRIFT <value>`
- `WITH PATTERN <pattern>`

### 3. Execution Model
N-SQL is:

- **live** (always current)
- **stateful** (network changes affect queries)
- **topology-aware**
- **signal-native**

### 4. Purpose
Replace:
- SNMP
- NetFlow
- traditional logs
- black-box APIs
- 7–12 hop indirection

Provide:
- real-time introspection
- pattern-based routing
- frequency analytics
- device/tower visibility
