writeCode

#### Import data from json file to mongodb database using `mongoimport`

```
mongoimport --host <host_name> --username <user_name> --password <password> --db
DB_NAME --collection COLLECTION_NAME --file cities.json(file location) --jsonArray
(an array of json data)
```

host, username and password are optional fields.

- --host : hostname // defaults to localhost:27017
- --username and --password: optional username and password for db user
- --db: database name
- --collection: Collection name
- --file: file location
- --jsonArray: Passed an array of json objects

## BLOCK-writeCode

Go to `https://www.json-generator.com/`

- generate 40 random json document using the format

```js
// paste this on left panel
[
  '{{repeat(30)}}',
  {
    _id: '{{objectId()}}',
    age: '{{integer(20, 40)}}',
    name: '{{firstName()}} {{surname()}}',
    gender: '{{gender()}}',
    company: '{{company().toUpperCase()}}',
    email: '{{email()}}',
    phone: '+1 {{phone()}}',
    tags: ['{{repeat(2)}}', '{{lorem(1, "words")}}'],
  },
];
```

- download it on `Desktop`
- import it into mongodb `test` database into a collection named `users`
<!-- mongoimport--db test --collection users --file C:\Users\HP\Downloads\generated.json(file location) --jsonArray
(an array of json data) -->

#### Export data from mongodb server to local system in json format using

`mongoexport`command.

```
mongoexport --db test --collection users --out C:\Users\HP\Downloads\generate.json --jsonArray
```

## BLOCK-writeCode

Export `users` collection from `test` database onto `Desktop` in a file named `exported.json`.

#### Import from csv file

```
mongoimport -d test -c users --type csv --file C:\Users\HP\Downloads\generated2.csv(file location) --headerline(including header)
```

## BLOCK-writeCode

Generate mock csv data from `https://www.convertcsv.com/generate-test-data.htm`

- insert this mock csv data into `test` database into a collection named `students`
<!-- mongoimport--db test --collection students --file C:\Users\HP\Downloads\convert.csv(file location) --jsonArray
(an array of json data) -->
