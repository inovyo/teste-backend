# TESTE - Desenvolvedor Backend
Neste teste você deverá desenvolver uma API para gerenciamento de pesquisas.

Utilize a linguagem que mais tem afinidade e persista os dados em um banco de sua preferência (SQL ou NoSQL).

*Aqui na Inovyo nós utilizamos Python ([FastAPI](https://fastapi.tiangolo.com/)) e Node ([Express](https://expressjs.com/)) para desenvolvimento, e a persistência de dados é em um banco SQL.*

## Quais endpoints minha API precisa ter?
GET
- Consulta de todas as pesquisas;
- Consulta individual de pesquisa com as questões da mesma;

POST
- Criação de pesquisa;
- Criação de questão dentro da pesquisa;

PUT/PATCH
- Atualização de pesquisa;
- Atualização de questão;

DELETE
- Remoção de pesquisa;
- Remoção de questão;

## Campos 
**Pesquisa**
Variável | Tipo
------------ | -------------
`id` | `int`
`title` | `string`
`status` | `lista` [open, closed]
`created_at` | `data`
`modified_at` | `data`

**Questão**
Variável | Tipo
------------ | -------------
`id` | `int`
`surveyid` | `int`
`title` | `string`
`type` | `lista` [radio, checkbox, textarea]
`options` | `objeto` (obrigatório quando o `type` for `radio` ou `checkbox`)
`created_at` | `data`
`modified_at` | `data`

## Entrega
- Crie um `README.md` com: comandos necessários para rodar a aplicação (bastando copiar/colar no terminal), documentação da API e testes;
- Publique sua API no [GitHub](http://github.com/) e envie a URL para o e-mail [talentos@inovyo.com](mailto:talentos@inovyo.com?subject=Teste%20Backend) com o título `Teste Backend`.

## Boa sorte!