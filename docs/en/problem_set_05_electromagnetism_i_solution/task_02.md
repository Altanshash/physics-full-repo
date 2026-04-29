# Problem 2 – Coulomb's Force

## Given

Two point charges:

$$
q_1 = 3 \ \mu C = 3 \times 10^{-6} \ C
$$

$$
q_2 = -5 \ \mu C = -5 \times 10^{-6} \ C
$$

Positions:

$$
\vec r_1 = (0,0) \ m
$$

$$
\vec r_2 = (0.4,0.3) \ m
$$

Coulomb constant:

$$
k = 9 \times 10^9 \ \frac{N \cdot m^2}{C^2}
$$

---

## 1. Force vector acting on \( q_2 \)

First, find the distance between the charges:

$$
\vec r = \vec r_2 - \vec r_1
$$

$$
\vec r = (0.4,0.3) - (0,0)
$$

$$
\vec r = (0.4,0.3) \ m
$$

Magnitude of distance:

$$
r = \sqrt{(0.4)^2 + (0.3)^2}
$$

$$
r = \sqrt{0.16 + 0.09}
$$

$$
r = \sqrt{0.25}
$$

$$
r = 0.5 \ m
$$

Unit vector from \(q_1\) to \(q_2\):

$$
\hat r = \frac{\vec r}{r}
$$

$$
\hat r = \frac{(0.4,0.3)}{0.5}
$$

$$
\hat r = (0.8,0.6)
$$

Because \(q_1\) is positive and \(q_2\) is negative, the force is attractive.  
So the force on \(q_2\) is directed toward \(q_1\).

Magnitude of the force:

$$
F = k \frac{|q_1q_2|}{r^2}
$$

$$
F = (9 \times 10^9)
\frac{(3 \times 10^{-6})(5 \times 10^{-6})}{(0.5)^2}
$$

$$
F = (9 \times 10^9)
\frac{15 \times 10^{-12}}{0.25}
$$

$$
F = 0.54 \ N
$$

Force vector on \(q_2\):

$$
\vec F_2 = -F \hat r
$$

$$
\vec F_2 = -0.54(0.8,0.6)
$$

$$
\vec F_2 = (-0.432,-0.324) \ N
$$

$$
\boxed{\vec F_2 = (-0.432,-0.324) \ N}
$$

---

## 2. Magnitude of the force

$$
|\vec F_2| = \sqrt{(-0.432)^2 + (-0.324)^2}
$$

$$
|\vec F_2| = \sqrt{0.186624 + 0.104976}
$$

$$
|\vec F_2| = \sqrt{0.2916}
$$

$$
|\vec F_2| = 0.54 \ N
$$

$$
\boxed{|\vec F_2| = 0.54 \ N}
$$

---

## 3. Potential energy of the system

The electric potential energy is:

$$
U = k \frac{q_1q_2}{r}
$$

Substitute the values:

$$
U = (9 \times 10^9)
\frac{(3 \times 10^{-6})(-5 \times 10^{-6})}{0.5}
$$

$$
U = (9 \times 10^9)
\frac{-15 \times 10^{-12}}{0.5}
$$

$$
U = -0.27 \ J
$$

$$
\boxed{U = -0.27 \ J}
$$

The negative sign means the charges attract each other.

---

## 4. Work required to separate the charges to \(2 \ m\)

Initial distance:

$$
r_i = 0.5 \ m
$$

Final distance:

$$
r_f = 2 \ m
$$

Initial potential energy:

$$
U_i = -0.27 \ J
$$

Final potential energy:

$$
U_f = k \frac{q_1q_2}{r_f}
$$

$$
U_f = (9 \times 10^9)
\frac{(3 \times 10^{-6})(-5 \times 10^{-6})}{2}
$$

$$
U_f = -0.0675 \ J
$$

Work required:

$$
W = U_f - U_i
$$

$$
W = -0.0675 - (-0.27)
$$

$$
W = 0.2025 \ J
$$

$$
\boxed{W = 0.2025 \ J}
$$

---

## Final Answer

$$
\boxed{\vec F_2 = (-0.432,-0.324) \ N}
$$

$$
\boxed{|\vec F_2| = 0.54 \ N}
$$

$$
\boxed{U = -0.27 \ J}
$$

$$
\boxed{W = 0.2025 \ J}
$$

---

## Conclusion

The charges have opposite signs, so they attract each other.  
The force on \(q_2\) is directed toward \(q_1\).  
The potential energy is negative because the system is attractive.  
Positive work is needed to separate the charges from \(0.5 \ m\) to \(2 \ m\).
