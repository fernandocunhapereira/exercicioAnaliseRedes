1. Define:

	(a) Subgraph
	SUBGRAFOS SÃO GRAFOS FORMADOS A PARTIR DE NÓS EXISTENTES NO GRAFO ORIGINÁRIO, DE ACORDO COM AS ARESTAS (OU RELAÇÕES) QUE FORAM DEFINIDAS PARA A ANALISES QUE SE DESEJA FAZER DESSE SUBCONJUNTO
	
	(b) Bipartite graph.
	SÃO GRAFOS CUJOS NÓS PODEM SER DIVIDOS EM 2 CONJUNTOS DISJUNTOS (U & V) DE MODO QUE OS NÓS DE U SÓ SE CONTECTAM COM NÓS DE V E VICE-VERSA
	
	(c) Hamiltonian graph
	UM GRAFO HAMILTONIANO É O GRAFO ONDE É POSSIVEL CRIAR UM CAMINHO ONDE CADA NÓ É VISITADO APENAS UMA VEZ
	
	(d) Eulerian graph.
	UM GRAFO EULERIANO É O GRAFO ONDE É POSSIVEL CRIAR UM CAMINHO ONDE CADA ARESTA É UTILIZADA APENAS UMA VEZ, PODENDO OCORRER DE VISITAR UM MESMO NÓ MAIS DE UMA VEZ

2. Describe how a breadth-first search algorithm works.
	O BREADTH-FIRST SEARCH É UM ALGORITMO QUE BUSCA UM NÓ COM UMA CARACTERISTICA DESEJADA. PARTINDO DE UM NÓ RAIZ, O ALGORITMO FAZ A BUSCA PRIMEIRO EM TODOS OS NÓS IMEDIATAMENTE VIZINHOS DESTE NÓ (1 NIVEL), EM SEGUIDA BUSCA EM TODOS OS NÓS DO 2 NIVEL E ASSIM SUCESSIVAMENTE.

3. How many edges does a complete graph with n vertices have? What about a complete directed graph with n vertices?
	"GRAFO COMPLETO" NUMERO DE ARESTAS = (NUMERO NÓS*(NUMERO NÓS - 1))/2
	"GRAFO DIRECIONADO" NUMERO DE ARESTAS = NUMERO DE NÓS*(NUMERO DE NÓS -1)

4. What are isomorphic graphs? Draw an example.

5. Calculate the degree of the nodes for both node types in the bipartite adjacency matrix from the figure below. Find the isolated node(s).

![adjacency matrix](./img/matrix01.png)

6. Given the digraph `G = (V, E)` where `V = {M, N, O, P, Q, R, S}` and 

`E ={(M, S), (N, O), (P, R), (N, S), (O, M),
	 (N, Q), (O, M), (P, P), (S, M), (O, N), 
	 (S, M), (N, R), (P, M), (M, S)}`

	(a) Specify, if any, a simple path from vertex M to vertex S.
	A ARESTA (M, S) JÁ É UM CAMINHO ENTRE "M" E "S"

	(b) Specify, if any, a simple cycle, involving at least 4 nodes.
	NÃO HÁ

	(c) Is the digraph connected or not connected?

	(d) What is the degree of vertices N and R.
	N = 5
	R = 2

	(e) Represent the digraph using adjacency list representation.
	M: S
        N: O,S,Q,R
        O: M,N
        P: R,P,M
        Q:
        R:
        S: M

	(f) Represent the digraph using adjacency matrix representation.
	      M N O P Q R S
          M 0 0 0 0 0 0 1
          N 0 0 1 0 0 1 1
          O 1 1 0 0 0 0 0
          P 1 0 0 1 0 1 0
          Q 0 0 0 0 0 0 0
          R 0 0 0 0 0 0 0
          S 1 0 0 0 0 0 0

7. Draw the undirected and directed versions of the graph G(V, E), where V = {1, 2, 3, 4, 5, 6} and E = {(2, 5), (6, 1), (5, 3), (2, 3)}.

8. How many edges does a graph have 3 vertices of degree 3 and one vertex of degree 5?

9. Mr. A is friend with Mrs. B, but she doesn't like him back. She has a reciprocal friendship with both C and D, but only C considers D a friend. D has also sent friend requests to E, F, G, and H but, so far, only G replied. G also has a reciprocal relationship with A. Draw the corresponding directed graph.

10. Draw the graph from the previous exercise as undirected and weighted, with the weight being 2 if the connection is reciprocal, 1 otherwise.
