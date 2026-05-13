# Problem 3 — Lorentz Transformation

## Given

Two events are given in frame S:

$$
x_1 = 0, \quad t_1 = 0
$$

$$
x_2 = 900 \text{ m}, \quad t_2 = 4 \text{ microseconds}
$$

Frame S' moves with velocity:

$$
v = 0.6c
$$

Speed of light:

$$
c = 3 \times 10^8 \text{ m/s}
$$

Lorentz transformations:

$$
x' = \gamma (x - vt)
$$

$$
t' = \gamma (t - vx / c^2)
$$

Spacetime interval:

$$
s^2 = c^2t^2 - x^2
$$

---

# Solution

## 1. Lorentz Factor

$$
\gamma = 1 / \sqrt{1 - v^2 / c^2}
$$

Since:

$$
v = 0.6c
$$

then:

$$
\gamma = 1 / \sqrt{1 - 0.6^2}
$$

$$
\gamma = 1 / \sqrt{1 - 0.36}
$$

$$
\gamma = 1 / \sqrt{0.64}
$$

$$
\gamma = 1 / 0.8
$$

$$
\gamma = 1.25
$$

---

## 2. Transform the Position Coordinate

Given:

$$
x = 900 \text{ m}
$$

$$
t = 4 \times 10^{-6} \text{ s}
$$

Velocity:

$$
v = 0.6 \times 3 \times 10^8
$$

$$
v = 1.8 \times 10^8 \text{ m/s}
$$

First calculate:

$$
vt = (1.8 \times 10^8)(4 \times 10^{-6})
$$

$$
vt = 720 \text{ m}
$$

Now calculate:

$$
x' = 1.25(900 - 720)
$$

$$
x' = 1.25(180)
$$

$$
x' = 225 \text{ m}
$$

---

## 3. Transform the Time Coordinate

Formula:

$$
t' = \gamma (t - vx / c^2)
$$

First calculate:

$$
vx = (1.8 \times 10^8)(900)
$$

$$
vx = 1.62 \times 10^{11}
$$

Calculate:

$$
c^2 = (3 \times 10^8)^2
$$

$$
c^2 = 9 \times 10^{16}
$$

Now:

$$
vx / c^2 = (1.62 \times 10^{11}) / (9 \times 10^{16})
$$

$$
vx / c^2 = 1.8 \times 10^{-6} \text{ s}
$$

Now substitute:

$$
t' = 1.25(4 \times 10^{-6} - 1.8 \times 10^{-6})
$$

$$
t' = 1.25(2.2 \times 10^{-6})
$$

$$
t' = 2.75 \times 10^{-6} \text{ s}
$$

$$
t' = 2.75 \text{ microseconds}
$$

---

## 4. Can the Order of Events Change?

The first event occurs at:

$$
t_1' = 0
$$

The second event occurs at:

$$
t_2' = 2.75 \text{ microseconds}
$$

Since:

$$
t_2' > t_1'
$$

the order of events does not change.

Also:

$$
c \Delta t = (3 \times 10^8)(4 \times 10^{-6})
$$

$$
c \Delta t = 1200 \text{ m}
$$

and:

$$
\Delta x = 900 \text{ m}
$$

Since:

$$
1200 > 900
$$

the interval is timelike.

Therefore, the order of events cannot change in any inertial frame.

---

## 5. Spacetime Interval in Frame S

Formula:

$$
s^2 = c^2t^2 - x^2
$$

This can be written as:

$$
s^2 = (ct)^2 - x^2
$$

First:

$$
ct = 1200 \text{ m}
$$

So:

$$
s^2 = 1200^2 - 900^2
$$

$$
s^2 = 1440000 - 810000
$$

$$
s^2 = 630000 \text{ m}^2
$$

---

## 6. Verify Invariance in Frame S'

In frame S':

$$
x' = 225 \text{ m}
$$

$$
t' = 2.75 \times 10^{-6} \text{ s}
$$

Calculate:

$$
ct' = (3 \times 10^8)(2.75 \times 10^{-6})
$$

$$
ct' = 825 \text{ m}
$$

Now:

$$
s'^2 = 825^2 - 225^2
$$

$$
s'^2 = 680625 - 50625
$$

$$
s'^2 = 630000 \text{ m}^2
$$

So:

$$
s'^2 = s^2
$$

---

# Conclusion

The transformed coordinates of the second event in frame S' are:

$$
x_2' = 225 \text{ m}
$$

$$
t_2' = 2.75 \text{ microseconds}
$$

The order of events does not change.

The spacetime interval is:

$$
s^2 = 630000 \text{ m}^2
$$

The interval is the same in both frames:

$$
s'^2 = s^2
$$

Therefore, the spacetime interval is invariant under Lorentz transformation.
