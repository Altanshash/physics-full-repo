# Problem 6 – Curve length and numerical integration

## Given

A parametric trajectory in 2D is

$$
x(t)=t, \qquad y(t)=t^2, \qquad t\in[0,1]
$$

We need to:

1. determine the velocity vector,
2. determine the magnitude of the velocity,
3. write the arc length as an integral,
4. compute the integral analytically if possible,
5. implement the trapezoidal rule in HTML/JS.

---

## 1. Velocity vector

The position vector is

$$
\vec r(t) = (t, t^2)
$$

Differentiate each component:

$$
\vec v(t) = \frac{d\vec r}{dt} = (1, 2t)
$$

---

## 2. Magnitude of the velocity

$$
|\vec v(t)| = \sqrt{1^2 + (2t)^2}
$$

$$
|\vec v(t)| = \sqrt{1+4t^2}
$$

---

## 3. Arc length integral

The arc length is

$$
s=\int_0^1 |\vec v(t)|\,dt
$$

So,

$$
s=\int_0^1 \sqrt{1+4t^2}\,dt
$$

---

## 4. Analytical calculation

Use the substitution

$$
u=2t, \qquad dt=\frac{du}{2}
$$

Then

$$
s=\frac12\int_0^2 \sqrt{1+u^2}\,du
$$

Using the standard formula

$$
\int \sqrt{1+u^2}\,du
=
\frac12\left(u\sqrt{1+u^2}+\ln\left|u+\sqrt{1+u^2}\right|\right)
$$

we get

$$
s
=
\frac14
\left[
u\sqrt{1+u^2}+\ln\left|u+\sqrt{1+u^2}\right|
\right]_0^2
$$

Therefore,

$$
s=\frac14\left(2\sqrt5+\ln(2+\sqrt5)\right)
$$

So,

$$
s=\frac{\sqrt5}{2}+\frac14\ln(2+\sqrt5)
$$

Approximate value:

$$
s \approx 1.47894
$$

---

## 5. Trapezoidal rule

Let

$$
f(t)=\sqrt{1+4t^2}
$$

Divide $[0,1]$ into $N$ equal parts:

$$
h=\frac1N, \qquad t_i=\frac{i}{N}
$$

Then the trapezoidal approximation is

$$
s_N=\frac{h}{2}\left[f(t_0)+2\sum_{i=1}^{N-1}f(t_i)+f(t_N)\right]
$$

That is,

$$
s_N=\frac{1}{2N}\left[f(0)+2\sum_{i=1}^{N-1}f\left(\frac{i}{N}\right)+f(1)\right]
$$

The error is

$$
E_N = |s_N-s|
$$

---

## Simple HTML/JS code

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Problem 6</title>
</head>
<body>
  <h1>Problem 6 – Curve length</h1>

  <label for="N">N:</label>
  <input id="N" type="number" value="10" min="1" />
  <button onclick="calculate()">Compute</button>

  <pre id="out"></pre>

  <script>
    function f(t) {
      return Math.sqrt(1 + 4 * t * t);
    }

    function exactLength() {
      return Math.sqrt(5) / 2 + 0.25 * Math.log(2 + Math.sqrt(5));
    }

    function trapezoidal(N) {
      const h = 1 / N;
      let sum = 0.5 * (f(0) + f(1));
      for (let i = 1; i < N; i++) {
        sum += f(i * h);
      }
      return h * sum;
    }

    function calculate() {
      const N = parseInt(document.getElementById("N").value, 10);
      const exact = exactLength();
      const approx = trapezoidal(N);
      const error = Math.abs(approx - exact);

      document.getElementById("out").textContent =
        "v(t) = (1, 2t)\n" +
        "|v(t)| = sqrt(1 + 4t^2)\n" +
        "Exact length = " + exact.toFixed(10) + "\n" +
        "Trapezoidal result = " + approx.toFixed(10) + "\n" +
        "Error = " + error.toExponential(6);
    }

    calculate();
  </script>
</body>
</html>
