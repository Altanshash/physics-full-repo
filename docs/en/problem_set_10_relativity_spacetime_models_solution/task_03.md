# Problem 3 — Lorentz Transformation

## Given

Two events are given in frame \(S\):

$$
x_1 = 0, \qquad t_1 = 0
$$

$$
x_2 = 900 \text{ m}, \qquad t_2 = 4 \ \mu s
$$

Frame \(S'\) moves with velocity:

$$
v = 0.6c
$$

The Lorentz transformations are:

$$
x' = \gamma (x - vt)
$$

$$
t' = \gamma \left(t - \frac{vx}{c^2}\right)
$$

The spacetime interval is:

$$
s^2 = c^2t^2 - x^2
$$

### Find:

1. The transformed coordinates of the second event in \(S'\)
2. Whether the order of events can change
3. The spacetime interval
4. Verification that the interval is invariant

---

# Solution

## 1. Calculate the Lorentz Factor

Given:

$$
v = 0.6c
$$

The Lorentz factor is:

$$
\gamma = \frac{1}{\sqrt{1-\frac{v^2}{c^2}}}
$$

Substitute:

$$
\gamma = \frac{1}{\sqrt{1-0.6^2}}
$$

$$
\gamma = \frac{1}{\sqrt{1-0.36}}
$$

$$
\gamma = \frac{1}{\sqrt{0.64}}
$$

$$
\gamma = \frac{1}{0.8}
$$

$$
\gamma = 1.25
$$

---

## 2. Transform the Second Event

For the second event:

$$
x_2 = 900 \text{ m}
$$

$$
t_2 = 4 \ \mu s = 4 \times 10^{-6} \text{ s}
$$

Use:

$$
x' = \gamma (x - vt)
$$

Since:

$$
c = 3 \times 10^8 \text{ m/s}
$$

then:

$$
v = 0.6c = 1.8 \times 10^8 \text{ m/s}
$$

Calculate:

$$
vt = (1.8 \times 10^8)(4 \times 10^{-6})
$$

$$
vt = 720 \text{ m}
$$

Now:

$$
x_2' = 1.25(900 - 720)
$$

$$
x_2' = 1.25(180)
$$

$$
x_2' = 225 \text{ m}
$$

Therefore:

$$
x_2' = 225 \text{ m}
$$

---

## 3. Transform the Time Coordinate

Use:

$$
t' = \gamma \left(t - \frac{vx}{c^2}\right)
$$

First calculate:

$$
\frac{vx}{c^2}
=
\frac{(0.6c)(900)}{c^2}
$$

$$
\frac{vx}{c^2}
=
\frac{0.6 \times 900}{c}
$$

$$
\frac{vx}{c^2}
=
\frac{540}{3 \times 10^8}
$$

$$
\frac{vx}{c^2}
=
1.8 \times 10^{-6} \text{ s}
$$

Now:

$$
t_2' = 1.25(4 \times 10^{-6} - 1.8 \times 10^{-6})
$$

$$
t_2' = 1.25(2.2 \times 10^{-6})
$$

$$
t_2' = 2.75 \times 10^{-6} \text{ s}
$$

So:

$$
t_2' = 2.75 \ \mu s
$$

Therefore, the second event in frame \(S'\) is:

$$
x_2' = 225 \text{ m}
$$

$$
t_2' = 2.75 \ \mu s
$$

---

## 4. Can the Order of Events Change?

The first event is:

$$
x_1 = 0, \qquad t_1 = 0
$$

After transformation:

$$
x_1' = 0, \qquad t_1' = 0
$$

The second event has:

$$
t_2' = 2.75 \ \mu s
$$

Since:

$$
t_2' > t_1'
$$

the order of events does not change in this frame.

To check whether the order can change in any frame, compare:

$$
c\Delta t
$$

and:

$$
\Delta x
$$

Here:

$$
c\Delta t = (3 \times 10^8)(4 \times 10^{-6})
$$

$$
c\Delta t = 1200 \text{ m}
$$

and:

$$
\Delta x = 900 \text{ m}
$$

Since:

$$
c\Delta t > \Delta x
$$

the interval is timelike.

For timelike-separated events, the time order cannot change in any inertial frame.

Therefore:

$$
\text{The order of events cannot change.}
$$

---

## 5. Calculate the Spacetime Interval in Frame \(S\)

The spacetime interval is:

$$
s^2 = c^2t^2 - x^2
$$

Substitute:

$$
s^2 = (3 \times 10^8)^2(4 \times 10^{-6})^2 - 900^2
$$

Calculate:

$$
ct = (3 \times 10^8)(4 \times 10^{-6})
$$

$$
ct = 1200 \text{ m}
$$

Therefore:

$$
s^2 = 1200^2 - 900^2
$$

$$
s^2 = 1,440,000 - 810,000
$$

$$
s^2 = 630,000 \text{ m}^2
$$

So:

$$
s^2 = 6.3 \times 10^5 \text{ m}^2
$$

---

## 6. Verify Invariance in Frame \(S'\)

In frame \(S'\):

$$
x_2' = 225 \text{ m}
$$

$$
t_2' = 2.75 \ \mu s
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
s'^2 = c^2t'^2 - x'^2
$$

$$
s'^2 = 825^2 - 225^2
$$

$$
s'^2 = 680,625 - 50,625
$$

$$
s'^2 = 630,000 \text{ m}^2
$$

Therefore:

$$
s'^2 = s^2
$$

The spacetime interval is invariant.

---

# Conclusion

For the second event, the coordinates in frame \(S'\) are:

$$
x_2' = 225 \text{ m}
$$

$$
t_2' = 2.75 \ \mu s
$$

The order of events does not change because the interval is timelike:

$$
c\Delta t > \Delta x
$$

The spacetime interval in frame \(S\) is:

$$
s^2 = 6.3 \times 10^5 \text{ m}^2
$$

The spacetime interval in frame \(S'\) is:

$$
s'^2 = 6.3 \times 10^5 \text{ m}^2
$$

Thus:

$$
s^2 = s'^2
$$

This confirms that the spacetime interval is invariant under Lorentz transformation.
