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

<p align="center">
  <img src="https://github.com/vivalladarez/uber-data-analysis/assets/146302874/4397ec97-67ac-4556-950d-26d2b79c8c22" alt="Image7">
</p>

### Cluster 0 | Regular
Viagens tradizionais e proporcionais ao histórico
### Cluster 1 | Viajante 
Corridas mais distantes, com longa duração e mais caras
### Cluster 2 | Altas Tarifas
Viagens realizadas com alta dinamica no aplicativo


