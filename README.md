# Fatec-Atividade-01-BD

Repositório para Anexo referente a Banco de Dados não relacional 			

![image](https://user-images.githubusercontent.com/106127869/226207195-5825a910-b5ae-4366-88cf-d8a975589310.png)
Comando: show dbs	| Função: Mostra todos os BD's criados no MongoDB 

--------------------------------------------------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/106127869/226207200-77902f65-8f67-4765-bc89-7e25c887061e.png)
Comando: use aula | Função: fixa o banco selecionado para uso de criação/pesquisa 

--------------------------------------------------------------------------------------------------------------------


![image](https://user-images.githubusercontent.com/106127869/226207206-84f1e62e-0261-450b-9e9b-69f84f40866c.png)
Comando: show collection | Função: Mostra as coleções criadas no banco de dados atual

--------------------------------------------------------------------------------------------------------------------


![image](https://user-images.githubusercontent.com/106127869/226207209-7e5733e2-1437-402b-9781-2e253f6959c7.png)
Comando: db.livros.count() | Função: Conta todos os itens da coleção 

--------------------------------------------------------------------------------------------------------------------


![image](https://user-images.githubusercontent.com/106127869/226207213-a6b8d854-7a91-4204-9d25-f6731133a1f6.png)
Comando: db.livros.count({pageCount:{$lte: 100}}) | Função: Conta dos os livros que tenha a quantidade de paginas menor igual que 100 

--------------------------------------------------------------------------------------------------------------------


![image](https://user-images.githubusercontent.com/106127869/226207217-9c042e86-7b02-4840-b35e-2c30e83f4251.png)
Comando: db.livros.count({isbn:{$gt: "1933988746"}}) | Função: Retornará os isbn maiores que 1933988746 

--------------------------------------------------------------------------------------------------------------------


![image](https://user-images.githubusercontent.com/106127869/226207233-b133f675-c61b-441d-9f73-af0cc004938d.png)
Comando: db.livros.find({title: /G/, isbn: {$tle:1617200000}}) | Função: Consulta os livros com o campo isbn menor ou igual a "1617200000" que tenha o titulo que começa com "G" 

--------------------------------------------------------------------------------------------------------------------


![image](https://user-images.githubusercontent.com/106127869/226207276-974cf680-ed07-489b-81f8-ac2b984542c3.png)
![image](https://user-images.githubusercontent.com/106127869/226207286-b215adc2-ef56-40f1-9f4f-283d7dfa26fe.png)
Comando: db.livros.find({isbn: "10"}}).limit(2) | Função Consulta os libros com o isbn = 10, mas só irá aparecer 2 livros(.limit) 

--------------------------------------------------------------------------------------------------------------------


![image](https://user-images.githubusercontent.com/106127869/226207292-5f464907-ab57-4261-a756-da3aed3b7719.png)
Comando: db.livros.find({title: /Windows/}).count() | Função: Conta os livros que tenha como titulo Windows 

--------------------------------------------------------------------------------------------------------------------


![image](https://user-images.githubusercontent.com/106127869/226207296-c48fe426-01f0-4751-a87d-ac03b241c73c.png)
![image](https://user-images.githubusercontent.com/106127869/226207298-722790c9-cd06-4d5f-bf0e-32c57df8793c.png)
Comando: db.livros.find({}).sort({"pageCount": -1}).limit(2) | Função: Consulta os livros pela quantidade de folhas decrescente(.sort) com o limite de visualização de 2 itens(.limit)
