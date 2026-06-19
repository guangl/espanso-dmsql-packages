# DM Database (达梦) SQL Snippets

Espanso snippets for working with **DM Database** (达梦数据库, DMSQL), covering:

- Session/事务管理 (active sessions, transaction blocking/wait)
- 系统参数与版本查询 (`V$DM_INI`, version info)
- DBA 操作 (creating users and granting privileges)
- 备份 (full database backup)
- 内存诊断 (per-session memory usage, buffer pressure, total memory)
- 故障诊断 (deduplicated stack traces, cached/package execution plan dumps)

## Triggers

| Trigger | Description |
| --- | --- |
| `:dmsess` | 查看当前的活动会话 |
| `:dmtwait` | 查看当前事物阻塞 |
| `:dmparam` | 查询系统参数值 |
| `:dmver` | 查询数据库版本 |
| `:dmcuser` | 创建用户以及赋予权限 |
| `:dmbackup` | 对数据库进行全量备份 |
| `:dmmemsql` | 单个会话内存使用总量 |
| `:dmbuff` | 判断 BUFFER 空闲还是紧张 |
| `:dmmemtotal` | 达梦内存总量 |
| `:dmpsp` | 去重堆栈 |
| `:dmtrace` | 获取缓存计划/包计划 |
