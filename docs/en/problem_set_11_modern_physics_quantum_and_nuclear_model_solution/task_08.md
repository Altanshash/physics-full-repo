# Problem 8 – Radioactive Decay  
## Probabilistic Model

## Given

Number of undecayed nuclei:

$$
N(t)=N_0e^{-\lambda t}
$$

where:

$$
N_0
$$

is the initial number of nuclei,

$$
\lambda
$$

is the decay constant,

$$
t
$$

is time.

---

## Solution

### 1. Monte Carlo simulation idea

In the probabilistic model, each nucleus decays randomly.

The decay time of each nucleus follows an exponential distribution:

$$
P(t)=\lambda e^{-\lambda t}
$$

For each nucleus, we generate a random decay time:

$$
t_i = -\frac{\ln(1-r)}{\lambda}
$$

where:

$$
0 < r < 1
$$

is a random number.

---

### 2. Number of undecayed nuclei

At time \(t\), a nucleus has not decayed if:

$$
t_i > t
$$

So the simulated number of undecayed nuclei is:

$$
N_{\text{sim}}(t)=\text{number of nuclei with } t_i > t
$$

---

### 3. Analytical solution

The theoretical solution is:

$$
N(t)=N_0e^{-\lambda t}
$$

The Monte Carlo result fluctuates around this curve.

For large \(N_0\), the simulation becomes smoother.

For small \(N_0\), fluctuations become larger.

---

### 4. Half-life

Half-life is the time when:

$$
N(t)=\frac{N_0}{2}
$$

Substitute into the decay formula:

$$
\frac{N_0}{2}=N_0e^{-\lambda t_{1/2}}
$$

Cancel \(N_0\):

$$
\frac{1}{2}=e^{-\lambda t_{1/2}}
$$

Take logarithm:

$$
\ln\left(\frac{1}{2}\right)=-\lambda t_{1/2}
$$

So:

$$
t_{1/2}=\frac{\ln 2}{\lambda}
$$

---

## Conclusion

Radioactive decay is a random process for individual nuclei.

However, for many nuclei, the total number of undecayed nuclei follows:

$$
N(t)=N_0e^{-\lambda t}
$$

The half-life is:

$$
t_{1/2}=\frac{\ln 2}{\lambda}
$$

Monte Carlo simulation shows random fluctuations, especially when \(N_0\) is small.
