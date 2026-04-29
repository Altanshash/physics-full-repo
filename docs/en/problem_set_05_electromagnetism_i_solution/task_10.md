# Problem 10 – Field Flux Verification of Gauss's Law

## Given

We need to verify Gauss's law for a point charge inside a sphere.

Find:

1. Define the electric field flux.
2. Consider a sphere around a point charge.
3. Implement a discrete approximation of the flux.
4. Investigate dependence on the number of grid points.
5. Compare with the analytical result.

---

## Solution

## 1. Electric field flux

Electric flux through a surface is:

```math
\Phi_E
=
\oint \vec{E}\cdot d\vec{S}
```

For a closed surface, Gauss's law is:

```math
\Phi_E
=
\frac{q}{\varepsilon_0}
```

---

## 2. Sphere around a point charge

For a point charge at the center of a sphere:

```math
E
=
k\frac{q}{R^2}
```

The surface area of the sphere is:

```math
S
=
4\pi R^2
```

Flux:

```math
\Phi_E
=
E S
```

```math
\Phi_E
=
\left(k\frac{q}{R^2}\right)(4\pi R^2)
```

Since:

```math
k=\frac{1}{4\pi\varepsilon_0}
```

Then:

```math
\Phi_E
=
\frac{q}{\varepsilon_0}
```

---

## 3. Discrete approximation

The sphere surface is divided into small surface elements.

For each element:

```math
\Delta \Phi_i
=
\vec{E}_i\cdot \vec{n}_i \Delta S_i
```

Total numerical flux:

```math
\Phi_{\text{num}}
=
\sum_i \vec{E}_i\cdot \vec{n}_i \Delta S_i
```

Using spherical coordinates:

```math
\Delta S
=
R^2\sin\theta \Delta\theta \Delta\phi
```

---

## 4. Dependence on grid points

If the number of grid points increases, the numerical approximation becomes more accurate.

```math
N \uparrow
\Rightarrow
\Phi_{\text{num}}
\rightarrow
\frac{q}{\varepsilon_0}
```

The error is:

```math
\text{error}
=
\left|
\frac{\Phi_{\text{num}}-\Phi_{\text{exact}}}
{\Phi_{\text{exact}}}
\right|
\times 100\%
```

---

## 5. Analytical result

The exact result from Gauss's law is:

```math
\Phi_{\text{exact}}
=
\frac{q}{\varepsilon_0}
```

So the numerical result must approach this value.

---

## Example Numerical Values

Let:

```math
q=1\times10^{-6}\ \text{C}
```

```math
\varepsilon_0=8.85\times10^{-12}\ \text{F/m}
```

Then:

```math
\Phi_{\text{exact}}
=
\frac{1\times10^{-6}}{8.85\times10^{-12}}
```

```math
\Phi_{\text{exact}}
\approx
1.13\times10^5\ \text{N m}^2/\text{C}
```

---

## Python Code

```python
import numpy as np

epsilon0 = 8.85e-12
k = 1 / (4 * np.pi * epsilon0)

q = 1e-6
R = 1.0

def numerical_flux(N_theta, N_phi):
    theta = np.linspace(0, np.pi, N_theta)
    phi = np.linspace(0, 2*np.pi, N_phi)

    dtheta = theta[1] - theta[0]
    dphi = phi[1] - phi[0]

    flux = 0

    for th in theta:
        for ph in phi:
            E = k * q / R**2
            dS = R**2 * np.sin(th) * dtheta * dphi

            flux += E * dS

    return flux

exact_flux = q / epsilon0

for N in [10, 20, 40, 80, 160]:
    flux = numerical_flux(N, 2*N)
    error = abs((flux - exact_flux) / exact_flux) * 100

    print("N =", N)
    print("Numerical flux =", flux)
    print("Exact flux =", exact_flux)
    print("Error =", error, "%")
    print()
```

---

## Final Answer

```math
\Phi_E
=
\oint \vec{E}\cdot d\vec{S}
```

```math
\Phi_E
=
\frac{q}{\varepsilon_0}
```

For a point charge inside a sphere:

```math
\Phi_{\text{exact}}
=
1.13\times10^5\ \text{N m}^2/\text{C}
```

The numerical approximation approaches the analytical result as the number of grid points increases.

---

## Conclusion

The electric flux through a closed spherical surface around a point charge does not depend on the radius of the sphere.  
It depends only on the charge inside the surface.  
As the number of grid points increases, the numerical flux becomes closer to Gauss's law result.
