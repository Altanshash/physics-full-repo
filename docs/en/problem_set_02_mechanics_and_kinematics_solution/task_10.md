## Problem 10 – Analysis of motion from numerical data

### Given

The motion is given by

$$
x(t)=t+\frac{1}{20}t^2
$$

on the interval

$$
t\in[0,10]
$$

with time step

$$
\Delta t=0.1
$$

Find:

1. Approximate the velocity using the finite difference method
2. Approximate the acceleration using the finite difference method
3. Compare with the analytical solution
4. Investigate the effect of the time step on accuracy

---

### Solution

#### 1. Analytical solution

The given function is

$$
x(t)=t+\frac{1}{20}t^2
$$

The analytical velocity is the derivative of $x(t)$:

$$
v(t)=\frac{dx}{dt}=1+\frac{1}{10}t
$$

The analytical acceleration is the derivative of $v(t)$:

$$
a(t)=\frac{dv}{dt}=\frac{1}{10}
$$

Therefore,

$$
\boxed{v(t)=1+0.1t}
$$

$$
\boxed{a(t)=0.1}
$$

---

#### 2. Numerical approximation of velocity

Let

$$
t_n=n\Delta t, \qquad x_n=x(t_n)
$$

where

$$
\Delta t=0.1
$$

To approximate the velocity, we use the finite difference formula.

For interior points, the central difference formula is

$$
v_n \approx \frac{x_{n+1}-x_{n-1}}{2\Delta t}
$$

At the left boundary, we use the forward difference:

$$
v_0 \approx \frac{x_1-x_0}{\Delta t}
$$

At the right boundary, we use the backward difference:

$$
v_N \approx \frac{x_N-x_{N-1}}{\Delta t}
$$

Now compute the position values:

$$
x(t)=t+\frac{1}{20}t^2
$$

For example:

$$
x(0)=0
$$

$$
x(0.1)=0.1+\frac{1}{20}(0.1)^2=0.1005
$$

$$
x(0.2)=0.2+\frac{1}{20}(0.2)^2=0.202
$$

Then,

$$
v(0)\approx \frac{x(0.1)-x(0)}{0.1}=\frac{0.1005-0}{0.1}=1.005
$$

At the interior point $t=0.1$:

$$
v(0.1)\approx \frac{x(0.2)-x(0)}{2\cdot0.1}
=\frac{0.202-0}{0.2}=1.01
$$

At $t=1$:

$$
x(0.9)=0.9+\frac{1}{20}(0.9)^2=0.9405
$$

$$
x(1.1)=1.1+\frac{1}{20}(1.1)^2=1.1605
$$

Thus,

$$
v(1)\approx \frac{x(1.1)-x(0.9)}{0.2}
=\frac{1.1605-0.9405}{0.2}=1.1
$$

which agrees with the analytical value

$$
v(1)=1+0.1\cdot1=1.1
$$

So the numerical velocity approximation is very accurate.

---

#### 3. Numerical approximation of acceleration

To approximate the acceleration, we use the second central difference formula:

$$
a_n \approx \frac{x_{n+1}-2x_n+x_{n-1}}{(\Delta t)^2}
$$

At $t=0.1$:

$$
a(0.1)\approx \frac{x(0.2)-2x(0.1)+x(0)}{(0.1)^2}
$$

Substitute the values:

$$
a(0.1)\approx \frac{0.202-2(0.1005)+0}{0.01}
$$

$$
a(0.1)\approx \frac{0.202-0.201}{0.01}
=\frac{0.001}{0.01}=0.1
$$

At $t=1$:

$$
x(0.9)=0.9405,\qquad x(1)=1.05,\qquad x(1.1)=1.1605
$$

Then

$$
a(1)\approx \frac{1.1605-2(1.05)+0.9405}{0.01}
$$

$$
a(1)\approx \frac{1.1605-2.1+0.9405}{0.01}
=\frac{0.001}{0.01}=0.1
$$

Thus, the numerical acceleration also agrees with the analytical value:

$$
\boxed{a(t)\approx 0.1}
$$

---

#### 4. Comparison with the analytical solution

The analytical results are

$$
v(t)=1+0.1t
$$

$$
a(t)=0.1
$$

The numerical approximations using finite differences give nearly the same values.

In fact:

- the central difference formula reproduces the exact derivative for this quadratic function when computing the velocity at interior points
- the second central difference formula reproduces the exact constant acceleration

Thus, for this problem, the finite difference method gives very accurate results.

---

#### 5. Effect of the time step on accuracy

The accuracy of finite difference approximations depends on the size of the time step $\Delta t$.

- A smaller $\Delta t$ usually gives higher accuracy
- A larger $\Delta t$ usually gives larger numerical error

For this particular function,

$$
x(t)=t+\frac{1}{20}t^2
$$

the position is quadratic in time.

Because of this:

- the central difference formula gives the exact velocity at interior points
- the second central difference formula gives the exact acceleration

So even for $\Delta t=0.1$, the result is already exact at interior points up to rounding.

However, in more general problems, reducing $\Delta t$ improves the approximation.

For example:

- if $\Delta t=0.5$, the approximation is coarser
- if $\Delta t=0.1$, the approximation is better
- if $\Delta t=0.01$, the approximation is even more accurate

Therefore, the time step strongly affects accuracy in general, although for this quadratic example the finite difference method performs especially well.

---

### Final Conclusion

For the motion

$$
x(t)=t+\frac{1}{20}t^2
$$

the analytical velocity and acceleration are

$$
\boxed{v(t)=1+0.1t}
$$

$$
\boxed{a(t)=0.1}
$$

Using the finite difference method with

$$
\Delta t=0.1
$$

the numerical approximations of velocity and acceleration agree with the analytical solution.

Thus, the finite difference method gives very accurate results for this problem. In general, decreasing the time step improves the accuracy of numerical differentiation.
