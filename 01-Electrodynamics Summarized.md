# Governing Equations of Electrodynamics

Fluid Dynamics are written with Volumetric Equations, and thus to incorporate Electrodynamics in them, we have to write Electrodynamics Equations also in a Volumetric formulation. This page should serve as a review of the nessecary Electrodynamics, while also deriving theese volumetric formulations nessecary for Magnetohydrodynamics.

## Lorentz Force

A charged particle with a velocity $v$ and charge $q$ experiences the force given by 
$$f = q \vec{E_s} + q \vec{E_i} + q (\vec{b} \times \vec{b})$$ 
* $\vec{E_s}$ = Static Electric Field
* $\vec{E_i}$ = Force from Varying Magnetic Field
* $q(v\times B)$ = Lorentz Force

The static electric field is Irrotational and has a fixed divergence. 
$$\nabla \times \vec{E_s} = 0 \:\:\:\: \nabla \cdot \vec{E_s} =  \frac{\rho_e}{\epsilon _ 0}$$
* $\rho_e$ = Total Charge Density
* $\epsilon_0$ = Permitivity of Free Space

The Electrostatic Potential $V$ is given by 

$$\vec{E_s} = - \nabla V \:\:\: \nabla ^2 V = \frac{\rho_e}{\epsilon _ 0}$$

The total electric field given by $\vec{E_s} + \vec{E_i} = \vec{E}$ is subject to the following constraints. 

$$\nabla \cdot \vec{E} =  \frac{\rho_e}{\epsilon _ 0} \:\:\: \text{Gauss Law}\\ \nabla \times \vec E = \frac {\partial \vec B}{\partial t} \:\:\: \:\:\text{Faraday's Law}$$

THe magnetic field $\vec B$ is a pseudovector, which will have consequences for Dynamo Theory.

### Volumetric Lorentz Force

Let $\vec J$ represent current density.

$$\vec J = \sigma \vec E$$
In a moving frame, the same equation can be written as 
$$ \vec J= \sigma (\vec E + \vec v \times \vec B)$$
We can identify this as the Volumetric Gauss Law

The Electrostatic Lorentz force is given by 

$\vec F = q (\vec E + \vec v \times B)$

Dividing this by the volume, we get 

$$\vec f = \rho_l \vec E + \vec J \times B$$
This is the volumetric Lorentz Force Equation.

> **Claim**: In non Relativistic Frames, the leading $\rho_l \vec E$ term is negligible. 
> 
> **Proof**: 
> We can write the continuity equation of charge to be of the form
> $$\nabla \cdot \vec J = - \frac{\partial \rho _l}{\partial t}$$
> This simply says that the rate at which charge is decreasing inside a small volume must equal the rate at which charge flows out across the surface of that volume. 
> Taking divergence on both sides of the volumetric gauss law, and substituting it in the continuity of charge equation, we get
> $$\frac{\partial \rho _l}{\partial t} + \frac{\rho _l}{\tau _ l} + \sigma \nabla \cdot (\vec v \times \vec B) = 0$$
> where $\tau_l$ represents the relaxation time of the system and is a very small quantity.
> So when we observe at timescales much larger than $\tau _l$,
> $$\frac{\partial \rho_l}{\partial t} << \frac{\rho _l}{\tau _ l} $$
> and we can neglect the term $\frac{\partial \rho_l}{\partial t}$.Rearranging the terms we get that
> $\rho_l = - \epsilon _ 0 \tau _l \nabla \cdot ((\vec v \times \vec B)$ is very small and can be neglected as well (because $\tau _l$ is small)
> Going back to the volumetric Lorentz Force equation, we find under these assumptions of Non-Relativistic frames, the equation reduces to 
> $$\vec f = \vec J \times \vec B$$

## Ampere Maxwell's Laws

The Ampere Maxwell Law is given by 
$$\nabla \times \vec B = \mu \left[ \vec J + \epsilon _ 0 \frac{\partial \vec E}{\partial t} \right]$$
In conductors, this second term $\epsilon _ 0 \frac{\partial \vec E}{\partial t}$ contributes negligibly, and Maxwell's Correction is not nessecary, leaving us with $\nabla \times B = \mu \vec J$

Inverting the last equation there gives us the biot savart law.

$$B(x) = \frac {\mu}{4 \pi} \int \frac{J(x') \times \vec r}{r^3} d^3 x' $$

### Reduced Maxwell's Laws 

The general form of Maxwell's Laws are given by 