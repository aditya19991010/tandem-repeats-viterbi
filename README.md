# tandem-repeats-viterbi
This project simulates dinucleotide tandem repeats (e.g., ATATAT...) in DNA and models how replication or sequencing errors introduce mutations into these repetitive regions. A Hidden Markov Model (HMM) is then used to reconstruct the original repeat sequence using the Viterbi algorithm.


🧪 Objectives
Generate a synthetic tandem repeat sequence (mother sequence).

Introduce mutations simulating real-world errors (corrupted daughter sequence).

Apply the Viterbi algorithm to decode and reconstruct the original sequence.

Evaluate fidelity using Bit Error Rate (BER) or repeat-level accuracy.

🧬 Methodology
Tandem Repeat Generation

Define a base repeat unit (e.g., AT).

Generate a repeat sequence by repeating the unit n times.

Optionally simulate repeat unit transitions.

Mutation Simulation

Introduce substitutions, insertions, or deletions at controlled probabilities.

Create a noisy daughter sequence representing replication errors.

Viterbi Reconstruction

Define an HMM with:

States: Possible repeat units.

Transition/Emission Probabilities: Modeled mutation likelihoods.

Decode the most probable original repeat sequence from the corrupted one.

Evaluation

Compare predicted vs. true sequence.

Calculate Bit Error Rate (BER).

⚙️ Applications
Study of repeat instability in genomic regions.

Modeling errors in replication and sequencing.

Basis for detecting microsatellite instability in disease contexts.
