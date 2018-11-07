# Warmup: Knex Query Builder

## Resources

* [Knex Docs - Query Builder](https://knexjs.org/#Builder)

## Questions

* How would you construct the equivalent of a `SELECT * FROM tablename` query using Knex?

```js
knex.select('*')
  .from('tablename')
  .then(response => {
    console.log(response)
  })
```

* How would you construct the equivalent of a `SELECT * FROM tablename WHERE id=5` query using Knex?

```js
// Object syntax
knex('tablename')
  .where({
    id: 5
  })
  .then(response => {
    console.log(response)
  })

// Key, value syntax
knex('tablename')
  .where('id', 5)
  then(response => {
    console.log(response)
  })
```

* How would execute similar queries as above but only select particular columns?