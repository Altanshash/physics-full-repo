# Problem 8 – Orbit Perturbation and Precession

## Given

We consider a modified gravitational potential:

$$U(r)=-\frac{GMm}{r}+\frac{\alpha}{r^2}$$

Where:

- $G$ is the gravitational constant.
- $M$ is the central mass.
- $m$ is the orbiting mass.
- $r$ is the distance from the central body.
- $\alpha$ is the perturbation parameter.

The goal is to investigate how the parameter $\alpha$ changes the orbit.

---

## Solution

### 1. Modified Potential

The usual Newtonian gravitational potential is:

$$U_N(r)=-\frac{GMm}{r}$$

In this problem, an additional perturbation term is added:

$$U_p(r)=\frac{\alpha}{r^2}$$

So the total potential becomes:

$$U(r)=-\frac{GMm}{r}+\frac{\alpha}{r^2}$$

---

### 2. Equation of Motion

The radial force is obtained from the potential:

$$F(r)=-\frac{dU}{dr}$$

Differentiating:

$$\frac{dU}{dr}=\frac{GMm}{r^2}-\frac{2\alpha}{r^3}$$

Therefore:

$$F(r)=-\frac{GMm}{r^2}+\frac{2\alpha}{r^3}$$

The acceleration is:

$$a(r)=\frac{F(r)}{m}$$

Thus:

$$a(r)=-\frac{GM}{r^2}+\frac{2\alpha}{mr^3}$$

In vector form:

$$\vec{a}=\left(-\frac{GM}{r^3}+\frac{2\alpha}{mr^4}\right)\vec{r}$$

---

### 3. Precession of the Perihelion

In the pure Newtonian case, when:

$$\alpha=0$$

the orbit is a closed ellipse.

When:

$$\alpha \neq 0$$

the orbit is no longer exactly closed.

The closest point to the central mass is called the perihelion.

Because of the perturbation, the perihelion shifts after each orbit. This shift is called precession.

---

### 4. Effect of the Parameter Alpha

The parameter $\alpha$ controls the strength of the perturbation.

If $\alpha=0$, the orbit is a stable closed ellipse.

If $\alpha>0$, the additional term changes the effective force and causes the ellipse axis to drift.

As $\alpha$ increases, the precession angle becomes larger.

---

## HTML Requirements

The HTML visualization should include:

- animation of the ellipse axis drift
- measurement of the precession angle
- slider for the parameter $\alpha$

---

## Conclusion

A modified gravitational potential can change the shape and orientation of an orbit.

The potential is:

$$U(r)=-\frac{GMm}{r}+\frac{\alpha}{r^2}$$

The resulting radial force is:

$$F(r)=-\frac{GMm}{r^2}+\frac{2\alpha}{r^3}$$

When $\alpha=0$, the orbit is a closed Newtonian ellipse.

When $\alpha$ is not zero, the orbit begins to precess. This means that the perihelion slowly shifts from one orbit to the next.

Thus, the perturbation parameter $\alpha$ controls the amount of orbital precession.
