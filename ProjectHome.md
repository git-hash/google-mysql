This project hosts the work-in-progress MySQL 5.1 that contains the MySQL 5.0 Google-specific features (group IDs, semi-sync replication, googlestats engine, etc).


The current tree is based on MySQL 5.1.63 (prior version 5.1.61) and the heads we have the following:

```
20-fixes-google-2 (6)     ######
19-mapped-user (14)       ##############
18-stats (26)             ##########################
17-sql-log (11)           ###########
16-proxy-auth (1)         #
15-httpd (36)             ####################################
14-checksum-io (6)        ######
13-compression (6)        ######
12-user-stats (21)        #####################
11-table-stats (6)        ######
10-multiports (8)         ########
09-innodb-counters (26)   ##########################
08-rpl-semi-sync (12)     ############
07-rpl-crc (5)            #####
06-rpl-ids (47)           ###############################################
05-rpl (9)                #########
04-audit-log (13)         #############
03-fixes-google-1 (32)    ################################
02-fixes (25)             #########################
01-base (26)              ##########################
```

**Note**: the heads are rebased on top each.

How to checkout, build and test the tree:

  * git clone https://code.google.com/p/google-mysql/
  * cd google-mysql/
  * ./google/compile
  * ./google/tests

How to build a deb package:
  * git clean -fxd
  * ./google/deb