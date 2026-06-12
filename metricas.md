# Obtenção e análise das métricas
A partir dos dados iniciais obtidos (personagens e suas relações uns com os outros), o grafo com 1175 arestas foi criado e partimos para a análise das métricas.

### 📑 Métricas analisadas

- Degree (grau)
- Betweenness centrality (centralidade de intermediação)
- Diameter (diâmetro)
- Radius (raio)
- Eccentricity (excentricidade)
- Clustering (coeficiente de aglomeração)
- Degree assortativity (Coeficiente de assortatividade baseado no grau)
- Density (densidade)

### ✒️ Degree
O *degree* indica quantas conexões diretas cada personagem possui. Coriolanus Snow possui 75 conexões diretas com
outros personagens, ou seja, ele está conectado a 50% dos personagens da saga de Jogos Vorazes.

| Personagem | Degree |
| :--- | :--- |
| Coriolanus | 75 |
| Katniss | 66 |
| Peeta | 53 |
| Sejanus | 36 |
| Finnick | 34 |
| Gale | 33 |
| Lucy Gray | 33 |
| Caesar | 30 |
| Hilarius | 27 |
| Felix | 26 |

### ✒️ Betweenness centrality
O cálculo da centralidade de intermediação se dá pela soma dos menores caminhos que passam pelo vértice.

| Personagem | Betweenness Centrality |
| :--- | :--- |
| Coriolanus | 6007 |
| Katniss | 4270 |
| Caesar | 1183 |
| Peeta | 769 |
| Gale | 651 |
| Tigris | 556 |
| Plutarch | 520 |
| Finnick | 272 |
| Sra Everdeen | 269 |
| Lucy Gray | 186 |

### ✒️ Métricas gerais do grafo

| Métricas gerais do grafo | Valor |
|--------------------------|-------|
| Diameter                 | 4     |
| Radius                   | 3     |
| Eccentricity             | 3-4   |
| Clustering               | 0,76  |
| Degree Assortativity     | -0,14 |
| Density                  | 0,11  |

O **diâmetro do grafo**, isto é, o
maior entre os menores caminhos, possui valor 4, o que
significa que, em geral, os personagens estão bem próximos
uns dos outros. 

O **raio do grafo** mede 3, representando o
menor entre os maiores caminhos. 

A métrica **eccentricity
(excentricidade)** combina essas duas métricas, diâmetro e
raio, em uma só, sendo o diâmetro o valor máximo de
eccentricity e o raio, o seu valor mínimo. Assim, tem-se que
o caminho máximo entre um personagem e outro varia de 3
a 4.

O **coeficiente de aglomeração (clustering)** é de
0.76, o que significa que há grupos de personagens com
fortes interações na borda da rede

Também foi calculado o **coeficiente de
assortatividade baseado no grau (degree assortativity)**. Essa
métrica é responsável por medir a tendência dos vértices de
degree alto a se conectarem com outros vértices que
também possuem um degree alto. Sendo r igual ao
coeficiente de assortatividade baseado em grau, temos que
se r é menor que 0, então o grafo é dissortativo, ou seja, os
vértices se conectam com outros independente do seu
degree ser semelhante ou não. Esse é o caso do grafo de
Jogos Vorazes, uma vez que o valor de r é igual a -0,14.

A **densidade do grafo** de Jogos Vorazes é de 0,11, o que
significa que o grafo, em geral, pode ser considerado
esparso.

### ✔️ Conclusões 

Através da análise das métricas obtidas a partir da
construção do grafo, foi possível **confirmar a hipótese inicial**
de que o personagem Coriolanus Snow é de fato o
personagem mais influente da saga, possuindo não somente
o maior número de conexões, como também de
intermediação. Superando, inclusive, os personagens
principais da saga que, por senso comum, costumam ser os
personagens com maior número de conexões.

Ainda que a métrica de densidade indique que o grafo é
esparso, a introdução de novas obras, como é o caso de
Sunrise on the Reaping (“Nascer do sol na colheita”, em
tradução livre) que está previsto para ser lançado em 2025,
deve cumprir o trabalho de gerar novas conexões que ainda
não temos conhecimento, aumentar a densidade do grafo, e
portanto, tornar o universo fictício criado por Collins ainda
mais completo.
