# Migration from SQL to N-SQL

SQL queries data at rest.  
N-SQL queries the network in motion.

| SQL | N-SQL |
|-----|-------|
| SELECT rows | SELECT live network state |
| WHERE filters | WHERE signal conditions |
| No routing | OPTIMIZE ROUTE |
| No frequency | INSPECT FREQUENCY |
| No live topology | TRACE, ANALYZE |

Migration steps:
1. Map tables → Law-N network tables
2. Map filters → signal conditions
3. Replace joins → route introspection
4. Add frequency/pattern operators
