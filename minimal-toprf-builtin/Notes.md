# Diffie-Hellman with Multiplication Extension

1. Use `DH-multiplication` builtin instead of `diffie-hellman`
2. Sorts are expressed using a capital letter in front of the variable/constant, e.g. Fexp for a fresh non-zero exponent:
   1. G: group element
   2. E: exponent
   3. N: Non-zero exponent
   4. F: fresh Non-zero exponent
   5. P: public group element
3. `FrDH(...)` fact instead of `Fr(...)`
4. `dhExp(G, E)` instead of `G^E`
5. `dhMult(G, G)` instead of `G*G`
6. Don't use regular `G` variables. Pattern-match them as `dhExp(g, E)` for some `P'g'` (public group element) that is always the same.
7. Also use the variable naming inside lemmas