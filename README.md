# DOA AÍ

O tema do trabalho é referente a uma aplicação web que visa conectar pessoas que pretendem doar seus itens para outras que estão precisando. Uma pessoa que doa algo, também pode receber doações, por isso, o sistema não cria perfis de usuário distintos; para submeter uma doação ou receber uma doação, os usuários precisam estar logados no sistema; esta aplicação web visa unir as necessidades dos usuários nos diferentes cenários. O sistema fica a cargo de validar com os doadores a doação e aqueles que receberam a doação poderão lhe contactar por algum contato informado por ele no momento do cadastramento no sistema. Algumas das funcionalidades são: Visualizar itens, pesquisar por itens, uso de filtros, aba de favoritos com itens selecionados pelo usuários, cadastro de usuários e items para doação

## Membros da equipe

- Isânio Vitor
- Ewaldo Júnior

## Tecnologias e frameworks utilizados

**Frontend:**

VueJS: Vue.js é um framework JavaScript de código-aberto, focado no desenvolvimento de interfaces de usuário e aplicativos de página única.

**Backend:**

Strapi: O Strapi é um Framework de Gerenciamento de Conteúdo (CMF), que nos oferece facilidades no desenvolvimento de um CMS e/ou no desenvolvimento de software no geral. 

## Papeis ou tipos de usuário do sistema

- Usuário não autenticado
- Usuário autenticado

## Entidades, Tabelas ou Coleções utilizadas

- Nome das tabelas (bancos sql) ou coleções (bancos nosql) utilizadas

Operações implementadas para cada entidade

| Entidade| Create | Read | Update | Delete |
| --- | --- | --- | --- | --- |
| Donation | X |  X  | X | X |
| Tag |  |    |   |  |
| User | X |    |  |  |

## Rotas da API REST utilizadas
## Rotas da API REST utilizadas


### Login
| Método HTTP | URL |
| --- | --- |
| POST | /api/auth/local |

### Registrar
| Método HTTP | URL |
| --- | --- |
| POST | /api/auth/local/register |

### Usuário autenticado
#### Donation
| Método HTTP | URL |
| --- | --- |
| GET | api/donations/|
| GET FindOne | api/donations/:id |
| POST | api/donations/ |
| PUT | api/donations/:id |
| DELETE | api/donations/:id |

#### Tag
| Método HTTP | URL |
| --- | --- |
| GET | api/tags/|
| GET FindOne | api/tags/:id |

#### Upload
| Método HTTP | URL |
| --- | --- |
| GET |  /api/upload/files|
| GET FindOne | /api/upload/files/:id |
| POST |  /api/upload/|

#### Filters
| Método HTTP | URL |
| --- | --- |
| GET |  /donations?populate=*&filters[tag][id][$eq]=:id|
| GET | /donations?populate=*&filters[users_permissions_user][id][$eq]=:id |
| GET | /donations?populate=*&filters[users_liked][id][$in]=:id|

### Usuário público
#### Donation
| Método HTTP | URL |
| --- | --- |
| GET | api/donations/|
| GET FindOne | api/donations/:id |

