# tandem-repeats-viterbi
This project simulates dinucleotide tandem repeats (e.g., ATATAT...) in DNA and models how replication or sequencing errors introduce mutations into these repetitive regions. A Hidden Markov Model (HMM) is then used to reconstruct the original repeat sequence using the Viterbi algorithm.

---

## 📚 Project Overview

1. **Generate a tandem repeat sequence** (e.g., `AT` repeated `n` times).
2. **Simulate mutations** (substitutions, indels) to form a corrupted daughter sequence.
3. **Use Viterbi algorithm** to reconstruct the most probable original sequence.
4. **Evaluate reconstruction accuracy** using Bit Error Rate (BER).

---

## 🧪 Objectives
1. Generate a synthetic tandem repeat sequence (mother sequence).
2. Introduce mutations simulating real-world errors (corrupted daughter sequence).
3. Apply the Viterbi algorithm to decode and reconstruct the original sequence.
4. Evaluate fidelity using Bit Error Rate (BER) or repeat-level accuracy.

## 🧬 Methodology
1. Tandem Repeat Generation
   - Define a base repeat unit (e.g., AT).
   - Generate a repeat sequence by repeating the unit n times.
   - Simulate repeat unit transitions.
2. Mutation Simulation
 - Introduce substitutions, insertions, or deletions at controlled probabilities.
 - Create a noisy daughter sequence representing replication errors.
Viterbi Reconstruction

3. Define an HMM with:
- States: Possible repeat units.
- Transition/Emission Probabilities: Modeled mutation likelihoods.
- Decode the most probable original repeat sequence from the corrupted one.

4. Evaluation
 - Compare predicted vs. true sequence.
 - Calculate Bit Error Rate (BER).

## ⚙️ Applications
1. Study of repeat instability in genomic regions.
2. Modeling errors in replication and sequencing.
3. Basis for detecting microsatellite instability in disease contexts.
