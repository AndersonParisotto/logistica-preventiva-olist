Visão Geral do Projeto
Neste projeto, apliquei a metodologia RFM (Recency, Frequency, Monetary) sobre a base de dados do Olist para classificar mais de 96 mil clientes. O objetivo foi identificar quem são os clientes mais fiéis e quem está prestes a abandonar a plataforma, permitindo ações de marketing muito mais precisas.

O Problema de Negócio
Tratar todos os clientes de forma igual é ineficiente e caro. Percebi que o Olist tinha um grande volume de pedidos, mas eu precisava responder:

Quem são os nossos "Campeões"?

Por que tantos clientes compram apenas uma vez e não voltam?

Como podemos reativar clientes que gastaram muito no passado, mas sumiram?

Tecnologias Utilizadas
Linguagem: Python 3.x

Manipulação de Dados: Pandas (Merges complexos e agrupamentos por customer_unique_id)

Matemática/Datas: Datetime (Cálculo de Recência) e Numpy

Visualização: Seaborn e Matplotlib (Gráficos de distribuição de segmentos)

Técnica: Quintis e Lógica de Scoring Customizada.

Insights e Descobertas
Ao realizar a análise, notei comportamentos fundamentais na base:

O "Balde Furado": Percebi que a retenção é o maior desafio. Mais de 93.000 clientes compraram apenas uma vez. Isso mostra que o esforço deve ser em transformar o "Novo Cliente" em "Fiel".

Baleias de Consumo: Identifiquei que, embora o ticket médio seja de R$ 166, o maior gasto individual passou de R$ 13 mil, o que justifica um tratamento VIP para esse grupo.

Saúde da Base: Notei que os grupos de "Clientes Perdidos" e "Novos" são quase do mesmo tamanho, indicando que a empresa ganha clientes na mesma velocidade que os perde.

Ações Recomendadas (Plano de Ataque)
Criei uma matriz de ação para cada segmento identificado:

Campeões: Programa de fidelidade e mimos exclusivos.

Novos Clientes: Cupom de desconto para a segunda compra (estimular a recorrência).

Clientes em Risco: E-mails de "Sentimos sua falta" com ofertas personalizadas.

Perdidos: Campanhas agressivas de reativação em datas sazonais (Black Friday).

Conclusão
Este projeto prova que a análise de dados é o motor para o crescimento (Growth). Ao segmentar a base, saímos de um "disparo de e-mail em massa" para uma estratégia onde cada cliente recebe o incentivo certo para o seu momento de compra.
