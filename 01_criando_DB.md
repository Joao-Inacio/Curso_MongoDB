### Para Iniciar o MongoDB
* no CMD:  
`cd   C:\Program Files\MongoDB\Server\6.0\bin`
* Em seguida   
`mongo.exe`  

#### Para criar uma base de dados
`use dbmidias` == dbmidias é o nome da base  
#### Consulta as base de dados
`show dbs`
#### Para inseri dados 
`db.posts.insert({nome: 'José', postagem: 'Bom Produtos!', dia: '31-06-2022'})`  
db == a base de dados  
posts == nome da coleção  
#### Para inseri vários dados  
`db.posts.insert([{nome: 'José', postagem: 'Bom Produtos!', dia: '31-06-2022'}, {nome: 'José', postagem: 'Bom Produtos!', dia: '31-06-2022'}, {nome: 'José', postagem: 'Bom Produtos!', dia: '31-06-2022'}])`  
#### Para recuperar os dados
`db.posts.find()`  
#### Para recuperar os dados mais organizados 
`db.posts.find().pretty`  
#### Para trazer o primeiro registro estruturado  
`db.posts.findOne()`  
#### Recuperando um registro especifico  
`db.posts.find({nome:"José"})`  
#### Filtragem com operador AND simples
`db.posts.find({nome:"José", postagem: "Bons Produtos"})` 
#### Filtragem com operador AND
`db.posts.find({postagem: "Produtos caros", idade: {$lte: 12}})`  
Idade <= 12  
#### Filtragem com operador OR
`db.posts.find({$or:[{nome:"José"}, {nome: "Antonio"}]})`
