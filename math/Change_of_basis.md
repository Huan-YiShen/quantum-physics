# Change of Basis (Basic)
Motivation: In Quantum mechanics and linear algebra, the operation to change the basis of a vector is a fundamental procedure that is useful to simplify calculations, visulize problems, and can help teach students the process of constructing an useful operator from scratch. For more professional resources go directly to [reference section](#Reference--Examples).

Goal: As the name suggest, the goal of the operation is to change a vector from one basis representation to another (i.e. from basis A = {[1,0], [0,1]} to B = {[1,1], [1,-1]}).

Since how we describe operations in LA is via linear operators (matrices), our goal is to create a matrix that transforms the basis. Namely,
<p align="center">
  $[v]_{B} = S_{A \rightarrow B}[v]_{A}$
<p/>

where
- $[v]_A$ is the vector in basis A
- $S_{A \rightarrow B}$ is the matrix we will build that transforms vectors from basis A to basis B
- $[v]_B$ is the vector in basis B

Note that: 
- **Although the value of the vector changed, the information the vector carries did not change.** Changing the basis is similiar to changing our perspective,
viewing the vector from a different angle makes the vector look different eventhough the vector itself did not change. This maybe more sensible if we view
a **vector as a model of some physical system**, so it contain physical information (i.e. a robotic arm positioned in 2D space, or the state of a 2 level quantum system).
When we change the basis, the physical system that the vector models does not change, what changed is our basis representation of
that physical system (like changing the coordinate system we use to describe a real system).
- Vectors by default are represented in cartestian basis - [1,0,0], [0,1,0], [0,0,1] or $\hat i, \hat j, \hat k$. Even when we use a different basis such as B = {[1,1], [1, -1]}, it is still written in the cartestian basis. This can be a source of confusion, but just know that our default communication is always on the cartestian basis.

## Goal 1: generate the change-of-basis matrix $S_{A \rightarrow B}$

notice: $[v]_A = v_1a_1+v_2a_2+...+v_na_n$ and $[v]_B = v_1b_1+v_2b_2+...+v_nb_n$
* so if we were able to represent each component of A in basis B ($[a_1]_B$), we are able to change $[v]_A$ to $[v]_B$
* namely: $[v]_B = v_1b_1+v_2b_2+...+v_nb_n = v_1[a_1]_B+v_2[a_n]_B+...+v_n[a_n]_B = [[v]_A]_B$
* Notice: the magnitude of the vector never changes {v1, v2, ..., vn), but it is multiplied by a different basis
* If we bring all of these transformation into a matrix it looks as the follow

<p align="center">
  $S_{A \rightarrow B}[v]_{A} = [ [a_1]_B  [a_2]_B ... [a_n]_B]$
<p/>

where
- $[a_n]_B$ is a column vector - component of basis-A represented in basis-B
- $[ [a_1]_B [a_2]_B ... [a_n]_B]$ each column of this matrix changes one component of basis-A into basis-B. When the full matrix is applied to vector in basis-A,
all its component gets represented in basis-B. Thus the change of basis operation is performed.

## Goal 2: so how to compute this column vector $[a_n]_B$
- above reasoning proved that we just need to know the column vectors $[a_1]_B$, $[a_2]_B$, ..., $[a_n]_B$ to construct the transformation matrix S
- you are usually given the starting and resulting basis (namley all its components), also recall $[a_n]_B$ means how to represent $a_n$ using the available components,
so **all you need to do is to write $a_n$ as a linear combination of the basis components of B**.

$$\begin{matrix}
a_1 = c_1b_1 + c_2b_2 + ... + c_nb_n \rightarrow [a_1]_B = [c_1, c_2, ..., c_n] \\
a_2 = d_1b_1 + d_2b_2 + ... + d_nb_n \rightarrow [a_2]_B = [d_1, d_2, ..., d_n] \\
a_n = z_1b_1 + z_2b_2 + ... + z_nb_n \rightarrow [a_n]_B = [z_1, z_2, ..., z_n] \\
\end{matrix}
$$

## Problem Solving Procedure
when question gives you the starting and resulting basis
1. Compute how to starting basis components can be represented by the resulting basis (reasoning see Goal 2)
2. Step 1 generates a list of column vectors, put the column vectors in a matrix (reasoning see Goal 1)
3. This matrix is the change of basis operator, apply it to any vector in starting basis to change it to the resultant basis. Use it to solve the rest of the problem

When I first learned this process, it was difficult for me to understand why ths above steps worked. So I structured this document in such a way to explain the reasoning (proofs) behind each step, starting from the abstract question of how to change bases, ending at the actual computation we need to perform. After understanding this proofs, the actual execution is to work backward, and constructing the matrices is as simple as solve a few lines of linear equations. 

# Change of Basis (Operators)
Linear operators can be represented as matrices. This representation is only defined for a given basis. So, if we change the basis, the matrix representation of the same linear operators need to be changed as well.

We can use the change-of-basis matrix to witch the matrix representation of a linear operator from one basis to another. 

WIP

# Reference & Examples
https://www.statlect.com/matrix-algebra/change-of-basis

Remark: In linear algebra, we are constantly working with abstract mathematic symbols and systems of linear equations that all look the same. It is easy to get lost in the sause and mix up simple definitions (especally since LA is usually student's first introduction to formal proofs and abstract algebra concepts).  So it is particularly important to pay attention to the reason why we are performing certain calculations. It is important to remember the chain of reasoning, and not the form of computation.

