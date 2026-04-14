# Problem 6 – Curve length and numerical integration

## Given

A parametric trajectory in 2D is given by

$$
x(t) = t, \qquad y(t) = t^2, \qquad t \in [0,1]
$$

Determine:

1. the velocity vector
   $$
   \vec v(t) = \frac{d\vec r}{dt},
   $$
2. the magnitude of the velocity $|\vec v(t)|$,
3. write the arc length of the trajectory as an integral
   $$
   s = \int_0^1 |\vec v(t)|\,dt,
   $$
4. calculate this integral analytically if possible, or reduce it to a form that requires a numerical method,
5. implement the trapezoidal rule in HTML/JS to calculate $s$,
   - check the convergence of the result with increasing number of divisions $N$,
   - plot the error as a function of $N$.

Requirement: visualization of the trajectory and the ability to change $N$ in the application.

---

## 1. Velocity vector

The position vector is

$$
\vec r(t) = (x(t),y(t)) = (t,t^2)
$$

Differentiate each component:

$$
\vec v(t) = \frac{d\vec r}{dt} = \left(\frac{dx}{dt},\frac{dy}{dt}\right)
$$

Since

$$
\frac{dx}{dt} = 1, \qquad \frac{dy}{dt} = 2t
$$

we get

$$
\vec v(t) = (1,2t)
$$

---

## 2. Magnitude of the velocity

The magnitude of the velocity is

$$
|\vec v(t)| = \sqrt{1^2 + (2t)^2}
$$

Therefore,

$$
|\vec v(t)| = \sqrt{1+4t^2}
$$

---

## 3. Arc length as an integral

The arc length of the trajectory from $t=0$ to $t=1$ is

$$
s = \int_0^1 |\vec v(t)|\,dt
$$

Substitute the expression for $|\vec v(t)|$:

$$
s = \int_0^1 \sqrt{1+4t^2}\,dt
$$

---

## 4. Analytical calculation of the integral

We need to compute

$$
s = \int_0^1 \sqrt{1+4t^2}\,dt
$$

Use the substitution

$$
u = 2t
$$

Then

$$
du = 2\,dt, \qquad dt = \frac{du}{2}
$$

When

$$
t=0, \quad u=0
$$

and when

$$
t=1, \quad u=2
$$

So the integral becomes

$$
s = \frac{1}{2}\int_0^2 \sqrt{1+u^2}\,du
$$

Now use the standard formula

$$
\int \sqrt{1+u^2}\,du
=
\frac{1}{2}\left(u\sqrt{1+u^2}+\ln\left|u+\sqrt{1+u^2}\right|\right)
$$

Therefore,

$$
s
=
\frac{1}{2}\cdot
\frac{1}{2}
\left[
u\sqrt{1+u^2}+\ln\left|u+\sqrt{1+u^2}\right|
\right]_0^2
$$

So,

$$
s
=
\frac{1}{4}
\left[
u\sqrt{1+u^2}+\ln\left|u+\sqrt{1+u^2}\right|
\right]_0^2
$$

Now evaluate at the bounds.

At

$$
u=2
$$

we get

$$
2\sqrt{5}+\ln(2+\sqrt{5})
$$

At

$$
u=0
$$

we get

$$
0+\ln(1)=0
$$

Hence,

$$
s = \frac{1}{4}\left(2\sqrt{5}+\ln(2+\sqrt{5})\right)
$$

So the exact arc length is

$$
s = \frac{\sqrt{5}}{2} + \frac{1}{4}\ln(2+\sqrt{5})
$$

Approximate value:

$$
s \approx 1.47894
$$

---

## 5. Trapezoidal rule

To approximate

$$
s = \int_0^1 \sqrt{1+4t^2}\,dt
$$

using the trapezoidal rule, divide the interval $[0,1]$ into $N$ equal parts.

The step size is

$$
h = \frac{1-0}{N} = \frac{1}{N}
$$

Let

$$
t_i = ih, \qquad i=0,1,2,\dots,N
$$

and define

$$
f(t) = \sqrt{1+4t^2}
$$

Then the trapezoidal approximation is

$$
s_N =
\frac{h}{2}
\left[
f(t_0) + 2\sum_{i=1}^{N-1} f(t_i) + f(t_N)
\right]
$$

That is,

$$
s_N =
\frac{1}{2N}
\left[
f(0) + 2\sum_{i=1}^{N-1} f\left(\frac{i}{N}\right) + f(1)
\right]
$$

where

$$
f(t)=\sqrt{1+4t^2}
$$

The absolute error is

$$
E_N = |s_N - s|
$$

where $s$ is the exact value

$$
s = \frac{\sqrt{5}}{2} + \frac{1}{4}\ln(2+\sqrt{5})
$$

As $N$ increases, the trapezoidal result should converge to the exact arc length.

---

## HTML/JS implementation

