### Desafio intelbras

Escrever uma aplicação em Lua usando orbit (http://keplerproject.github.io/orbit) que responda as seguintes URLs.

#### Receber um GET na url http://localhost/api/user/1
Lê um arquivo e retorna o seu contêudo no formato json, exemplo:

users.txt tem o conteúdo abaixo:
```
{id  = 1, name = 'Jairo', age = 30}
```
retorna:
```
{
	"id": 1,
	"name": "Jairo",
	"age": 30
}
```
#### Receber um POST na url  http://localhost/api/user
Add no arquivo o conteúdo do JSON recebido, exemplo:

```
{
	"id": 2,
	"name": "Roberto",
	"age": 31
}
```
users.txt
```
{id  = 1, name = 'Jairo', age = 30},
{id  = 2, name = 'Roberto', age = 31}
```

#### Receber um PUT na url http://localhost/api/user/id
Receber um JSON conforme spec do POST, gravar o 'novo conteúdo' no arquivo caso exista o id enviado.

#### Receber um DELETE na url http://localhost/api/user/id
excluir item associado ao id.

O Webservice deve respeitar as boas praticas do padrão REST usando a rfc2616
#### Bonus: 
 - Testes unitários.
 - Testes de API.
 - Documentar o código e gerar documentação via alguma ferramenta.
