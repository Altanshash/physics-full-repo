# Problem 6 – Damped oscillator

## Given

The equation is

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0
$$

We need to:

1. Derive the general solution for each case.
2. Present the classification of cases: underdamped, critically damped, overdamped.
3. Solve the equation numerically using RK4.
4. Investigate the effect of parameter $b$.
5. Generate the graph of $x(t)$.
6. Generate the phase portrait.


---

## Solution

### 1. General analytical solution

We look for a solution of the form

$$
x(t) = e^{rt}
$$

Then

$$
\frac{dx}{dt} = re^{rt},
\qquad
\frac{d^2x}{dt^2} = r^2 e^{rt}
$$

Substitute into the differential equation:

$$
m r^2 e^{rt} + b r e^{rt} + k e^{rt} = 0
$$

Factor out $e^{rt}$:

$$
e^{rt}(mr^2 + br + k) = 0
$$

Since $e^{rt} \neq 0$, we get the characteristic equation:

$$
mr^2 + br + k = 0
$$

The roots are

$$
r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

So the form of the solution depends on the discriminant

$$
D = b^2 - 4mk
$$

---

### 2. Classification of cases

#### Case 1: Underdamped motion

If

$$
b^2 < 4mk
$$

then the roots are complex:

$$
r = -\frac{b}{2m} \pm i\omega_d
$$

where

$$
\omega_d = \sqrt{\frac{k}{m} - \left(\frac{b}{2m}\right)^2}
$$

Therefore, the solution is

$$
\boxed{
x(t)=e^{-\frac{b}{2m}t}\left(C_1\cos(\omega_d t)+C_2\sin(\omega_d t)\right)
}
$$

This means the oscillator still oscillates, but the amplitude decreases exponentially with time.

---

#### Case 2: Critically damped motion

If

$$
b^2 = 4mk
$$

then the characteristic equation has one repeated root:

$$
r = -\frac{b}{2m}
$$

The solution is

$$
\boxed{
x(t)=(C_1 + C_2 t)e^{-\frac{b}{2m}t}
}
$$

This is the boundary case between oscillatory and non-oscillatory motion.

---

#### Case 3: Overdamped motion

If

$$
b^2 > 4mk
$$

then the roots are real and different:

$$
r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

The solution is

$$
\boxed{
x(t)=C_1 e^{r_1 t} + C_2 e^{r_2 t}
}
$$

In this case there is no oscillation. The system returns to equilibrium slowly.

---

### 3. RK4 numerical solution

To solve the equation numerically, we convert it into a system of first-order equations.

Let

$$
v = \frac{dx}{dt}
$$

Then

$$
\frac{dx}{dt} = v
$$

and from the original equation

$$
m\frac{dv}{dt} + bv + kx = 0
$$

so

$$
\frac{dv}{dt} = -\frac{b}{m}v - \frac{k}{m}x
$$

Thus the system is

$$
\boxed{
\frac{dx}{dt} = v
}
$$

$$
\boxed{
\frac{dv}{dt} = -\frac{b}{m}v - \frac{k}{m}x
}
$$

Now apply the Runge–Kutta 4th order method.

For the variable $x$:

$$
k_1^x = h\,v_n
$$

$$
k_2^x = h\left(v_n + \frac{k_1^v}{2}\right)
$$

$$
k_3^x = h\left(v_n + \frac{k_2^v}{2}\right)
$$

$$
k_4^x = h\left(v_n + k_3^v\right)
$$

For the variable $v$:

$$
k_1^v = h\left(-\frac{b}{m}v_n - \frac{k}{m}x_n\right)
$$

$$
k_2^v = h\left(-\frac{b}{m}\left(v_n+\frac{k_1^v}{2}\right)-\frac{k}{m}\left(x_n+\frac{k_1^x}{2}\right)\right)
$$

$$
k_3^v = h\left(-\frac{b}{m}\left(v_n+\frac{k_2^v}{2}\right)-\frac{k}{m}\left(x_n+\frac{k_2^x}{2}\right)\right)
$$

$$
k_4^v = h\left(-\frac{b}{m}\left(v_n+k_3^v\right)-\frac{k}{m}\left(x_n+k_3^x\right)\right)
$$

Then update:

$$
x_{n+1} = x_n + \frac{1}{6}(k_1^x + 2k_2^x + 2k_3^x + k_4^x)
$$

$$
v_{n+1} = v_n + \frac{1}{6}(k_1^v + 2k_2^v + 2k_3^v + k_4^v)
$$

This gives the numerical trajectory of the damped oscillator.

---

### 4. Effect of parameter $b$

The parameter $b$ is the damping coefficient.

- If $b$ is small, the system oscillates for a long time.
- If $b$ increases, the oscillations decay faster.
- At the critical value

$$
b_c = 2\sqrt{mk}
$$

the motion becomes critically damped.
- If $b > b_c$, the motion is overdamped and there is no oscillation.

So, increasing $b$ changes the system from:

1. underdamped  
2. critically damped  
3. overdamped

---

### 5. Graph of $x(t)$

The graph of displacement versus time depends on the damping regime.

#### Underdamped
- The graph oscillates around zero.
- The amplitude decreases exponentially.

#### Critically damped
- The graph returns to zero as fast as possible without oscillation.

#### Overdamped
- The graph returns to zero slowly without oscillation.

So the shape of $x(t)$ clearly shows the effect of damping.

---

### 6. Phase portrait

The phase portrait is the graph of

$$
v(t) \text{ versus } x(t)
$$

It shows the motion in phase space.

#### Underdamped
- The trajectory spirals toward the origin.
- This means the system oscillates while losing energy.

#### Critically damped
- The trajectory approaches the origin without spiraling.
- This is the fastest non-oscillatory return.

#### Overdamped
- The trajectory approaches the origin slowly, also without spiraling.

The origin

$$
(x,v) = (0,0)
$$

is the equilibrium point.

---

## Final Answer

The damped oscillator equation

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0
$$

has the characteristic equation

$$
mr^2 + br + k = 0
$$

with roots

$$
r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

Therefore:

### Underdamped

$$
\boxed{
x(t)=e^{-\frac{b}{2m}t}\left(C_1\cos(\omega_d t)+C_2\sin(\omega_d t)\right)
}
$$

where

$$
\omega_d = \sqrt{\frac{k}{m} - \left(\frac{b}{2m}\right)^2}
$$

### Critically damped

$$
\boxed{
x(t)=(C_1 + C_2 t)e^{-\frac{b}{2m}t}
}
$$

### Overdamped

$$
\boxed{
x(t)=C_1 e^{r_1 t} + C_2 e^{r_2 t}
}
$$

The critical damping value is

$$
\boxed{
b_c = 2\sqrt{mk}
}
$$

The RK4 numerical model is based on

$$
\frac{dx}{dt}=v,
\qquad
\frac{dv}{dt}=-\frac{b}{m}v-\frac{k}{m}x
$$

The graph $x(t)$ and the phase portrait change significantly with the value of $b$.

---

## Conclusion

The damped oscillator has three regimes depending on the value of the damping coefficient $b$.

- For small $b$, the motion is oscillatory with decaying amplitude.
- At critical damping, the system returns to equilibrium as fast as possible without oscillation.
- For large $b$, the motion is non-oscillatory and slower.

The RK4 method allows us to compute the numerical solution, plot $x(t)$, and draw the phase portrait.  
The parameter $b$ controls how fast the energy is lost and how the system approaches equilibrium.
