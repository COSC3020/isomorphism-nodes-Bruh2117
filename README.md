[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=13148724&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

# Theorem: 

Suppose graphs $A = (V_1, E_1)$ and $B = (V_2, E_2)$ don't have the same number of nodes and are isomorphic.
Since they don't have the same number of nodes, $A$ will have less nodes than $B$ or vice versa. 

Since they're isomorphic there exists a bijective funtion $f: V_1 -> V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

It follows that $f$ is then a onto and one-to-one function. This means that for it to be one-to-one, for each $s \in V_2$ 
there is at most one $t \in V_1$ such that $f(t) = s$, and to be onto, for each $s \in V_2$ there is at least one 
$t \in V_1$ such that $f(t) = s$. 

However, since one graph will have less nodes than the other, there will be some node in a graph that is either mapped to 
more than one node or not mapped to any node in the other graph. 

This means that $f$ cannot be both a one-to-one and onto function. But we stated that it is. This is a contradiction, 
thus proving the theorem. 
