# Teste_Tecnico__Estagio_Data_Science
### Teste Técnico Estágio de Data Science
O primeiro passo foi compreender mais sobre análise de redes socias. Utilizei o site da [Columbia University](https://www.publichealth.columbia.edu/research/population-health-methods/social-network-analysis#:~:text=Social%20Network%20analysis%20is%20the,,%20groups%20and/or%20organizations.) e [Science Direct](https://www.sciencedirect.com/topics/social-sciences/social-network-analysis). O passo seguinte foi compreender a Centralidade de proximidade, que é definida como $C(x)=\frac{1}{\sum_{y}d(x,y)}$, podendo ser normalizada para $C(x)=\frac{n-1}{\sum_{y}d(x,y)}$, onde n= número de vértices.
O passo inicial é importar algumas bibliotecas para facilitar a manipulação de dados, usando "Pandas" para importar o arquivo fornecido gerando uma tabela e encontrar o número de vértices e ligações. Gerei uma classe que através dessa lista gera um dicionario com cada vértice e as ligações que ele possui. Isso é possivel com o uso de um loop, que resulta em um objeto "G". Essa técnica é baseada na biblioteca "Networkx", que também faz uso de um dicionario para isso.
### Centralidade de proximidade
A distancia entre dois vértices pode ser calculada de algumas maneiras com o uso de algoritmos: 

 - Algoritimo de Dijkstra
 - Busca A* 
 - Algoritimo Breadth-First Search (BFS)

Devido ao tamanho dos dados elegi o "Busca A*" como preferencial, ele é considerado um algoritmo de busca direcionado, ou seja, só tenta um caminho se ele az sentido. Para gerar a função heuristica necessária para a execução, 10 vértices foram escolhidos e a distancia entre eles calculada manualmente.
### Gráfico de Rede Social
Para gerar o gráfico foi utilizado o "plotly", defini uma matriz 10x10 com os vértices em cada ponto dela, organizados com o de maior centralidade em 1x1 e o de menor em 10x10. Inicialmente as ligações foram plotadas, seguido pelos vértices com seus nomes.
### Dependências

 - [Pandas](https://pandas.pydata.org/)
 - [Numpy](https://numpy.org/)
 - [Collections](https://docs.python.org/3/library/collections.html)
 - [Plotly](https://plotly.com/)
 - [Project Jupyter | Home](https://jupyter.org/)

### Executar
O código foi escrito em Python pelo Jupyter Lab, assim para executar o arquivo [Teste_Tecnico_Semantix.ipynb](Teste_Tecnico_Semantix.ipynb) ele deve ser aberto no Jupyter, com o arquivo edges na mesma pasta. E assim "Executar todas as Células".

### Referências 

 - [Graphs in Python: Dijkstra's Algorithm (stackabuse.com)](https://stackabuse.com/dijkstras-algorithm-in-python/)
 - [Implementing Dijkstra’s Algorithm in Python | Udacity](https://www.udacity.com/blog/2021/10/implementing-dijkstras-algorithm-in-python.html)
 - [A* Algorithm in Artificial Intelligence You Must Know in 2022 (simplilearn.com)](https://www.simplilearn.com/tutorials/artificial-intelligence-tutorial/a-star-algorithm)
 - [Implementation of A Star Search Algorithm in python - VTUPulse](https://www.vtupulse.com/artificial-intelligence/implementation-of-a-star-search-algorithm-in-python/)
 - [A-star-rabiscos.pdf (usp.br)](https://www.ime.usp.br/~coelho/mac0323-2018/aulas/aula09/A-star-rabiscos.pdf)
 - [Shortest path problem - Wikipedia](https://en.wikipedia.org/wiki/Shortest_path_problem)
 - [Centrality - Wikipedia](https://en.wikipedia.org/wiki/Centrality#Closeness_centrality)
 - [Visualizing Networks in Python. A practical guide to tools which helps… | by Mohit Mayank | Towards Data Science](https://towardsdatascience.com/visualizing-networks-in-python-d70f4cbeb259)
