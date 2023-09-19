## Api

### Criação do projeto
* criando o projeto
``` iniciar um projeto json
npm init -y
```
* json Server
```Instalar biblioteca
    npm install json-server
```
``` package.json
    "scripts": {
        "api": "json-server --watch ./data/db.json --watch"
    },
```
* construir estrutura do json
```
{
    "produtos" : [
        { "id": 1, "nome": "jogo 1", "quantidade": 2, "valor": 100 }
    ],
    "cliente" : [
        { "id": 1, "nome": "joao sousa", "telefone": ""}
    ]
}
```
```rodar projeto
    npm run api
```

### EndPoits da API
#### Produtos
* Cadastrar :: POST
```POST
http://localhost:8080
```
```json post
    {
        "nome": "jogo 2",
        "quantidade": 10,
        "valor": 100
    }
```

* Listar :: GET
```GET
http://localhost:8080
```

* ListarUM :: GET
```GET
http://localhost:8080/1
```

* Deletar :: DELETE
```DELETE
http://localhost:8080/1
```

* Atualizar :: PUT
```PUT
http://localhost:8080/1
```
```json put
    {
        "nome": "jogo 2",
        "quantidade": 10,
        "valor": 100
    }
```

#### Clientes