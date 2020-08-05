# JDBC Project for Batch 18
A project to demonstrate usage of **_Java Database Connectivity_** from **JDK**.

* DriverManager
* Driver
* Connection
* Statement
* ResultSet
* SQLException
---
```java
Connection conn = DriverManager.getConnection(connectionStr, username, password);
Statement stmnt = conn.createStatement( ResultSet.TYPE_SCROLL_INSENSITIVE,
                                        ResultSet.CONCUR_READ_ONLY);
ResultSet rs = stmnt.executeQuery("SELECT * FROM JOBS");
```