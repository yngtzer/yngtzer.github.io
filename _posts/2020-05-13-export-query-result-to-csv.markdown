---
layout: post
title: "Export Query Result To CSV Format"
date: 2020-05-13  23:19:00 +0800
categories: SQL
---

### Export Query Result To CSV

1. `docker exec -it my_docker_name sh`
2. `sqlplus / as sysdba`
3. `alter session set current_schema=MY_SCHEMA`
4. `set colsep ","`
5. `set pagesize 50000`
6. `set trimspool on`
7. `set linesize 32767`
8. `set underline off`
9. `alter session set NLS_TIMESTAMP_FORMAT='DD-MON-YYYY HH24:MI:SS.FF';`
10. `spool myOutputCsv.csv`
11. execute your query here...
12. `spool off`