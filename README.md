# PG-CC

#Architect 
The Transactional Database Postgresql 10 support the quorum commit for multiple synchronous replication ,
the replication still receive WAL from master directely.

Here we use Apache Kudu to store and tansffer the WAL , it porovides RAFT consistency.

The Postgresl master server do not kown where is the replica.
The replica number should be more than 5.

