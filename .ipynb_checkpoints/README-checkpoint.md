# Teste_Tecnico__Estagio_Data_Science
[Português](README_pt.md)
### Technical Test Data Science Internship 
The first step to solve the test was learning more about social network analysis. I visited the website of [Columbia University](https://www.publichealth.columbia.edu/research/population-health-methods/social-network-analysis#:~:text=Social%20Network%20analysis%20is%20the,,%20groups%20and/or%20organizations.) and [Science Direct](https://www.sciencedirect.com/topics/social-sciences/social-network-analysis). After this step I seached a little more about Closeness Centrality, that is defined as $C(x)=\frac{1}{\sum_{y}d(x,y)}$, and a normalized version can be interpreted as $C(x)=\frac{n-1}{\sum_{y}d(x,y)}$, where n= number of nodes.
The first step is importing libraries to facilitate the data manipulation, using "Pandas" to import the given file and generate a Dataframe as well getting the number of nodes and edges. I created a class named "Graph" to generate a dictionary with the node and the edges from it. Using a loop all of the info on the file is entered on the object "G". This was based on the "Networkx" library, that use a dictionary for the nodes as well.
### Closeness Centrality
Some algorithms can be used to calculate the distance between two nodes as: 

 - Dijkstra's Algorithm
 - A* Search
 - Breadth-First Search (BFS) Algorithm

Considering the size of the data the chosen one was the "A* Search", it is a guided algorithm so steps are only take if they seems promising and reasonable. 10 node were choose and the distance between then calculate, the results were feeded to the heurist function, necessary for this technique.
### Core Graph
The core graph was generated using "plotly", a matrix(10x10) was defined with the nodes at each item, organized with the node with the biggest Closeness Centrality in the position 1x1 e the smallest at 10x10. First all the edges were plotted, and then the nodes with the names.
### Dependencies

 - [Pandas](https://pandas.pydata.org/)
 - [Numpy](https://numpy.org/)
 - [Collections](https://docs.python.org/3/library/collections.html)
 - [Plotly](https://plotly.com/)
 - [Project Jupyter | Home](https://jupyter.org/)

### Build and Run
The code was created with Python on Jupyter Lab, to execute it the file [Teste_Tecnico_Semantix.ipynb](Teste_Tecnico_Semantix.ipynb) should be open on Jupyter, the file edges need to be on the same foldes. After this just "Run all cells".

### References

 - [Graphs in Python: Dijkstra's Algorithm (stackabuse.com)](https://stackabuse.com/dijkstras-algorithm-in-python/)
 - [Implementing Dijkstra’s Algorithm in Python | Udacity](https://www.udacity.com/blog/2021/10/implementing-dijkstras-algorithm-in-python.html)
 - [A* Algorithm in Artificial Intelligence You Must Know in 2022 (simplilearn.com)](https://www.simplilearn.com/tutorials/artificial-intelligence-tutorial/a-star-algorithm)
 - [Implementation of A Star Search Algorithm in python - VTUPulse](https://www.vtupulse.com/artificial-intelligence/implementation-of-a-star-search-algorithm-in-python/)
 - [A-star-rabiscos.pdf (usp.br)](https://www.ime.usp.br/~coelho/mac0323-2018/aulas/aula09/A-star-rabiscos.pdf)
 - [Shortest path problem - Wikipedia](https://en.wikipedia.org/wiki/Shortest_path_problem)
 - [Centrality - Wikipedia](https://en.wikipedia.org/wiki/Centrality#Closeness_centrality)
 - [Visualizing Networks in Python. A practical guide to tools which helps… | by Mohit Mayank | Towards Data Science](https://towardsdatascience.com/visualizing-networks-in-python-d70f4cbeb259)
