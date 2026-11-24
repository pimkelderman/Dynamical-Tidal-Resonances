# Dynamical-Tidal-Resonances

The data in [filename] contain lists {{"n", "k", "m", "s"}, {"a", "p", "e", "x", "Omega_td", "b"}, {"dE", "dL", "dQ"}} for one resonance (n,k,m,s) over a parameter space in (a,e,x) with a grid of 20x20x10 for 11 Omega_td values (based on b values in folder name, see below), prograde and retrograde separately.

"\[Epsilon]\[CapitalEpsilon]q=1, \[Epsilon]B=1, \  \[Epsilon]\[CapitalEpsilon]o=0" This just means that it used only the **quadropole** electric and magnetic tidal moments. (and not yet higher multipole order or PN order)

IMPORTANT: The data depends on the value of Omega_td (perturber frequency in BL time), that is calculated via Sqrt[1/b^3]. When introducing a mass m2 for the perturber, Omega_td = Sqrt[(1+m2)/b^3]. Calculate the needed Omega_td and then fetch from the data with that Omega_td (in this case, the actual b value will be slightly different than in the data. Omega_td is the leading value.)

In the static case, we set m2 = 1  and b = 1 (both for the scaling that CAN be taken out, these are not used in Omega_td), meaning that you still have to mulitply the data by m2/b^3. (where m2 is mass of the perturber, and b is distance to the perturber, all in geometrized units)

For this data it works kind of similar: - When a resonance has k+m = even,   multiply by m2/b^3. 
                                        - When instead it has k+m = odd,     multiply by m2/b^3 * \Sqrt[ (1+m2)/b ]  


