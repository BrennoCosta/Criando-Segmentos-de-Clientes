# Projeto 2 - Criando segmentos de clientes
Segundo projeto do NanoDegree de Engenheiro Machine Learning da Udacity. Consiste em aplicar técnicas de aprendizagem supervisionada sobre os dados coletados pelo censo dos Estados Unidos para ajudar a CharityML (uma instituição de caridade fictícia) a identificar as pessoas com maior probabilidade de doar à causa deles.

# Objetivo do Projeto
Usar técnicas de aprendizagem não supervisionada em dados sobre gastos, coletados de clientes de uma distribuidora atacadista em Lisboa, para identificar segmentos de clientes ocultos nos dados.

# Destaques do Projeto
Este projeto foi desenvolvido para você ter experiência prática com aprendizagem não supervisionada e trabalhar desenvolvendo conclusões para um cliente em potencial com um conjunto de dados do mundo real. Muitas empresas, hoje, colhem uma vasta quantidade de dados sobre clientes, e eles têm um forte desejo de entender o significado das relações escondidos em sua clientela. Ter essa informação pode ajudar o engenheiro da empresa com futuros produtos e serviços que melhor satisfazem as demandas ou necessidades de seus clientes.

O que você aprenderá ao concluir este projeto:

Como aplicar técnicas de pré-processamento, como dimensionamento de atributos e detecção de valores aberrantes.
Como interpretar dados que foram dimensionados, transformados ou reduzidos por meio de PCA.
Como analisar as dimensões de PCA e construir um novo espaço de atributos.
Como agrupar de forma ótima um conjunto de dados para encontrar padrões ocultos.
Como avaliar informações dadas pelos dados segmentados e utilizá-los de maneira significativa.

# Algoritmos Usados no Projeto
DecisionTree e K-Algoritmos.

# Resultados dos Modelos
Nós estabelecemos dois clusters iniciais e o score foi realmente melhor com apenas 2 clusters. Definimos eles como Restaurante e Supermercado, generalizando. Restaurantes, ou estabelecimentos que vendem comidas prontas, precisam ser abastecidos quase todo dia. Precisam de reposição de produtos e sem falta. Acho que esse tipo de cliente não ficaria satisfeito com uma diminuição de entrega de 5 para 3 dias na semana. Já um estabelecimento de supermercado, não precisa de um reabastecimento de mercadorias com tanta frequencia. Talvez de alguns produtos específicos, mas olhando por cima, acho que daria pra fazer um acordo e uma entrega de 3 dias por semana não os afetariam. Com isso, os testes A/B poderiam ser feitos em clientes do segundo segmento, facilitando a escolha dos clientes e os testes também e, depois, verificar a satisfação deles.

# Explicação do Modelo Escolhido
Vou utilizar o K-Means, apesar do MMG ser melhor com dados não lineares, vimos que os 2 primeiros principais componentes são responsáveis pos quase 72% da variância. Então já sabemos que precisaremos de 2 clusters. No caso do modelo MMG, poderíamos aplicar se não tivéssemos um número de cluster já definido.
