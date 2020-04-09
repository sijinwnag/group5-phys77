# group5-phys77
# Quantum mechanics numerical method
import numpy as np

# define some constants
# hb refers to the reduced planks constant
hb = 6.626e-34/np.pi/2

# the following functions are the wave functions and energy levels
# of 1D infinite squre well from google


# the following function defines the energy level
# a is the length of infinite square well (suppose x=0 to a)
# m is the mass of the particle
# n is the energy level index
# for example
# n=1 means the energy level is the lowest energy level
# n=2 means the energy level is the second lowest energy
# and so on
def E(a, m, n):
    E = n**2*np.pi**2*hb**2/2/m/a**2
    return E


# the following function defines the wave equation (time independent)
def psi(a, n, x):
    psi = np.sqrt(2/a)*np.sin(n*np.pi*x/a)
    return psi

# the next step is to plot the wave function and energy level
