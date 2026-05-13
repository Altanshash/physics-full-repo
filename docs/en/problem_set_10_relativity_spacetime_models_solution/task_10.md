# Problem 10 — Numerical Simulation of Relativistic Motion

## Given

Relativistic equation of motion:

<div align="center" style="font-size:26px;"><b>d(γmv) / dt = F</b></div>

where:

<div align="center" style="font-size:24px;"><b>γ = 1 / √(1 − v²/c²)</b></div>

A constant force acts on a particle.

We need to:

1. Implement the RK4 method  
2. Compare classical and relativistic motion  
3. Investigate the asymptotic approach to \(c\)  
4. Create graphs of \(v(t)\) and \(x(t)\)  
5. Evaluate energy differences  

---

# Solution

## 1. Classical Model

In classical mechanics:

<div align="center" style="font-size:26px;"><b>F = ma</b></div>

Therefore:

<div align="center" style="font-size:26px;"><b>a = F / m</b></div>

Velocity:

<div align="center" style="font-size:26px;"><b>v(t) = at</b></div>

Position:

<div align="center" style="font-size:26px;"><b>x(t) = 1/2 at²</b></div>

In the classical model, velocity increases without limit.

So, mathematically:

<div align="center" style="font-size:26px;"><b>v → ∞</b></div>

This is not physically correct for very high speeds.

---

## 2. Relativistic Model

Relativistic momentum is:

<div align="center" style="font-size:26px;"><b>p = γmv</b></div>

The equation of motion is:

<div align="center" style="font-size:26px;"><b>dp / dt = F</b></div>

For constant force:

<div align="center" style="font-size:26px;"><b>p(t) = Ft</b></div>

Velocity can be found from momentum:

<div align="center" style="font-size:26px;"><b>v = p / √(m² + p²/c²)</b></div>

As time increases, velocity approaches the speed of light:

<div align="center" style="font-size:26px;"><b>v → c</b></div>

but never exceeds it.

---

## 3. RK4 Method

The RK4 method is a numerical method used to solve differential equations.

For position:

<div align="center" style="font-size:26px;"><b>dx / dt = v</b></div>

For velocity in the relativistic case:

<div align="center" style="font-size:26px;"><b>dv / dt = F / (mγ³)</b></div>

where:

<div align="center" style="font-size:26px;"><b>γ = 1 / √(1 − v²/c²)</b></div>

The RK4 method updates velocity and position step by step.

It gives more accurate results than the simple Euler method.

---

## 4. Comparison of Motion

### Classical motion

The classical velocity increases linearly:

<div align="center" style="font-size:26px;"><b>vclassical = at</b></div>

This means the classical particle can exceed the speed of light.

This violates relativity.

### Relativistic motion

The relativistic velocity increases at first, but then the acceleration decreases.

As the velocity gets closer to \(c\), the Lorentz factor increases.

Because of this, more force is needed to produce the same acceleration.

Thus:

<div align="center" style="font-size:26px;"><b>vrelativistic &lt; c</b></div>

---

## 5. Asymptotic Approach to c

At low speeds:

<div align="center" style="font-size:26px;"><b>v ≪ c</b></div>

classical and relativistic results are almost the same.

At high speeds:

<div align="center" style="font-size:26px;"><b>v → c</b></div>

the relativistic velocity approaches the speed of light asymptotically.

This means it gets closer and closer to \(c\), but never reaches or exceeds it.

---

## 6. Energy Difference

Classical kinetic energy:

<div align="center" style="font-size:26px;"><b>Kclassical = 1/2 mv²</b></div>

Relativistic kinetic energy:

<div align="center" style="font-size:26px;"><b>Krelativistic = (γ − 1)mc²</b></div>

At small velocities, these two energies are approximately equal.

At relativistic velocities, the relativistic kinetic energy becomes much larger.

This is because energy goes into increasing the Lorentz factor rather than allowing the object to exceed the speed of light.

---

# Conclusion

The numerical simulation shows that classical and relativistic motion are similar only at low speeds.

In the classical model:

<div align="center" style="font-size:26px;"><b>v = at</b></div>

so velocity grows without limit.

In the relativistic model:

<div align="center" style="font-size:26px;"><b>v → c</b></div>

so the speed approaches the speed of light but never exceeds it.

The RK4 method allows accurate numerical calculation of:

<div align="center" style="font-size:26px;"><b>v(t)</b></div>

and:

<div align="center" style="font-size:26px;"><b>x(t)</b></div>

The main physical result is that relativity prevents any massive object from reaching or exceeding the speed of light.

At high speeds, the energy difference between the classical and relativistic models becomes very large.
