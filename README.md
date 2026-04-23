# Relatorio de Testes de API - Postman

Este documento descreve a colecao de testes criada para validar os endpoints da API JSONPlaceholder, abrangendo as operacoes fundamentais de GET, POST e PUT.

## Estrutura dos Testes

A colecao foi configurada para validar tres aspectos principais em cada requisicao: o codigo de status da resposta, a integridade do corpo dos dados e os cabecalhos de comunicacao.

| Requisicao | Endpoint | Validações Realizadas |
| :--- | :--- | :--- |
| GET | /posts | Status 200, Formato de Array, Content-Type JSON |
| POST | /posts | Status 201, Persistencia de Dados, Geracao de ID |
| PUT | /posts/1 | Status 200, Atualizacao de Titulo, Presenca de Header Server |

## Detalhamento das Requisicoes

### Listagem de Posts (GET)
Esta operacao recupera a lista de postagens existentes. Os testes garantem que o servidor retorne sucesso e que os dados estejam estruturados corretamente para consumo.

### Criacao de Post (POST)
Esta operacao simula o envio de novas informacoes para o servidor. Os testes validam se o objeto criado mantem as propriedades enviadas e se o servidor confirma o recebimento com o codigo de criacao adequado.

### Atualizacao de Post (PUT)
Esta operacao modifica um registro ja existente. O teste foca em garantir que a alteracao solicitada foi processada e que o servidor respondeu com os metadados esperados.

## Instrucoes de Uso

1. Importe o arquivo Postman_Collection.json no software Postman.
2. Selecione a colecao importada na barra lateral.
3. Utilize a opcao Run Collection para executar todos os testes de forma automatizada.
# 3_BrasilAPI-
