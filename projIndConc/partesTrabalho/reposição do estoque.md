Caso de Uso: Reposição do Estoque

Ator Principal: Compras

Outros Atores: N/A

Descrição: O departamento de Compras realiza a reposição de materiais quando o estoque de algum material atinge o nível de segurança.

Requisitos do Sistema:

    R14: O sistema deve permitir a solicitação de reposição de materiais.
    R15: O sistema deve registrar e controlar as solicitações de reposição.

Funções Básicas:

    FB7: Solicitar Reposição de Materiais
    FB8: Registrar Solicitação de Reposição
    FB9: Acompanhar Status da Solicitação

Pré-condições: N/A

Fluxo Principal:

    1 - O departamento de Compras acessa a funcionalidade de reposição de estoque.
    2 - O sistema exibe a lista de materiais com estoque abaixo do nível de segurança.
    3 - O departamento de Compras seleciona o material que precisa ser reposto.
    4 - O sistema solicita as informações necessárias para a reposição do material, como quantidade e fornecedor.
    5 - O departamento de Compras preenche as informações solicitadas.
    6 - O departamento de Compras confirma a solicitação de reposição.
    7 - O sistema registra a solicitação de reposição com as informações fornecidas.
    8 - O departamento de Compras pode acompanhar o status da solicitação de reposição no sistema.
    9 - Quando a reposição do material chega ao estoque:
    9.1 -  O departamento de Compras atualiza o status da solicitação para "Concluído".
    9.2 -  O sistema registra a chegada da reposição no estoque.
    10 - O caso de uso é encerrado.

Fluxo Alternativo:
N/A

Pós-condições: N/A

| Ação do Ator                         | Resposta do Sistema                            | Função Básica / Requisito |
|--------------------------------------|------------------------------------------------|--------------------------|
| O departamento de Compras            | 2. O sistema exibe a lista de materiais com    | R14                      |
| acessa a funcionalidade de           | estoque abaixo do nível de segurança.          |                          |
| reposição de estoque.                 |                                                |                          |
| O departamento de Compras            | 3. O sistema solicita informações para a       | FB7, R14                 |
| analisa os níveis de estoque.         | reposição do material, como quantidade e        |                          |
|                                       | fornecedor.                                    |                          |
| O departamento de Compras            | 4. O departamento de Compras fornece as         |                          |
| preenche as informações para a       | informações solicitadas.                       |                          |
| reposição do material.                |                                                |                          |
| O departamento de Compras            | 6. O sistema registra a solicitação de         | FB8, R15                 |
| confirma a solicitação de reposição. | reposição com as informações fornecidas.        |                          |
|                                       |                                                |                          |
| O departamento de Compras            | 8. O departamento de Compras pode acompanhar   | FB9                      |
| acompanha o status da solicitação.   | o status da solicitação de reposição no sistema.|                          |
|                                       |                                                |                          |
| Quando a reposição do material       | 9.1. O departamento de Compras atualiza o       |                          |
| chega ao estoque:                    | status da solicitação para "Concluído".         |                          |
| O departamento de Compras            | 9.2. O sistema registra a chegada da reposição |                          |
| atualiza o status da solicitação.    | no estoque.                                    |                          |
