# NOME DO PROJETO

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

## Entidades, Tabelas ou ColeÃ§Ãµes utilizadas

- Nome das tabelas (bancos sql) ou coleÃ§Ãµes (bancos nosql) utilizadas

OperaÃ§Ãµes implementadas para cada entidade

| Entidade| Create | Read | Update | Delete |
| --- | --- | --- | --- | --- |
| Donation | X |  X  | X | X |
| Tag |  |    |   |  |
| User | X |    |  |  |

## Rotas da API REST utilizadas


| Método HTTP | URL |
| --- | --- |
| GET | api/entidade1/|
| POST | api/entidade2 |