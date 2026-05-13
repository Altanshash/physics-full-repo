# Problem 4 – Schrödinger Equation  
## 1D Infinite Potential Well

## Given

Width of the well:

$$
L
$$

Potential energy:

$$
V(x) = 0, \quad 0 < x < L
$$

$$
V(x) = \infty, \quad x \le 0 \text{ or } x \ge L
$$

Boundary conditions:

$$
\psi(0) = 0
$$

$$
\psi(L) = 0
$$

---

## Solution

### 1. Schrödinger equation

Inside the well:

$$
V(x) = 0
$$

The time-independent Schrödinger equation is:

$$
-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} = E\psi
$$

Boundary conditions:

$$
\psi(0) = 0
$$

$$
\psi(L) = 0
$$

---

### 2. Energy levels

The allowed wave functions are:

$$
\psi_n(x) = A\sin\left(\frac{n\pi x}{L}\right)
$$

where:

$$
n = 1,2,3,...
$$

The energy levels are:

$$
E_n = \frac{n^2\pi^2\hbar^2}{2mL^2}
$$

Using:

$$
\hbar = \frac{h}{2\pi}
$$

we can also write:

$$
E_n = \frac{n^2h^2}{8mL^2}
$$

---

### 3. Ratio \(E_2/E_1\)

For \(n = 1\):

$$
E_1 = \frac{h^2}{8mL^2}
$$

For \(n = 2\):

$$
E_2 = \frac{4h^2}{8mL^2}
$$

Therefore:

$$
\frac{E_2}{E_1} = 4
$$

---

### 4. Energy change when \(L\) is doubled

Energy depends on the well width as:

$$
E_n \propto \frac{1}{L^2}
$$

If the width is doubled:

$$
L_2 = 2L
$$

Then:

$$
E'_n = \frac{n^2h^2}{8m(2L)^2}
$$

$$
E'_n = \frac{n^2h^2}{32mL^2}
$$

So:

$$
E'_n = \frac{E_n}{4}
$$

When \(L\) is doubled, the energy becomes **4 times smaller**.

---

### 5. Probability maximum for \(n = 1\)

For \(n = 1\), the wave function is:

$$
\psi_1(x) = A\sin\left(\frac{\pi x}{L}\right)
$$

Probability density:

$$
|\psi_1(x)|^2 = A^2\sin^2\left(\frac{\pi x}{L}\right)
$$

The maximum occurs when:

$$
\sin^2\left(\frac{\pi x}{L}\right) = 1
$$

This happens at:

$$
\frac{\pi x}{L} = \frac{\pi}{2}
$$

So:

$$
x = \frac{L}{2}
$$

---

## Conclusion

The Schrödinger equation for a particle in a 1D infinite potential well is:

$$
-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} = E\psi
$$

The allowed energy levels are:

$$
E_n = \frac{n^2h^2}{8mL^2}
$$

The energy ratio is:

$$
\frac{E_2}{E_1} = 4
$$

If the well width is doubled:

$$
E'_n = \frac{E_n}{4}
$$

For the ground state \(n = 1\), the probability is maximum at:

$$
x = \frac{L}{2}
$$
