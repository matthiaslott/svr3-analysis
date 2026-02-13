# TOPRF Experimentation

Explores modelling SVR3's TOPRF using a new extension supporting the multiplication of Diffie-Hellman terms.

## Directory Structure

```
.
├── toprf
│   ├── toprf.spthy                # TOPRF model using the new extension
│   │
│   └── executability-proof.spthy  # Proof of the executability lemma
│
└── toprf-minimisation
    ├── toprf.spthy                # Minimised version of the TOPRF theory using the existing DH extension
    │                              # demonstrating the proof cycle that occurs in the secrecy lemma
    │
    └── proof-cycle.spthy          # Demonstration of the proof cycle.
```