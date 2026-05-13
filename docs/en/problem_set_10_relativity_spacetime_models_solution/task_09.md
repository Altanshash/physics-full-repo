# Problem 9 — Schwarzschild Radius

## Given

The Schwarzschild radius formula is:

$$
r_s = \frac{2GM}{c^2}
$$

where:

$$
G = 6.67 \times 10^{-11}\ \text{N·m}^2/\text{kg}^2
$$

$$
c = 3.00 \times 10^8\ \text{m/s}
$$

Mass of the Sun:

$$
M_{\text{Sun}} = 1.99 \times 10^{30}\ \text{kg}
$$

Mass of the Earth:

$$
M_{\text{Earth}} = 5.97 \times 10^{24}\ \text{kg}
$$

---

# Solution

## 1. Schwarzschild Radius of the Sun

Use the formula:

$$
r_s = \frac{2GM}{c^2}
$$

Substitute the values:

$$
r_s =
\frac{
2(6.67 \times 10^{-11})(1.99 \times 10^{30})
}{
(3.00 \times 10^8)^2
}
$$

Calculate the denominator:

$$
(3.00 \times 10^8)^2
=
9.00 \times 10^{16}
$$

Calculate the numerator:

$$
2(6.67 \times 10^{-11})(1.99 \times 10^{30})
\approx
2.65 \times 10^{20}
$$

Now divide:

$$
r_s =
\frac{
2.65 \times 10^{20}
}{
9.00 \times 10^{16}
}
$$

$$
r_s \approx 2.95 \times 10^3\ \text{m}
$$

Therefore:

$$
r_s \approx 2.95\ \text{km}
$$

---

## 2. Schwarzschild Radius of the Earth

Use:

$$
r_s = \frac{2GM}{c^2}
$$

Substitute the values:

$$
r_s =
\frac{
2(6.67 \times 10^{-11})(5.97 \times 10^{24})
}{
(3.00 \times 10^8)^2
}
$$

Calculate the numerator:

$$
2(6.67 \times 10^{-11})(5.97 \times 10^{24})
\approx
7.96 \times 10^{14}
$$

Calculate the denominator:

$$
(3.00 \times 10^8)^2
=
9.00 \times 10^{16}
$$

Now divide:

$$
r_s =
\frac{
7.96 \times 10^{14}
}{
9.00 \times 10^{16}
}
$$

$$
r_s \approx 8.84 \times 10^{-3}\ \text{m}
$$

Therefore:

$$
r_s \approx 8.84\ \text{mm}
$$

---

# 3. Redshift at \( r = 1.5r_s \)

The gravitational redshift is:

$$
z =
\frac{
1
}{
\sqrt{
1 - \frac{r_s}{r}
}
}
- 1
$$

Given:

$$
r = 1.5r_s
$$

Substitute into the formula:

$$
z =
\frac{
1
}{
\sqrt{
1 - \frac{r_s}{1.5r_s}
}
}
- 1
$$

Cancel \( r_s \):

$$
z =
\frac{
1
}{
\sqrt{
1 - \frac{1}{1.5}
}
}
- 1
$$

Since:

$$
\frac{1}{1.5}
=
\frac{2}{3}
$$

then:

$$
z =
\frac{
1
}{
\sqrt{
1 - \frac{2}{3}
}
}
- 1
$$

$$
z =
\frac{
1
}{
\sqrt{
\frac{1}{3}
}
}
- 1
$$

$$
z =
\sqrt{3} - 1
$$

$$
z \approx 0.732
$$

Therefore:

$$
z \approx 73.2\%
$$

---

## 4. What Happens as \( r \to r_s \)?

The redshift formula is:

$$
z =
\frac{
1
}{
\sqrt{
1 - \frac{r_s}{r}
}
}
- 1
$$

As:

$$
r \to r_s
$$

then:

$$
\frac{r_s}{r}
\to
1
$$

Therefore:

$$
1 - \frac{r_s}{r}
\to
0
$$

So:

$$
z \to \infty
$$

This means the emitted light becomes infinitely redshifted for a distant observer.

---

## 5. Interpretation of the Event Horizon

The surface:

$$
r = r_s
$$

is called the event horizon.

At this radius, the escape velocity becomes equal to the speed of light.

Therefore:

$$
v_{\text{escape}} = c
$$

Inside this boundary, nothing can escape, not even light.

A distant observer sees objects approaching the event horizon become increasingly redshifted and appear to freeze in time.

---

# Conclusion

The Schwarzschild radius formula is:

$$
r_s = \frac{2GM}{c^2}
$$

For the Sun:

$$
r_s \approx 2.95\ \text{km}
$$

For the Earth:

$$
r_s \approx 8.84\ \text{mm}
$$

At:

$$
r = 1.5r_s
$$

the gravitational redshift is:

$$
z \approx 0.732
$$

or:

$$
73.2\%
$$

As:

$$
r \to r_s
$$

the redshift becomes infinite:

$$
z \to \infty
$$

The Schwarzschild radius represents the event horizon of a black hole. Inside this radius, no light or information can escape.
