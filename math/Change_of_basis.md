# Change of Basis (Basic)
Motivation: In Quantum mechanics and linear algebra, the operation to change the basis of a vector is a fundamental procedure that teaches students the 
process of constructing an operator(matrix), as well as strengthen their visulization of vector spaces.

Goal: As the name suggest, the goal of the operation is to change a vector from one basis representation to another (i.e. from basis A = {[1,0], [0,1]} to B = {[1,1], [1,-1]}).
Since how we describe operations in LA is via operators, our goal is to create a matrix that transforms the basis. 

$$ [v]_B = S_{A \rightarrow B} [v]_A$$


where
- $[v]_A$ is the vector in basis A
- $S_{A \rightarrow B}$ is the matrix we will build that transforms vectors from basis A to basis B
- $[v]_B$ is the vector in basis B

Note that: **Although the value of the vector changed, the information the vector carry did not change.** Changing the basis is similiar to changing our perspective,
viewing the vector from a different angle makes the vector look different eventhough the vector itself did not change. This maybe more sensible if we view
a vector as a model of some physical system, so it contain physical information (i.e. a robotic arm positioned in 2D space, or the state of a 2 level quantum system).
When we change the basis, the physical information the vector models does not change, namely the physical system does not change, what changed is our basis representation of
that physical system (like changing the coordinate system we use to describe the system).

# Procedure
Goal: generate the change-of-basis matrix $S_{A \rightarrow B}$

$[v]_A = v_1a_1+v_2a_2+...+v_na_n \text{ and } [v]_B = v_1b_1+v_2b_2+...+v_nb_n$

$$ 
[v]_B = S_{A \rightarrow B} [v]_A

$$



# Reference
https://www.statlect.com/matrix-algebra/change-of-basis
