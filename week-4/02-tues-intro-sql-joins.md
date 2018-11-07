# Warmup: Intro to SQL Joins

The goal of this warmup is to familiarize yourself with the concept of SQL joins and the different types of join operations that can be completed. Read through some of the following resources and answer the questions.

## Resources

* First section of: [Learn - SQL Joins and Operators](https://github.com/gSchool/sql-curriculum/blob/master/Joins.md) 
* Types of Joins: [Learn - SQL Joins and Operators](https://github.com/gSchool/sql-curriculum/blob/master/Joins.md#inner--left--right--full-outer-joins)
* [Visual Join](http://joins.spathon.com/)
* [Types of Joins - Alternate Visualizations](https://blog.jooq.org/2016/07/05/say-no-to-venn-diagrams-when-explaining-joins/)

## Questions

* Why do we need to join tables in a relational database?
  - So we don't have have to make each table HUGE and INCLUSIVE of all data that relates to it
  - Normalize
  - Separation of concerns
    * DB is more efficient than our JS code at performing these kinds of operations
  - DRY database
  - Finding matches based on comparisons
    * Primary key to foreign key relationships

* What are the four common types of joins?
  - What does each one do?
  - Why might we use them?
    * Left
      - Returns everything on the left table & just what's matching from the right table
    * Right
      - Returns everything on the right table & just what's matching from the left table
    * Inner
      - Returns whatever is matching from both tables
    * Outer
      - Returns everything from both tables

* SELECT with joins is JUST showing a temporary combination of data (window)