writeCode

Write code to:-

- create a database named `sports`.
<!-- use sports -->
- list all databases present in local mongod server.
<!-- show dbs -->
- create 3 collections named `cricket`, `football`, `TT` in sports databse.
  <!--db.crateCollection("cricket")  -->
  <!-- db.createCollection("football") -->
  <!-- db.createCollection("TT") -->
- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
  <!-- db.cricket.createCollections([{name:"Dhoni", age:38, email:"Dhonicsk@gmail.com",team:"csk",     bid_price:10000000"},{name:"Virat kohli", age:34, email:"viratrcb@gmail.com",team:"Rcb",     bid_price:8000000"},
  {name:"Rahul Sharma", age:36, email:"rahulmi@gmail.com",team:"Mi",     bid_price:7000000"},]) -->

  <!-- db.football.createCollections([{name:"Sunil Chhetri", age:38, email:"sunil@gmail.com",team:"India",     bid_price:700000"},{name:"Cristiano Ronaldo", age:35, email:"ronaldo@gmail.com",team:" Manchester United",     bid_price:20000000"},
  {name:"Lionel Messi", age:33, email:"messi@gmail.com",team:"Paris Saint-Germain", bid_price:20000000"},]) -->

  <!-- db.TT.createCollections([{name:"rahul", age:30, email:"rahul@gmail.com",team:"India",     bid_price:200000"},{name:"Raj", age:25, email:"raj@gmail.com",team:"India",     bid_price:10000"},
  {name:"Nitish", age:33, email:"nitish@gmail.com",team:"India", bid_price:400000"},]) -->

- list all collections in sports database.
<!-- show collections -->
- rename `TT` collection to `tennis`.
<!-- db.adminCommand({renameCollection:"sports.TT ",to:"sports.tennis"})-->
- create a capped collection called `khokho` which should have max 3 documents.
  <!-- db.createCollection('Khokho',{capped:true,size:1024,max:3}) -->
  Try inserting more than 3 and see what happens?
    <!-- db.Khokho.createCollections([{name:"suraj", age:20, email:"suraj@gmail.com",team:"India"},{name:"sumit", age:25, email:"sumit@gmail.com",team:"India"},
    {name:"Niraj", age:23, email:"niraj@gmail.com",team:"India"},{name:"Arun", age:27, email:"arun@gmail.com",team:"India"}])  -->
- check whether a collection is capped or not?
<!-- db.Khokho.isCapped() -->
- drop all documents from `football` collection.
<!-- db.football.drop() -->
- delete cricket collection completely.
<!--db.cricket.drop()  -->
- delete sports database.
<!-- db.dropDatabase() -->
- check which database you are connected to ?
<!-- db -->
- connect to test database
<!-- use test -->
