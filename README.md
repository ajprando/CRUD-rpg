# RPG CRUD API

API para gerenciamento de personagens e itens mágicos de um RPG.

## Requisitos

- Node.js
- MongoDB
- NestJS

## Instalação

```bash
# Instalar dependências
npm install

# Iniciar o servidor
npm run start:dev
```

## Rotas da API

### Personagens

#### Criar Personagem
```http
POST /personagem
```


#### Listar Todos os Personagens
```http
GET /personagem
```

#### Buscar Personagem por ID
```http
GET /personagem/{id}
```

#### Atualizar Nome do Aventureiro
```http
PUT /personagem/{id}/nome-aventureiro
```


#### Remover Personagem
```http
DELETE /personagem/{id}
```

### Itens Mágicos

#### Criar Item Mágico
```http
POST /item-magico
```



#### Listar Todos os Itens Mágicos
```http
GET /item-magico
```

#### Buscar Item Mágico por ID
```http
GET /item-magico/{id}
```

#### Remover Item Mágico
```http
DELETE /item-magico/{id}
```

### Relacionamentos

#### Adicionar Item Mágico ao Personagem
```http
POST /personagem/{personagemId}/item-magico/{itemMagicoId}
```

#### Listar Itens Mágicos do Personagem
```http
GET /personagem/{id}/item-magico
```

#### Remover Item Mágico do Personagem
```http
DELETE /personagem/{personagemId}/item-magico/{itemMagicoId}
```



## Swagger

A documentação completa da API está disponível no Swagger em:
```
http://localhost:3000/api
``` 

