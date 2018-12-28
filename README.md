# blockchain_spectral_analysis

Transforming blockchain timestamps into frequency domain to highlight related transactions

**Data:** Neptune Research

**Analysis:** Isthmus & @handleTBD
---

Notes

Use `n_tx_hashes` as the signal (y, to be transformed), and test two different time domains (akin to depth):
-  `height` field [caveat: this is not a uniform domain]
-  `timestamp` field [caveat: these can be inaccurate by +/- 400 s]

