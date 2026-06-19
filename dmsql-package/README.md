# DM Database (达梦) SQL Snippets

Espanso snippets for working with **DM Database** (达梦数据库, DMSQL), covering:

- Common SQL syntax (`SELECT`, `INSERT`, `UPDATE`, `DELETE`, `JOIN`, `CREATE TABLE`, indexes, paging)
- DM-specific functions and system views (`V$VERSION`, `V$INSTANCE`, `V$SESSIONS`, `V$LOCK`, `V$SQL`, `V$DM_INI`, `SYSDATE`, `ROWID`, `EXPLAIN`)
- DBA/admin commands (users, grants, tablespaces, backup/restore, killing sessions, table size)

## Triggers

| Trigger | Description |
| --- | --- |
| `:dmsel` | SELECT template |
| `:dmins` | INSERT template |
| `:dmupd` | UPDATE template |
| `:dmdel` | DELETE template |
| `:dmjoin` | JOIN template |
| `:dmctab` | CREATE TABLE template |
| `:dmidx` | CREATE INDEX template |
| `:dmlimit` | SELECT with LIMIT |
| `:dmpage` | SELECT with LIMIT/OFFSET paging |
| `:dmver` | Query `V$VERSION` |
| `:dminst` | Query `V$INSTANCE` |
| `:dmsess` | Query `V$SESSIONS` |
| `:dmlock` | Query `V$LOCK` |
| `:dmsql` | Search `V$SQL` by text |
| `:dmsysparam` | Query `V$DM_INI` parameter |
| `:dmsysdate` | `SELECT SYSDATE FROM DUAL` |
| `:dmrowid` | SELECT with `ROWID` |
| `:dmexplain` | `EXPLAIN` statement |
| `:dmcreateuser` | CREATE USER |
| `:dmgrant` | GRANT privileges |
| `:dmrevoke` | REVOKE privileges |
| `:dmtbs` | CREATE TABLESPACE |
| `:dmbackup` | BACKUP DATABASE |
| `:dmrestore` | RESTORE DATABASE |
| `:dmkilsess` | `SP_CLOSE_SESSION` |
| `:dmtabsize` | Table size report |
