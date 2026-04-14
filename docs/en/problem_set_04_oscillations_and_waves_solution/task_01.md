import numpy as np

# Problem 1 – Harmonic Motion
# x(t) = A cos(ωt + φ)

print("=== Problem 1 ===")

# Given
A = 0.2   # meters
f = 2     # Hz

# 1. Period and angular frequency
T = 1 / f
omega = 2 * np.pi * f

print("Period T =", T, "s")
print("Angular frequency ω =", omega, "rad/s")

# 2. Maximum velocity and acceleration
v_max = A * omega
a_max = A * omega**2

print("Max velocity v_max =", v_max, "m/s")
print("Max acceleration a_max =", a_max, "m/s^2")
