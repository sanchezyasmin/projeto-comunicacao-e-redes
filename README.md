# Análise Estatística de Redes Complexas com Python
Projeto final da disciplina de Comunicação e Redes, realizada em 2024 na UFABC.

### 🎯 Objetivos

Este projeto busca mapear e compreender métricas estruturais em redes complexas através do universo fictício criado pela autora Suzanne Collins na saga Jogos Vorazes. A ideia principal é verificar se as personagens desse mundo fictício se conhecem para que então, possamos confirmar que há uma rede complexa de relações criadas dentro desse mundo distópico. Para cumprir esses objetivos, iremos utilizar as seguintes ferramentas: 

### 🛠️ Ferramentas de Software, Plataformas e Serviços Computacionais

* **Linguagem principal**: Python
* **Modelagem de redes**: NetworkX
* **Bibliotecas complementares**: Pandas, NumPy, Seaborn, MatPlotLib

### 📊 Modelagem dos dados

* **Vértices**: personagens
* **Arestas**: conexão entre os personagens

### ✔️ Resultados gerais

Foram localizados 150 personagens mencionados, sendo 52 da Capital e o restante dos 12 Distritos existentes na trama, além disso, o personagem com mais conexões é Coriolanus Snow. Analisando os três jogos descritos da saga (74ª, 75ª e 10ª edição, respectivamente na ordem de lançamento), apenas no 10º jogo temos nomes de todos as personagens dos 12 distritos que participaram. Confira o código, dados obtidos e métricas completas abaixo: 

| Tipo | Visualizar | Descrição |
| :--- | :--- | :--- |
| **Código em Python** | [Ver código](trabalho_cr.ipynb) | Jupyter Notebook com o código completo utilizado. |
| **Dados obtidos** | [Ver Dados](metricas/betweenness.md) | Tabelas com os dados obtidos a partir da EDA inicial. |
| **Métricas** | [Ver Métricas](closeness.csv) | Tabelas com as métricas obtidas a partir do grafo e análises. |

### 🔍 Observações importantes 

O projeto foi realizado no ano de 2024 e não há pretensão de ser atualizado caso a autora publique mais livros que expandam o universo e, consequentemente, o número de personagens. Os livros utilizados de base para o projeto são: Jogos Vorazes, Em Chamas, A Esperança e A Cantiga dos Pássaros e das Serpentes.
