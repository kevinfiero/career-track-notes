* Transactions [Link 1](https://node-postgres.com/features/transactions) [Link 2](https://www.postgresqltutorial.com/postgresql-transaction/)
  * PostgreSQL transactions are considered ACID:
    * **Atomicity** guarantees that the transaction completes in an all-or-nothing manner.
    * **Consistency** ensures the change to data written to the database must be valid and follow predefined rules.
    * **Isolation** determines how transaction integrity is visible to other transactions.
    * **Durability** makes sure that transactions that have been committed will be stored in the database permanently.
  * Use the BEGIN transaction to start, COMMIT so that it is visible in other sessions, and ROLLBACK if it needs to be reverted.
