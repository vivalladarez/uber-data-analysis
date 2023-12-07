# uber-data-analysis 🚘 

Este projeto tem como objetivo analisar dados das viagens do Uber para identificar padrões, tendências ou insights que possam melhorar a eficiência das viagens, compreender o comportamento dos usuários ou otimizar a operação em áreas específicas. A análise se concentra em segmentar usuários com base em seus padrões de viagem sem rótulos predefinidos, sendo um problema não supervisionado. Todos os dados utilizados são provenientes do consumo da própria autora do projeto que consente a liberação dessas informações, disponibilidados pela Uber através do aplicativo.

### Premissas sobre o Problema
1.   Viagens mais longas podem ter uma correlação com um valor de tarifa mais alto;
2.   A duração da viagem dependendo do tráfego na cidade naquele momento;
3.   A velocidade média das viagens depende do horário/tráfego no momento


Atributos | Definição
--- | :---:
`Cidade` | Nome da cidade onde a viagem ocorreu.
`Tipo de Produto` | Categoria ou tipo específico de serviço oferecido pela Uber, como UberX, Uber Black, Uber Pool, etc.
`Status da Viagem ou Pedido` | Indicação do estado atual da viagem ou do pedido, como "Solicitado", "Em andamento" ou "Concluído".
`Tempo de Solicitação` | Momento em que o usuário fez a solicitação da viagem.
`Hora de Início da Viagem` | Horário em que a viagem começou.
`Início da Viagem Lat./Long.` | Coordenadas de latitude e longitude do ponto de partida da viagem.
`Endereço Inicial da Viagem` | Localização inicial (endereço) de onde a viagem foi solicitada.
`Horário de Entrega` | Horário em que a viagem foi finalizada ou entregue.
`Lat. de Desembarque` | Coordenadas de latitude e longitude do ponto de desembarque ou destino da viagem.
`Entrega de GNL` | Possível indicação se a entrega foi feita através de algum serviço específico chamado GNL.
`Endereço de Entrega` | Localização de destino da viagem (endereço).
`Distância (milhas)` | Distância percorrida durante a viagem, frequentemente medida em milhas.
`Valor da Tarifa` | Montante cobrado ao usuário pela viagem.
`Moeda Tarifária` | A moeda na qual a tarifa foi cobrada (por exemplo, dólar, euro, etc.).

# Análise de dados & Visualizações

Nesta etapa, será realizada uma análise exploratória dos dados para observar seus padrões e tendências, respondendo às seguintes perguntas:

1. Como a distância percorrida influencia no valor da tarifa e na duração da viagem?
2. Qual foi o total de viagens completadas nos anos anteriores?
3. Quais foram os valores máximos, mínimos e médios da tarifa, distância percorrida e duração da viagem?
4. Qual foi o montante total das tarifas cobradas por mês e por ano?
5. Quantas viagens foram realizadas por ano, divididas pelos dias da semana?
6. Qual foi a velocidade média das viagens realizadas?

# Clusterização

A clusterização é uma técnica de aprendizado não supervisionado que agrupa dados semelhantes em conjuntos, chamados de clusters. No contexto deste projeto usaremos a clusterização para segmentação de perfis de clientes.
Com base na coleta, limpeza e análise exploratória já realizada nos dados, nesta etapa será realizo os seguintes passos:

1. **Seleção de características (features)**: Escolha as características mais relevantes para a análise de clusterização.
2. **Normalização ou padronização**: Em alguns casos, é necessário normalizar ou padronizar os dados para que todas as características tenham o mesmo peso.
3. **Aplicação do método de Elbow**: Técnica usada na análise de clusterização para determinar o número ideal de clusters em um conjunto de dados.
4. **Configuração de parâmetros e execução do algortimo KMeans**: Ajustar os parâmetros do algoritmo de acordo com as características dos dados.
5. **Avaliação dos resultados e Interpretação dos clusters**: Analise e interprete os clusters gerados para extrair insights úteis.
