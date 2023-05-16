Caso de Uso: Monitorar Estoque

Ator Principal: Almoxarifado e Estocagem

Outros Atores: N/A

Descrição: O departamento de Almoxarifado e Estocagem monitora o estoque de materiais necessários para a produção de concreto.

Requisitos do Sistema:

    R7: O sistema deve permitir o monitoramento dos níveis de estoque dos componentes (cimento, areia, cascalho e água).
    R8: O sistema deve fornecer alertas quando os níveis de estoque ficarem abaixo do limite mínimo.

Funções Básicas:

    FB5: Monitorar níveis de estoque
    FB6: Enviar alertas de estoque baixo

Fluxo Principal:

    1 - O departamento de Almoxarifado e Estocagem acessa a funcionalidade de monitoramento de estoque.
    2 - O sistema exibe o painel de controle de estoque, mostrando os níveis atuais de estoque dos componentes.
    3 - O departamento de Almoxarifado e Estocagem analisa os níveis de estoque dos componentes e verifica as informações no painel de controle de estoque.
    4 - O sistema verifica se os níveis de estoque estão abaixo do limite mínimo.
    5 - O departamento de Almoxarifado e Estocagem identifica os componentes com estoque baixo.
    6 - O sistema envia um alerta de estoque baixo para os responsáveis ou departamentos relevantes.
    7 - O departamento de Almoxarifado e Estocagem solicita a reposição de estoque para os componentes identificados com estoque baixo.
    8 - O caso de uso é encerrado

Fluxos Alternativos: N/A

Pré-condições: N/A

| Ação do Ator         | Resposta do Sistema                 | Função Básica / Requisito |
|----------------------|-------------------------------------|--------------------------|
| O departamento de   | 2. O sistema exibe o painel de       | R7                       |
| Almoxarifado e       | controle de estoque, mostrando os   |                          |
| Estocagem acessa a  | níveis atuais de estoque dos         |                          |
| funcionalidade de   | componentes.                         |                           |
| monitoramento de    |                                      |                           |
| estoque.             |                                     |                          |
| O departamento de   | 3. O sistema verifica os níveis      | FB5, R7                  |
| Almoxarifado e       | de estoque dos componentes e exibe  |                          |
| Estocagem analisa os | as informações no painel de         |                          |
| níveis de estoque.   | controle de estoque.                |                          |
| O departamento de   | 5. O sistema verifica se os níveis   | FB6                      |
| Almoxarifado e       | de estoque estão abaixo do limite   |                          |
| Estocagem identifica | mínimo.                             |                          |
| componentes com     |                                     |                          |
| estoque baixo.       |                                     |                          |
| O departamento de   | 6. O sistema envia um alerta de      | FB6,R8                    |
| Almoxarifado e       | estoque baixo para os responsáveis   |                          |
| Estocagem solicita   | ou departamentos relevantes.        |                          |
| reposição de         |                                     |                          |
| estoque para os     |                                     |                          |
| componentes com     |                                     |                          |
| estoque baixo.       |                                     |                          |
