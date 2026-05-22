### Quantum MAXCUT

The quantum maxcut problem is defined in terms of the Heisenberg Hamiltonian. 

$$H = - \sum_{(i,j) \in E} \frac{I - \sigma_x^i \sigma_x^j - \sigma_y^i \sigma_y^j - \sigma_z^i \sigma_z^j}{4}$$

Where $G = (V,E)$ is given as input. The Hamiltonian can be block diagonalized (since it's hermitian) and each block corresponds to the laplacian of the token graph $F_k$.

A **token graph** $F_k$ is defined by a graph $G = (V,E)$ and an integer $0 \leq k \leq |V|$. 

We first define the structure of the graph $G$

* *Node*: Represents a node of $G$. Defined as a Int.
* *Edge*: Relation between two Nodes.
* *Graph*: Made up of a numbre $n$ (number of nodes), and a list of nodes and edges.

Moreover we define an equality measure for edges and an order for nodes.