Save the following as `problem6.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Problem 6 - Curve Length and Numerical Integration</title>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      line-height: 1.5;
    }
    h1, h2 {
      margin-bottom: 10px;
    }
    .controls {
      margin-bottom: 20px;
      padding: 12px;
      border: 1px solid #ccc;
      border-radius: 8px;
      max-width: 500px;
    }
    label {
      display: inline-block;
      width: 140px;
    }
    input[type="number"] {
      width: 120px;
      padding: 4px;
    }
    button {
      margin-top: 10px;
      padding: 8px 14px;
      cursor: pointer;
    }
    .result {
      margin-top: 16px;
      padding: 12px;
      background: #f5f5f5;
      border-radius: 8px;
      max-width: 700px;
    }
    canvas {
      margin-top: 20px;
      max-width: 900px;
    }
  </style>
</head>
<body>
  <h1>Problem 6 - Curve Length and Numerical Integration</h1>

  <p>Curve: <strong>x(t) = t, y(t) = t², t ∈ [0,1]</strong></p>

  <div class="controls">
    <div>
      <label for="nValue">Divisions N:</label>
      <input id="nValue" type="number" min="1" value="10" />
    </div>
    <button id="updateBtn">Calculate</button>
  </div>

  <div class="result" id="output"></div>

  <h2>Trajectory</h2>
  <canvas id="trajectoryChart"></canvas>

  <h2>Error vs N</h2>
  <canvas id="errorChart"></canvas>

  <script>
    // Exact arc length:
    // s = sqrt(5)/2 + (1/4) ln(2 + sqrt(5))
    function exactArcLength() {
      return Math.sqrt(5) / 2 + 0.25 * Math.log(2 + Math.sqrt(5));
    }

    // Speed function |v(t)| = sqrt(1 + 4 t^2)
    function speed(t) {
      return Math.sqrt(1 + 4 * t * t);
    }

    // Trapezoidal rule on [0,1]
    function trapezoidal(N) {
      const h = 1 / N;
      let sum = 0.5 * (speed(0) + speed(1));

      for (let i = 1; i < N; i++) {
        const t = i * h;
        sum += speed(t);
      }

      return h * sum;
    }

    // Build trajectory points
    function buildTrajectoryPoints(numPoints = 200) {
      const points = [];
      for (let i = 0; i <= numPoints; i++) {
        const t = i / numPoints;
        points.push({ x: t, y: t * t });
      }
      return points;
    }

    let trajectoryChart;
    let errorChart;

    function createTrajectoryChart() {
      const ctx = document.getElementById("trajectoryChart").getContext("2d");
      trajectoryChart = new Chart(ctx, {
        type: "scatter",
        data: {
          datasets: [
            {
              label: "Trajectory y = x²",
              data: buildTrajectoryPoints(),
              showLine: true,
              pointRadius: 0,
              borderWidth: 2
            }
          ]
        },
        options: {
          responsive: true,
          scales: {
            x: {
              type: "linear",
              min: 0,
              max: 1,
              title: {
                display: true,
                text: "x"
              }
            },
            y: {
              min: 0,
              max: 1,
              title: {
                display: true,
                text: "y"
              }
            }
          }
        }
      });
    }

    function createErrorChart() {
      const ctx = document.getElementById("errorChart").getContext("2d");
      errorChart = new Chart(ctx, {
        type: "line",
        data: {
          labels: [],
          datasets: [
            {
              label: "Absolute error",
              data: [],
              borderWidth: 2,
              fill: false
            }
          ]
        },
        options: {
          responsive: true,
          scales: {
            x: {
              title: {
                display: true,
                text: "N"
              }
            },
            y: {
              title: {
                display: true,
                text: "Error"
              }
            }
          }
        }
      });
    }

    function updateAll() {
      const N = parseInt(document.getElementById("nValue").value, 10);

      if (!Number.isInteger(N) || N < 1) {
        alert("Please enter an integer N >= 1.");
        return;
      }

      const exact = exactArcLength();
      const approx = trapezoidal(N);
      const error = Math.abs(approx - exact);

      const output = document.getElementById("output");
      output.innerHTML = `
        <p><strong>Velocity vector:</strong> v(t) = (1, 2t)</p>
        <p><strong>Speed:</strong> |v(t)| = √(1 + 4t²)</p>
        <p><strong>Exact arc length:</strong> ${exact.toFixed(10)}</p>
        <p><strong>Trapezoidal approximation for N = ${N}:</strong> ${approx.toFixed(10)}</p>
        <p><strong>Absolute error:</strong> ${error.toExponential(6)}</p>
      `;

      // Build error data for N = 1..maxN
      const maxN = Math.max(2, N);
      const labels = [];
      const errors = [];

      for (let k = 1; k <= maxN; k++) {
        labels.push(k);
        errors.push(Math.abs(trapezoidal(k) - exact));
      }

      errorChart.data.labels = labels;
      errorChart.data.datasets[0].data = errors;
      errorChart.update();
    }

    document.getElementById("updateBtn").addEventListener("click", updateAll);

    createTrajectoryChart();
    createErrorChart();
    updateAll();
  </script>
</body>
</html>
