Logística Preventiva: Predição de Atrasos com Machine Learning
Visão Geral do Projeto
Neste projeto, analisei a malha logística do Olist para identificar por que as entregas atrasam e como podemos prever esses gargalos antes que o cliente reclame. Saí de uma análise descritiva básica para a construção de um modelo de Machine Learning capaz de sinalizar pedidos de alto risco.

O Problema de Negócio
O atraso na entrega é o principal motivo de churn (perda de cliente) no e-commerce. Percebi que olhar apenas para a média de atrasos não era suficiente. Precisávamos de uma ferramenta que:

Identificasse as variáveis que mais pesam no atraso.

Previsse o atraso mesmo em uma base de dados onde 93% das entregas chegam no prazo (desbalanceamento de classes).

Tecnologias Utilizadas
Linguagem: Python 3.x

Bibliotecas de Dados: Pandas e Numpy

Machine Learning: Scikit-Learn (Random Forest Classifier)

Visualização: Seaborn e Matplotlib

Métricas de Avaliação: Recall, Precision, F1-Score e Matriz de Confusão.

Insights e Descobertas
Durante o desenvolvimento, percebi alguns pontos críticos na operação:

Anomalia Geográfica: Notei que estados do Norte (AC, AM, RO) possuem fretes caríssimos, mas entregam muito antes do prazo estimado (margens de segurança excessivas).

O Peso do Frete: O valor do frete sozinho representa 38% da importância na decisão do modelo de atraso.

Dificuldade Física: Peso e dimensões do produto somam 62% de influência, provando que o gargalo é operacional e de manuseio.

O Modelo Preditivo
Utilizei o algoritmo Random Forest. O grande desafio foi o desequilíbrio dos dados (apenas ~7% de atrasos).

Estratégia: Apliquei a técnica de class_weight='balanced'.

Resultado: Consegui dobrar a capacidade de detecção de atrasos (o Recall saltou de 13% para 24%), criando um modelo que realmente "enxerga" o problema em vez de apenas chutar o óbvio.

Conclusão
Este projeto demonstra como a Ciência de Dados pode ser aplicada para transformar a logística de reativa (tratar a reclamação) em preventiva (antecipar o problema). Com os pesos das variáveis identificados, a operação pode focar em otimizar o transporte de produtos pesados ou revisar rotas de frete caro.
