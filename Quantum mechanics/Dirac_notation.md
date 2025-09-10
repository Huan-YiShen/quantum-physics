# topics
topic from J.J. Sakuri's text

# 1.2 Kets, Bras, and operators
- Ket space
  - Hilbert Space (everything is complex!)
  - discrete dimension and continuous spectra
  - state vector (ket as a representation of physical state)
  - linear combination (addition + scalar multiplication)
  - null ket
  - global phase (only "direction" in vector space is of significant)
  - observable = operator
  - eigenstate (eigenkets) and eignevalues
  - linear combination of basis

$$\ket a = \sum_b c_b \ket b$$


- Bra space and inner product
  - dual correspondence of ket space (also a space)
  - convert bra to ket (don't forget to take the complex conjugate)
  - inner product
    - $\braket{b|a} = \braket{a|b}^*$
    - $\braket{a|a} \ge 0$ (positive definite metric)
  - orthogonal 
    - two kets are orthogonal iff $\braket{a|b} = 0$
  - normalization of ket
    - ket is normalized iff $\braket{a|a} = 1$
    - $\sqrt{\braket{a|a}}$ = norm of $\ket a$

- Operators
  - equvalence in operators
  - null operator
  - "Addition of operators" is commutative and associative (1 exception)
  - dual of operator --> Hermitian adjoint --> **Hermitian**
- Multiplication
  - non-commutative && associative
  - $(XY)^\dagger = X^\dagger Y^\dagger$
  - **outer product** <-- $\ket a \bra b$
    - if $X\ket a$, then its dual is $\bra a X^\dagger$
- The associative Axiom of multiplication
  - $A\ket z = (\ket x \bra y) \ket z = \ket x \braket{y|z} = c\ket x$
  - if $X = \ket a \bra b$, then $X^\dagger = \ket b \bra a$
  - $\bra b X \ket a = \bra a X^\dagger \ket b ^*$

# 1.3 Base Kets and Matrix Prepresentations
- 1.3.1 Eigenkets of an observable
- 1.3.2 Eigenkets as Base Kets
- 1.3.3 Matrix representations
- 1.3.4 Spin 1/2 System
# 1.4 Measurements, Observables, and the Unvertainty Relation
- 1.4.1 Measurements
- 1.4.2 Spin 1/2 System
- 1.4.3 Compatible Observables
- 1.4.4 Incompatible Observables
- 1.4.5 The uncertainty relation
# 1.5 Change of basis
- 1.5.1 Transformation operator
- 1.5.2 Transformation matrix
- 1.5.3 Diagonalization
- 1.5.4 Unitary Equivalent Observables