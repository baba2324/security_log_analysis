Research Note

Trial: Used a Random Forest classifier as a baseline model due to its robustness on structured tabular data and interpretability via feature importance.

Observation: The model performs well on structured benchmark logs (NSL-KDD). However, its effectiveness on real-world security logs may degrade due to noise, temporal dependencies, and evolving attack patterns.

Next Step: Evaluate sequence-aware models such as LSTM to capture temporal patterns in log sequences and compare performance against the Random Forest baseline.
