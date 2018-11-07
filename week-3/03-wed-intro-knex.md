# Warmup: Query Builders - Knex

## Resources

* [Intro to Knex](https://github.com/gSchool/node-curriculum/blob/master/Knex/README.md)
* [Learn - Knex Migrations & Seeds Overview](https://learn-2.galvanize.com/cohorts/757/blocks/23/content_files/Migrations%20and%20Seeds/00-overview.md)
* [Learn - Purpose of Migrations & Seeds](https://learn-2.galvanize.com/cohorts/757/blocks/23/content_files/Migrations%20and%20Seeds/01-why.md)
* [Learn - Migration Setup](https://learn-2.galvanize.com/cohorts/757/blocks/23/content_files/Migrations%20and%20Seeds/02-create.md)

## Goals/Questions

* What is knex.js?
  - 3rd party JS library
  - Builds SQL commands
  - Sends the commands to relational DBMS (query building)
  - Also helps us set up initial state of DB through migrations and seeds
    * Schema and starter data
    * Creating tables and getting initial data into those tables

* Why is knex useful?
  - JS, promise based syntax for querying
  - Migrations, seeds
  - Cross relational database functionality

* What is a migration?
  - SCHEMA
  - Structured way to manage the tables in your database
  - Create tables initially
  - Drop those tables if we need to
  - Alter tables in the future if needed

* Why are migrations useful?
  - We're not 'lost in the woods' if we need to drop tables, or drop db
  - Helpful for collaboration
  - Helpful if we get a new computer
  - Not as constrained to one environment

* What is a seed?
  - Starter data
  - Pseudo data used to test

* Why are seeds useful?
    - Testing
    * Initial 'state' of database and application
    * Helpful for collaboration

* Install knex globally:
  `npm install -g knex`