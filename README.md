# gravitationalwavesSchwarzschild
1 A brief description of the MATHEMAT-
ICA codes
The programs listed are written in such a manner that the relation to the
formulas in the manuscript (Axial and polar modes for the ring down of
a Schwarzschild black hole with an r dependent mass-function) should be
obvious.
Some denitions:
 r: radial distance
 y = r
m0
: Dimensionless radial distance
 m0: mass parameter
 ! (or ): Frequency, mode
 e!
= m0!: Dimensionless frequency (mode)
2 Eq.(23),(24) and Appendix B, Zerilli-ansatz
for Z.nb
This derives the equations (23) and (24) in the manuscript, i.e., it parts from
the ansatz for the Z-function, polar modes, and gives the solutions for the
functions (r) and (r).
This program applies the derivative d2
dy2

to an ansatz of Z(+), given by
(y = r
m0
)
Z(+) = (y)N(y) + (y)V (y) + 
(y)(L(y) + X(y)) (1)
in terms of the functions N(y), V (y) and X(y), see book of Chandrasekhar
and manuscript. It turns out that (y) = 0 and (y) = y, see mansucript
and further below, such that the Z-function is only a combination of V (r)
and LX = (L(y) + X(y)).
As a result one obtains that
 
d2
dy2 + ~!2
!
Z(+) = V +
V (y)V (y) + V +
LX(L(y) + X(y)) : (2)
1
The tilde refers to ~! = m0!.
More details:
We dene
LX(r) = L(r) + X(r) : (3)
The second derivative of r is applied to Z(+) and the factors of N(r),
V (r) and LX(r) are determined. In a further step, the routine sets all
contributions to zero, except of ~!2 (called in the program 2), i.e., the routine
selects the term of !2. The required result is
􀀀2 ((r)N(r) + (r)V (r) + 
(r)LX(r)) : (4)
As it turns out, the factor of N(r) does not depend on  and, thus, by
selecting the contribution of 2, Eq. (4) is satised when
(r) = 0 : (5)
Concentrating on the V (r) part, leads to the equations and the result for
(r):
n(r) 􀀀 (r) = 􀀀(r) ! (r) = 0 : (6)
Concentrating on the factor of LX(r) and using (r) = 0, leads for (r)
to
􀀀2(r) + n
(r) + 2r0(r) = n
(r) ! 0(r) =
1
r
(r) : (7)
the solution of this dierential equation is
(r) = r : (8)
Finally, the factor of N(r), still depending on  = 0,  = r and the
unknown funtion 
(r), is set to zero, which leads to the 
(r) as given in Eq.
(24) of the manuscript.
2
3 Dif-Equation for gam(r).nb
This routine sets up the dierential equation for the 
(r) function, equating
the functions rV (r) and 
(r)(L(r) + X(r)).
4 gam(r)-limit GR.nb
Sets the mass-function to a constant and uses the ansatz form Chandrasekhars
book of 
(r) into the dierential equation (27). The result is zero, showing
that the limit of GR is satised.
5 Figure.6-left hand side.nb and Figure.6-right
hand side.nb
Figure.6-left hand side.nb: Plot of the two potentials V (+)
V and V (+)
LX
Figure.6-right hand side.nb: plots the dierence

V (+)
V 􀀀 V (+)
LX

.
All the following programs use implicitly the approximation of

(r)!
6 Set up of the Zerilli (polar modes) and Regge-
Wheeler (axial modes) equation
The list of programs are:
 Zerilli-equation-pcGR-axial modes+gures.nb: Constructs the
Regge-Wheeler equation for the axial modes in pc-GR. It also determines
the functions 0 and s0 as used in the AIM. At the end, this
routine contains some gures of the main text and of the Appendix.
 Zerilli-QNM-pcGR-axial modes+gures.nb: Determines the axial
modes via the AIM formalism (see the manuscript). At the end, this
routine contains some gures of the main text and of the Appendix.
3
 Zerilli-equation-pcGR-polar modes+gures.nb: Constructs the
Regge-Wheeler equation for the axial modes in pc-GR. It also determines
the functions 0 and s0 as used in the AIM. At the end, this
routine contains some gures of the main text and of the Appendix.
 Zerilli-QNM-pcGR-polar modes+gures.nb: Determines the polar
modes via the AIM formalism (see the manuscript). At the end, this
routine contains some gures of the main text and of the Appendix.
 Zerilli-QNM-GR, axial=polar modes+gures.nb: Determines
the axial and polar modes via the AIM formalism (see the manuscript),
within the GR. The coecient functions 0 and s0 are taken from Cho-
2012 (see reference list in the manuscript). At the end, this routine
contains some gures of the main text and of the Appendix.
7 Eq. (29) and Figure1, V(r) and VLX(r).nb
This program constructs the potentials V (+)
V (r) and V (+)
LX (r), using the ansatz
for the Zerilli function with coecients determined in "... Zerilli-ansatz for
Z.nb" (see Section 2). It compares both functions.
8 Figure1 GR-potential.nb
Constructs the GR-potential. i.e., for a constant mass.
9 Eq.(50),Tortoise coordinate.nb
It determines the analytic solution of the integral (48) in the manuscript for
GR and the special ansatz for the mass-function in pc-GR.
The particular mass-function, used in pc-GR is:
m(r) = 1 􀀀
27
32y3 ; (9)
This case permits an analytic solution!
4
10 Eq.(33),(34),EventHorizon-n=4-a=0.nb
Solves the equation (33) in the event horizon, as a function in the parameter
value b. The physical solution is nally given in Eq. (34) of the manuscript.
11 plots-300-400-500-polar.nb
This is an example on how to use the calculated list of gravitational modes
and create plots, without recurring to repeat the calculations. The example
shown is for the polar modes of up to 500 iterations.
The method is to copy the list of modes, naming them in this example as
R300, R400 and R500. then make the plots. At the end, all plots are joined.
5
