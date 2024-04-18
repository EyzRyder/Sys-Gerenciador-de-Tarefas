# Sys Gerenciador de Tarefas

## Descrição
Este projeto consiste em um sistema gerenciador de tarefas, desenvolvido para auxiliar na organização da rotina diária. Com ele, é possível cadastrar, visualizar, editar e excluir tarefas de forma simples e eficiente.

### Funcionalidades
CRUD de Tarefas: Permite criar, ler, atualizar e excluir tarefas da lista.
Interface Web: Disponibiliza uma interface web para interação com o sistema.
Flexibilidade de Implementação: Pode ser desenvolvido como uma Web API ou utilizando o padrão MVC, de acordo com a preferência do desenvolvedor.

### Tecnologias
- Web API
- Entity Framework
- C#
- .Net

![Diagrama da classe Tarefa](diagrama.png)

Não se esqueça de gerar a sua migration para atualização no banco de dados.

## Métodos

**Swagger**

![Métodos Swagger](swagger.png)


**Endpoints**


| Verbo  | Endpoint                | Parâmetro | Body          |
|--------|-------------------------|-----------|---------------|
| GET    | /Tarefa/{id}            | id        | N/A           |
| PUT    | /Tarefa/{id}            | id        | Schema Tarefa |
| DELETE | /Tarefa/{id}            | id        | N/A           |
| GET    | /Tarefa/ObterTodos      | N/A       | N/A           |
| GET    | /Tarefa/ObterPorTitulo  | titulo    | N/A           |
| GET    | /Tarefa/ObterPorData    | data      | N/A           |
| GET    | /Tarefa/ObterPorStatus  | status    | N/A           |
| POST   | /Tarefa                 | N/A       | Schema Tarefa |

Esse é o schema (model) de Tarefa, utilizado para passar para os métodos que exigirem

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
```
