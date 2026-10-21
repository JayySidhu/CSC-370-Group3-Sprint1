# Co-op Application Tracker - CSC 370 Sprint 1

Group 3: Amrinder Singh, Jaiman Singh, Aashna Sadeque. 
We worked together on the design, implementation, verification and documentation.

This MySQL database tracks students' co-op applications, job postings, resume selections, interview rounds and offers. Sprint 1 extends the kick-off implementation with a normalized resume-selection relationship, stronger integrity rules, complete diagrams and reproducible verification. All demonstration data is synthetic.

## Run the database and reports

Requirement: MySQL 8.0.16 or later. Recorded database verification used MySQL 8.4.8. All nine tables explicitly use InnoDB.

Run these commands from the repository root with a MySQL account permitted to create databases, tables and triggers and execute SELECT, INSERT, UPDATE and DELETE:

```sh
mysql -u root -p < schema.sql
mysql -u root -p < supporting-files/seed.sql
mysql -u root -p < supporting-files/demo_queries.sql
``` 

## Verification evidence

The [evidence index](evidence/README.md) describes the saved results: 56 database checks, 15 migration checks, 12 worked theory checks, 10 design checks and two conceptual-diagram coverage checks. The [seven report outputs](evidence/demo-output.tsv) can be compared with a fresh run of the supplied schema, seed and report SQL.
