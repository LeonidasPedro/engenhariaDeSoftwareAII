
Requisitos basicos:

    R1 - O sistema deve permitir que os clientes solicitem pedidos de concreto, especificando o tipo e a quantidade necessários.
    R2 - O sistema deve permitir que o departamento de vendas processe e escalone os pedidos dos clientes.
    R3 - O sistema deve permitir que o gerente de produção receba os pedidos escalonados e coordene a produção de concreto.
    R4 - O sistema deve permitir que o encarregado do almoxarifado monitore os níveis de estoque de cimento, areia, cascalho e água.
    R5 - O sistema deve enviar notificações ao departamento de compras caso algum item de estoque fique abaixo do nível de segurança.
    R6 - O sistema deve permitir que o departamento de compras faça pedidos de reposição de estoque quando necessário.
    R7 - O sistema deve permitir que o setor de recebimento e distribuição verifique se os pedidos de reposição foram entregues corretamente.
    R8 - O sistema deve permitir que os operadores de máquinas e os auxiliares misturem os componentes necessários para a produção de concreto.
    R9 - O sistema deve permitir o controle do fluxo de trabalho na fábrica, incluindo o uso de balanças, válvulas de medição e controle de descarga de água.
    R10 - O sistema deve permitir que a transportadora da empresa entregue o concreto aos locais de construção conforme especificado nos pedidos.
    R11 - O sistema deve permitir que o departamento financeiro receba o pagamento dos clientes pelos produtos entregues.

Estudo de caso

    Estudo de caso baseado no artigo de modelagem de sistemas industriais, Palazzo e Edelweizz (1998), apud Lutherer E. et al., 1994. 
O estudo representa uma fábrica de concreto que inclui vendas, escritório e a planta industrial. A planta é composta de vários receptáculos de armazenagem de cimento, areia, cascalho e água; um misturador para preparação do concreto; duas balanças para pesar os componentes; uma válvula de medição de componentes; controle de descarga de água; duas esteiras de transporte para levar os ingredientes sólidos ao misturador.
Os clientes preenchem uma ordem de pedido entregue pelo representante com o tipo e quantidade de concreto para entrega em um ou mais dias pela transportadora da empresa. O departamento de vendas escalona a ordem e eventualmente encaminha a indústria para o encarregado de produção. A indústria providência a execução do pedido, através da área de produção e de matéria prima. A produção executa a ordem solicitando materiais que são entregues no local pelo encarregado do almoxarifado e estocagem. O operador das máquinas executa os controles de fabricação tendo como auxiliares os operários responsáveis pela mistura dos componentes e pelo funcionário encarregado do controle de fluxo de trabalho. Caso algum produto da matéria prima fique abaixo do nível de segurança, o encarregado da produção emite ordem para o departamento de compras providenciar o pedido da mercadoria que após a entrega é verificado pelo setor de recebimento e distribuição se está entregue conforme foi feito o pedido. Após a fabricação, o produto é entregue na construção e o cliente efetua o pagamento que é recebido pelo departamento financeiro da indústria.


Casos de Uso

Gerenciamento de pedidos: Os clientes solicitam o tipo e a quantidade de concreto necessários, e os representantes de vendas processam e escalonam os pedidos. O gerente de produção recebe esses pedidos e coordena com a equipe para garantir sua execução.

Controle de estoque : O encarregado do almoxarifado é responsável por monitorar e manter os níveis adequados de cimento, areia, cascalho e água. Se algum desses itens ficar abaixo do nível, o departamento de compras deve ser notificado para providenciar a reposição.

Produção de concreto: Os operadores de máquinas e os trabalhadores auxiliares são responsáveis por misturar os componentes e controlar o fluxo de trabalho na fábrica. Isso inclui o uso de balanças para pesar os componentes, a válvula de medição e o controle de descarga de água.

Transporte e entrega: Após a produção do concreto, a transportadora da empresa é responsável por entregá-lo aos locais de construção, conforme especificado pelos clientes nos pedidos.

Atores

Cliente
Vendas
Produção
Almoxarifado
Compras
Operador
Auxiliar
Transportadora

@startuml
left to right direction

actor Cliente
actor "Departamento de Vendas" as Vendas
actor Produção
actor "Almoxarifado e estocagem" as Almoxarifado
actor Compras
actor Operador
actor Auxiliar
actor Transportadora

rectangle "Gerenciar Pedidos" {
  Cliente -- (Solicitar Pedido)
  Vendas -- (Processar Pedido)
  Produção -- (Coordenar Produção)
  Operador -- (Misturar Componentes)
  Auxiliar -- (Misturar Componentes)
  Transportadora -- (Entregar Concreto)
}

rectangle "Controle de estoque" {
  Almoxarifado -- (Monitorar Estoque)
  Compras -- (Reposição de Estoque)
  (Monitorar Estoque) -- (Atualizar Estoque) : <<include>>
(Reposição de Estoque) -- (Realizar Pedido de Reposição) : <<include>>
(Reposição de Estoque) -- (Verificar Entrega) : <<include>>

}


@enduml

Relação de casos de uso com requisitos:

Gerenciar Pedidos:

    R1: Solicitar Pedido
    R2: Processar Pedido
    R3: Coordenar Produção

Controle de Estoque:

    R4: Monitorar Estoque
    R5: Notificar Estoque Baixo
    R6: Reposição de Estoque
    R7: Verificar Entrega

Produção de Concreto:

    R8: Misturar Componentes
    R9: Controlar Fluxo de Trabalho

Transporte e Entrega:

    R10: Entregar Concreto

Diagrama de Classes




