# Warmup: SQL Joins to Knex Joins

## Resources

* [Knex Docs](https://knexjs.org/)
* [Knex Query Lab](http://michaelavila.com/knex-querylab/)

## Questions

* What knex method do you use to make an inner join?
  - .innerJoin()
  - .join()

* What knex method do you use to make a left join?
  - .leftJoin()

* What knex method do you use to make a right join?
  - .rightJoin()

* What knex methods do you use to make outer joins?
  - .fullOuterJoin()
  - .leftOuterJoin()
  - .rightOuterJoin()

* STRETCH: Construct a sample knex query for a many-to-many inner join

```js
knex.select('*').from('user')
  .innerJoin('user_account', 'user.id', 'user_account.user_id')
  .innerJoin('account', 'account.id', 'user_account.account_id')
  .then(responseFromDb => {
    // do something with response
    console.log(responseFromDb)
    res.json({
      users: responseFromDb
    })
  })
```

* STRETCH: Construct a sample knex query for a many-to-many inner join using a WHERE clause