# The object-relational impedance mismatch

Mapping classes to tables: how to implement inheritance with tables?
* one table per class: leads to too many JOINs
* one table per concrete class: incurs large denormalization costs, throws away NULL constraints offered by RDBMSs
* one table per class family (a single table for the entire hyerarchy): again, throws away NULL constraints

Associations between objects are different from foreign keys between tables. [...?]

Who owns the database schema: developers of a specific object-oriented application or a database team?
Similary, how to deal with refactorings when the schema is effectively duplicated between the database
and the application(s)?

Object oriented systems are based on identity, while relational systems are based on value: two objects
are always different even if they have the same value, but two rows in a table are just truth
statements and can theoretically be identical (although there is usually a primary key).

What happens when two instances of the application query the database concurrently? Here the
DB concurrency control features (e.g. transactions) aren't useful anymore... This gets even
worse if the ORM offers a caching layer.

How can we construct an object from data stored in the DB?
* query by example: most fields of all classes must be nullable, and this approach is not expressive enough to support complex queries
* query by API: verbose, not expressive enough for complex JOINs, relies of devs writing DB field names correctly
* query by language: requires to create a language that is a subset of SQL [?]

Finally, OO systems access data in a different way that relational systems: OO systems always get the full set
of attributes for an object, while relational systems project tables onto a subset of attributes [...]

