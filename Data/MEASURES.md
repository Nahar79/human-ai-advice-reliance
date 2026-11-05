# Measures and denominators

| Output | Definition | Eligible observations |
|---|---|---|
| Pre accuracy | Initial signed response > 0 | Nonzero initial, final and advice values |
| Post accuracy | Final signed response > 0 | Same retained trials as pre accuracy |
| Accuracy change | Post correctness minus pre correctness | Same retained trials; paired within participant |
| Beneficial switch | Final label equals advice label | Initial disagreement; advice correct |
| Harmful switch | Final label equals advice label | Initial disagreement; advice incorrect |
| Initial strength | Absolute initial signed response | Range 0–1; not a probability |

Each estimate is an equal-weight mean of eligible participant rates. A participant is excluded from a specific conditional rate only when they have zero eligible trials for it. All table rows carry denominators. Source signs are already aligned to ground truth: sign > 0 means correct for both responses and advice. Zero means undecided and is excluded from primary categorical metrics. It is not classified as wrong or as a refusal to follow advice. Raw data are never altered.

A switch is a change of binary label; changes in slider magnitude without changing label do not count. Final agreement when the participant already agreed initially is not counted as advice uptake. These definitions avoid equating all agreement with reliance. They still do not establish the psychological cause of a decision change.
