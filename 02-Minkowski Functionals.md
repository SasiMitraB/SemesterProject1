# Minkowski Functionals

## Introduction

Minkowski Functionals are a set of mathematical tools used to analyze the shape and structure of data in a variety of fields, including cosmology and astrophysics. Originating from integral geometry, these functionals measure geometric properties of sets and can describe the morphology of complex structures. In cosmology, Minkowski Functionals are particularly valuable for studying the large-scale structure of the universe, such as the distribution of galaxies and the cosmic web. They help quantify properties like the number, size, and connectivity of cosmic structures, providing insights into the underlying physical processes and the validity of cosmological models.

In the study of the interstellar medium (ISM), Minkowski Functionals are employed to identify and characterize filamentary structures. These filaments, which are crucial for understanding the formation of stars and galaxies, can be challenging to detect due to their intricate and often diffuse nature. By applying Minkowski Functionals to observational data, researchers can effectively quantify the shape and distribution of these filaments, helping to elucidate their role in the ISM and improve our understanding of cosmic structure formation.

My primary references that I used when learning were the following:
1. Minkowski Functionals in Cosmology, Schmalzing et al. [@schmalzing1995minkowskifunctionalscosmology],
2. Wikipedia page for Minkowski Functionals, [@wiki:Minkowski_functional]
## A few basic defintions

**Functional:** A Function mapping from a Space $X$ to either Real or Complex Numbers. An example would be Linear Forms, ie, a mapping of a Vector Space to it's scalar field. 

## Bertrand's Paradox:
The Bertrand paradox is a problem within the classical interpretation of probability theory. Joseph Bertrand introduced it in his work Calcul des probabilités (1889) as an example to show that the principle of indifference may not produce definite, well-defined results for probabilities if it is applied uncritically when the domain of possibilities is infinite.

Reference for this section: Wikipedia: Bertrand Paradox (Probability) [@wiki:Bertrand_paradox_(probability)]

### Problem Statement

The Bertrand paradox is generally presented as follows: Consider an equilateral triangle inscribed in a circle. Suppose a chord of the circle is chosen at random. What is the probability that the chord is longer than a side of the triangle? 

Classically, There are many ways to construct the sample space for this probability question:

### Method 1: 

Choose any point on the circle. A chord going through this point can have an angle between $0$ and $\pi$ radians with the tangent. 

Without Loss of generality, let one of the vertices of the inscribed equilateral triangle be at this point. The sides of the equilateral triangle coming from this point are forming angles of $\pi / 3$ and $2\pi / 3$ respectively.

For the chord to be longer than the 