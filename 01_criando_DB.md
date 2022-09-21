### Para Iniciar o MongoDB
* no CMD:  
`cd   C:\Program Files\MongoDB\Server\6.0\bin`
* Em seguida   
`mongo.exe`  

#### Para criar uma base de dados
`use dbmidias` == dbmidias é o nome da base  
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