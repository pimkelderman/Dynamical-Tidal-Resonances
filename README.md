# Dynamical-Tidal-Resonances

The data in [filename] contain lists {{"n", "k", "m", "s"}, {"a", "p", "e", "x", "b"}, {"dE", "dL", "dQ"}} for one resonance (n,k,m,s) over a parameter space in (a,e,x) with a grid of 20x20x10, prograde and retrograde separately. (and later for several b values)

"\[Epsilon]\[CapitalEpsilon]q=1, \[Epsilon]B=1, \  \[Epsilon]\[CapitalEpsilon]o=0" This just means that it used only the **quadropole** electric and magnetic tidal moments. (and not yet higher multipole order or PN order)

In the static case, we set m2 = 1 and b = 1, meaning that you still have to mulitply the data by m2/b^3. (where m2 is mass of the perturber, and b is distance to the perturber, all in geometrized units)

For this data it works kind of similar: - When a resonance has k+m = even,   multiply by m2/b^3. 
                                        - When instead it has k+m = odd,     multiply by m2/b^3 * \Sqrt[ (1+m2)/b ]  


