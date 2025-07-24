# Formal Analysis of the SVR3 Client Protocol

This repository contains a formalisation of the SVR3 protocol in Tamarin.

## Information

Proof generation is not entirely automated. Hence, the full proofs are provided in file [proof.spthy](proof/proof.spthy). They may be verified using the command below. Please plan for around 35 GB RAM usage and 3h of verification time.

```bash
tamarin-prover proof/proof.spthy
```

## Repository Structure

```
.
├── model
│   ├── src/         # Parts of the theory describing brute-force attacks,
│   │                # secure channel, signatures and TOPRF
│   │
│   ├── svr3.spthy   # Main Tamarin theory file containing protocol rules
│   │
│   └── tactics      # Heuristics for guiding parts of the proofs
│
└── proof
    └── proof.spthy  # Proofs for the SVR3 protocol
```