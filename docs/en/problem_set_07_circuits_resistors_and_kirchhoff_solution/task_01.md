# Problem 1 — Equivalent Resistance

Calculate the equivalent resistance for the circuit shown in the figure.  
All resistors have resistance:

\[
R = 5\ \Omega
\]

---

# Step 1 — Analyze the Top Branch

The top branch contains **two resistors in series**.

For series connection:

:contentReference[oaicite:0]{index=0}

So,

\[
R_{\text{top}} = 5 + 5
\]

\[
R_{\text{top}} = 10\ \Omega
\]

---

# Step 2 — Analyze the Bottom Branch

On the bottom branch:

- the first resistor is \(5\ \Omega\)
- the two resistors on the right are connected in parallel

For parallel connection:

:contentReference[oaicite:1]{index=1}

Substitute the values:

\[
R_p = \frac{5 \times 5}{5 + 5}
\]

\[
R_p = \frac{25}{10}
\]

\[
R_p = 2.5\ \Omega
\]

Now add the series resistor:

\[
R_{\text{bottom}} = 5 + 2.5
\]

\[
R_{\text{bottom}} = 7.5\ \Omega
\]

---

# Step 3 — Combine the Two Main Branches

Now the circuit has:

- top branch: \(10\ \Omega\)
- bottom branch: \(7.5\ \Omega\)

These two branches are connected in parallel.

Using the parallel formula:

\[
R_{\text{main}} =
\frac{10 \times 7.5}{10 + 7.5}
\]

\[
R_{\text{main}} =
\frac{75}{17.5}
\]

\[
R_{\text{main}} =
4.2857\ \Omega
\]

---

# Step 4 — Add the Final Series Resistor

There is one more resistor of \(5\ \Omega\) in series on the right side.

So,

\[
R_{\text{eq}} = 4.2857 + 5
\]

\[
R_{\text{eq}} = 9.2857\ \Omega
\]

---

# Final Answer

\[
\boxed{R_{\text{eq}} \approx 9.29\ \Omega}
\]
