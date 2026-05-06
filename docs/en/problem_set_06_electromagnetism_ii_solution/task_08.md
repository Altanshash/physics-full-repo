# Problem 8 – Self-Induction

## Problem Statement

An RL circuit contains a coil with inductance $L$ and resistance $R$.  
It is powered by a DC voltage source $U$.

After a long time, the circuit is in steady state. Then at time $t = 0$, the power supply is disconnected, and the $L-R$ circuit remains without a source.

For the data:

$$
L = 0.20\ \text{H}
$$

$$
R = 5.0\ \Omega
$$

$$
U = 12\ \text{V}
$$

Answer the following questions:

1. Determine the steady current $I_0$ before disconnecting the power supply.
2. After disconnection, derive $I(t)$, the time constant $\tau$, and the voltage across the coil $U_L(t)$.
3. Calculate the energy stored in the magnetic field of the coil right before disconnection:

$$
W = \frac{1}{2}LI_0^2
$$

4. Show that this energy is converted into Joule heat in the resistor:

$$
\int_0^\infty I^2R\,dt
$$

5. Briefly explain why overvoltage appears when disconnecting the current.

---

## Given

$$
L = 0.20\ \text{H}
$$

$$
R = 5.0\ \Omega
$$

$$
U = 12\ \text{V}
$$

---

## Solution

## 1. Steady Current Before Disconnection

In steady state with a DC source, the inductor behaves like a short circuit.

Therefore, the current is determined only by Ohm's law:

$$
I_0 = \frac{U}{R}
$$

Substitute the values:

$$
I_0 = \frac{12}{5.0}
$$

$$
I_0 = 2.4\ \text{A}
$$

---

## 2. Current After Disconnection

After the power supply is disconnected, the current decreases with time.

The equation for the RL circuit is:

$$
L\frac{dI}{dt} + RI = 0
$$

Rearrange:

$$
\frac{dI}{dt} = -\frac{R}{L}I
$$

The solution is:

$$
I(t) = I_0 e^{-\frac{R}{L}t}
$$

The time constant is:

$$
\tau = \frac{L}{R}
$$

Substitute the values:

$$
\tau = \frac{0.20}{5.0}
$$

$$
\tau = 0.040\ \text{s}
$$

So:

$$
I(t) = 2.4e^{-\frac{t}{0.040}}
$$

or:

$$
I(t) = 2.4e^{-25t}
$$

---

## 3. Voltage Across the Coil

The voltage across the inductor is:

$$
U_L(t) = L\frac{dI}{dt}
$$

Since:

$$
I(t) = I_0 e^{-\frac{t}{\tau}}
$$

then:

$$
\frac{dI}{dt} = -\frac{I_0}{\tau}e^{-\frac{t}{\tau}}
$$

Therefore:

$$
U_L(t) = -L\frac{I_0}{\tau}e^{-\frac{t}{\tau}}
$$

Because:

$$
\tau = \frac{L}{R}
$$

we get:

$$
U_L(t) = -RI_0 e^{-\frac{t}{\tau}}
$$

Substitute:

$$
RI_0 = 5.0 \cdot 2.4 = 12
$$

Thus:

$$
U_L(t) = -12e^{-\frac{t}{0.040}}\ \text{V}
$$

or:

$$
U_L(t) = -12e^{-25t}\ \text{V}
$$

The negative sign means that the coil opposes the decrease of current.

---

## 4. Energy Stored in the Magnetic Field

The energy stored in the magnetic field is:

$$
W = \frac{1}{2}LI_0^2
$$

Substitute:

$$
W = \frac{1}{2} \cdot 0.20 \cdot (2.4)^2
$$

$$
W = 0.10 \cdot 5.76
$$

$$
W = 0.576\ \text{J}
$$

---

## 5. Joule Heat in the Resistor

The current after disconnection is:

$$
I(t) = I_0 e^{-\frac{t}{\tau}}
$$

The Joule heat is:

$$
Q = \int_0^\infty I^2R\,dt
$$

Substitute $I(t)$:

$$
Q = \int_0^\infty I_0^2 e^{-\frac{2t}{\tau}}R\,dt
$$

Since $I_0^2R$ is constant:

$$
Q = I_0^2R \int_0^\infty e^{-\frac{2t}{\tau}}dt
$$

The integral is:

$$
\int_0^\infty e^{-\frac{2t}{\tau}}dt = \frac{\tau}{2}
$$

So:

$$
Q = I_0^2R \cdot \frac{\tau}{2}
$$

Since:

$$
\tau = \frac{L}{R}
$$

then:

$$
Q = I_0^2R \cdot \frac{L}{2R}
$$

$$
Q = \frac{1}{2}LI_0^2
$$

Therefore:

$$
Q = W
$$

Substitute the value:

$$
Q = 0.576\ \text{J}
$$

So, all magnetic field energy is converted into Joule heat.

---

## 6. Why Overvoltage Appears During Disconnection

The inductor resists sudden changes in current.

The induced voltage is:

$$
U_L = -L\frac{dI}{dt}
$$

If the circuit is disconnected very quickly, then $\frac{dI}{dt}$ becomes very large.

As a result, the induced voltage can become very large.

This is why overvoltage or a spark can appear when disconnecting the current.

---

## Final Conclusion

The steady current before disconnection is:

$$
I_0 = 2.4\ \text{A}
$$

The time constant is:

$$
\tau = 0.040\ \text{s}
$$

The current after disconnection is:

$$
I(t) = 2.4e^{-25t}\ \text{A}
$$

The voltage across the coil is:

$$
U_L(t) = -12e^{-25t}\ \text{V}
$$

The stored magnetic energy is:

$$
W = 0.576\ \text{J}
$$

This energy is converted into Joule heat:

$$
Q = \int_0^\infty I^2R\,dt = 0.576\ \text{J}
$$

Overvoltage appears because the inductor tries to keep the current from changing suddenly.
