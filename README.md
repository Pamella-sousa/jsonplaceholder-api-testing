# API Automation Project - JSONPlaceholder

Este repositório contém uma suíte de testes automatizados desenvolvida para a API JSONPlaceholder.
O projeto tem como objetivo demonstrar competências em Quality Assurance, com foco em integridade de dados, validação contratual, regras de negócio, performance e resiliência da API.


**O projeto foi organizado em 7 coleções estratégicas, cobrindo diferentes camadas de teste e comportamentos da API:**

* 01 - Posts (Full CRUD)

Testes completos do ciclo de vida do recurso:

GET – Recuperação de recurso

POST – Criação

PUT – Atualização completa

PATCH – Atualização parcial

DELETE – Remoção

Validação de status codes, estrutura de resposta e tempo de execução.


* 02 - Users (Contract Testing)

Implementação de JSON Schema Validation para assegurar que a estrutura da resposta respeite o contrato estabelecido:

Validação de tipagem

Campos obrigatórios

Estruturas aninhadas (address, geo)

Teste de usuário inexistente


* 03 - Comments (Nesting)

Validação de relacionamentos hierárquicos entre recursos:

Listagem de comentários por Post

Filtro por postId

Criação de comentário

Validação de recurso inexistente


* 04 - Albums (Data Logic)

Verificação de integridade lógica e consistência de dados:

Listagem de álbuns

Recuperação de fotos por álbum

Criação de novo álbum

Atualização parcial de título


* 05 - Todos (State Testing)

Testes baseados em estados lógicos:

Listagem geral

Filtro por tarefas concluídas

Criação de tarefa

Exclusão

Validação de regras condicionais baseadas em propriedades booleanas.


* 06 - Query Filters

Validação de precisão em filtros dinâmicos aplicados via Query Parameters:

Filtro de posts por userId

Filtro de comentários por email

Filtro de álbuns por userId

Filtro combinado

Validação de retorno vazio


* 07 - Negative Scenarios

Testes de resiliência e comportamento sob falhas:

Recurso inexistente (404)

Criação com usuário inválido

Atualização de recurso inexistente

------------------

**Tecnologias e Habilidades Aplicadas**


Postman	-> Orquestração de requisições e organização modular

JavaScript ->	Scripts dinâmicos para validação de regras de negócio

JSON Schema	-> Garantia de conformidade estrutural da API

HTTP Methods ->	Implementação prática do padrão REST

SLA Validation	-> Verificação de tempo de resposta

------------------

**Diferenciais do Projeto**

Tratamento de exceções para respostas inconsistentes (texto vs JSON)

Validação de status codes e payloads

Monitoramento de tempo de resposta (SLA)

Estrutura modular organizada por domínio funcional

Separação clara entre cenários positivos e negativos

------------------

**Como Executar**

1. Importar o arquivo da Collection no Postman
2. Selecionar o ambiente configurado
3. Executar via Collection Runner
4. Analisar os resultados no painel de testes

------------------

**Desenvolvido por Pamella Sousa
Quality Assurance Analyst**
