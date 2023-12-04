# uber-data-analysis 🚘 
Identificar padrões de comportamento e preferências dos usuários do aplicativo Uber por meio da análise de dados de corridas, visando melhorar a oferta de serviços, aprimorar a experiência do usuário e aumentar a eficiência operacional da plataforma.
1. Como a distância percorrida influencia no valor da tarifa e na duração da viagem?
2. Qual foi o total de viagens completadas nos anos anteriores?
3. Quais foram os valores máximos, mínimos e médios da tarifa, distância percorrida e duração da viagem?
4. Qual foi o montante total das tarifas cobradas por mês e por ano?
5. Quantas viagens foram realizadas por ano, divididas pelos dias da semana?
6. Qual foi a velocidade média das viagens realizadas?

### Atributos

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

1. Como a distância percorrida influencia no valor da tarifa e na duração da viagem?

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/bfc99fd6-9f72-40e6-8f92-1eed37a357dc" alt="Image1">
</p>

2. Qual foi o total de viagens completadas nos anos anteriores?

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/9072d3dd-85b3-489a-bc4d-650153f723de" alt="Image2">
</p>

3. Quais foram os valores máximos, mínimos e médios da tarifa, distância percorrida e duração da viagem?

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/9ab3a92d-3bb8-4e8f-8669-d7e9870f7383" alt="Image3">
</p>

4. Qual foi o montante total das tarifas cobradas por mês e por ano?

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/45658ab6-321a-479d-9985-17a0ce7c95d1" alt="Image4">
</p>

5. Quantas viagens foram realizadas por ano, divididas pelos dias da semana?

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/0d6b5c70-0fd9-4311-ae03-43825275bfb8" alt="Image5">
</p>

6. Qual foi a velocidade média das viagens realizadas?

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/57a5da78-5dea-4a99-a93b-878e27c88a29" alt="Image6">
</p>

# Clusterização

A clusterização é uma técnica de aprendizado não supervisionado que agrupa dados semelhantes em conjuntos, chamados de clusters. No contexto deste projeto usaremos a clusterização para segmentação de perfis de clientes.

Com base na coleta, limpeza e análise exploratória já realizada nos dados, realizaremos as seguintes etapas:
1. **Seleção de características (features)**: Escolha as características mais relevantes para a análise de clusterização.
2. **Normalização ou padronizaçã**o: Em alguns casos, é necessário normalizar ou padronizar os dados para que todas as características tenham o mesmo peso.
3. **Aplicação do método de Elbow**: Técnica usada na análise de clusterização para determinar o número ideal de clusters em um conjunto de dados.
4. **Configuração de parâmetros e execução do algortimo KMeans**: Ajustar os parâmetros do algoritmo de acordo com as características dos dados.
5. **Avaliação dos resultados e Interpretação dos clusters**: Analise e interprete os clusters gerados para extrair insights úteis.

### **1. Seleção de características (features)**
Para esta etapa iremos calcular a matriz de correlação do dados, que consiste em uma tabela que mostra as relações entre todas as variáveis de um conjunto de dados, representando numericamente a intensidade e a direção dessas relações.

A correlação é uma ferramenta importante para entender a relevância e a influência das variáveis no modelo estatístico, isto é, um guia para escolher quais atributos serão escolhidos para o modelo.
<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/2e320746-09ca-4fba-a3ca-aaebe78bc87c" alt="Image7">
</p>

### **2. Normalização ou padronização**
StandardScaler é uma técnica de pré-processamento comum usada para normalizar e padronizar os dados antes da aplicação de algoritmos de aprendizado de máquina. StandardScaler é usado para padronizar os recursos (features) de um conjunto de dados, transformando-os para que tenham uma média de zero e um desvio padrão de um. Isso é importante porque muitos algoritmos de aprendizado de máquina assumem que os dados estão normalmente distribuídos e têm média zero e variância unitária.

### **3. Aplicação do método de Elbow**
Tecnica utilizada quando você não tem um número específico de clusters e deseja encontrar o valor mais apropriado com base na estrutura dos dados, identificando um ponto onde a adição de mais clusters não fornece um ganho significativo na explicação da variância dos dados.

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/b40dc21d-88c8-4480-ab32-c01aa8504f29" alt="Image7">
</p>

### **4. Configuração de parâmetros e execução do algortimo KMeans**
O algoritmo K-Means é um dos métodos mais populares de clustering e agrupamento de dados não supervisionados. Ele é utilizado para dividir um conjunto de dados em k grupos (clusters) baseados em características similares, seu funcionamento consiste na: 
1. Inicialização dos centróides: O algoritmo começa selecionando aleatoriamente k pontos como centróides iniciais (representantes dos clusters).

2. Atribuição de pontos aos clusters: Para cada ponto de dados, calcula-se a distância entre o ponto e os centróides. O ponto é atribuído ao cluster representado pelo centróide mais próximo.

3. Atualização dos centróides: Uma vez que todos os pontos foram atribuídos aos clusters, os centróides são recalculados como a média de todos os pontos atribuídos a cada cluster.

4. Repetição: Os passos 2 e 3 são repetidos iterativamente até que a atribuição dos pontos aos clusters não mude ou uma condição de parada seja atingida (como um número máximo de iterações).

Com base no resultado obtido pelo método de Elbow escolheu-se o parâmetro K = 4.

### **5. Avaliação dos resultados e Interpretação dos clusters**

*   Índice de silhueta e inércia: Métricas para avaliar a qualidade dos clusters formados pelo algoritmo K-Means
*   Gráfico de Dispersão: Usaremos essa visão para destar cada cluster com diferentes cores ou marcadores para compreender a separação e a sobreposição dos grupos.
*   Perfil dos Clusters: Analise das características médias de cada cluster para entender suas particularidades, realizando a comparação de médias, desvios padrão e distribuições de variáveis em cada cluster.

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/4397ec97-67ac-4556-950d-26d2b79c8c22" alt="Image7">
</p>

### Cluster 0 | Regular
Viagens tradizionais e proporcionais ao histórico
### Cluster 1 | Viajante 
Corridas mais distantes, com longa duração e mais caras
### Cluster 2 | Altas Tarifas
Viagens realizadas com alta dinamica no aplicativo


