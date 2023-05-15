Caso de Uso: Monitorar Estoque

Ator Principal: Almoxarifado e Estocagem

Outros Atores: N/A

Descrição: O departamento de Almoxarifado e Estocagem monitora o estoque de materiais necessários para a produção de concreto.

Requisitos do Sistema:

    RS12: O sistema deve permitir o monitoramento dos níveis de estoque dos componentes (cimento, areia, cascalho e água).
    RS15: O sistema deve fornecer alertas quando os níveis de estoque ficarem abaixo do limite mínimo.

Funções Básicas:

    FB5: Monitorar níveis de estoque
    FB6: Enviar alertas de estoque baixo

**Pré-condições:** N/A

| Ação do Ator         | Resposta do Sistema                 | Função Básica / Requisito |
|----------------------|-------------------------------------|--------------------------|
| O departamento de   | 2. O sistema exibe o painel de       | RS12                     |
| Almoxarifado e       | controle de estoque, mostrando os   |                          |
| Estocagem acessa a  | níveis atuais de estoque dos         |                          |
| funcionalidade de   | componentes.                        |                          |
| monitoramento de    |                                     |                          |
| estoque.             |                                     |                          |
| O departamento de   | 3. O sistema verifica os níveis      | FB5, RS12                |
| Almoxarifado e       | de estoque dos componentes e exibe  |                          |
| Estocagem analisa os | as informações no painel de         |                          |
| níveis de estoque.   | controle de estoque.                |                          |
| O departamento de   | 5. O sistema verifica se os níveis   | FB6, RS15                |
| Almoxarifado e       | de estoque estão abaixo do limite    |                          |
| Estocagem identifica | mínimo.                             |                          |
| componentes com     |                                     |                          |
| estoque baixo.       |                                     |                          |
| O departamento de   | 6. O sistema envia um alerta de      | FB6, RS15                |
| Almoxarifado e       | estoque baixo para os responsáveis   |                          |
| Estocagem solicita   | ou departamentos relevantes.        |                          |
| reposição de         |                                     |                          |
| estoque para os     |                                     |                          |
| componentes com     |                                     |                          |
| estoque baixo.       |                                     |                          |
