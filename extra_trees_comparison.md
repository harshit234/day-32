### Extra Trees vs. Random Forest Comparison

**A) Splitting Mechanism:**
- **Random Forest**: Searches for the *optimal* split threshold for a random subset of features at each node.
- **Extra Trees**: Chooses a *random* threshold for each feature in the subset and then selects the best among those random thresholds. This significantly increases randomness and reduces variance.

**B) Speed Comparison:**
- Extra Trees is typically **faster** because it skips the computationally expensive search for the best discriminative threshold for every feature candidate.

**C) Performance Comparison:**
- Based on our loan dataset, both models show strong performance. Extra Trees often provides better generalization when the data is noisy, though it might have a slightly higher bias than Random Forest.
