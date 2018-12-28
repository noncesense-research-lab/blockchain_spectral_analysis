# blockchain_spectral_analysis

Transforming blockchain timestamps into frequency domain to highlight related transactions

## Credit

**Data:** [Neptune Research](https://github.com/neptuneresearch)

**Analysis:** [Isthmus](https://github.com/mitchellptk) & handleTBD

## Monero (XMR) file notes:

Columns are: `id`, `is_alt_block`, `height`, `n_tx_hashes`, `timestamp`, `nrt`

There are two Monero files
-  `XMR_data_from_20181220.csv` contains the entire history of Monero transactions
-  `XMR_last_yearish.csv` contains the most recent 250,000 blocks 

The last-year file was extracted by `tail XMR_data_from_20181220.csv -n 250000 > XMR_last_yearish.csv`

Use `n_tx_hashes` as the signal (y, to be transformed), and test two different time domains (akin to depth):
-  `height` field [caveat: this is not a uniform domain]
-  `timestamp` field [caveat: these can be inaccurate by +/- 400 s]

## Solicitation
Looking for analogous data from transparent blockchains (Ethereum, Bitcoin, etc) so that temporal signals can be checked against ground truth from transaction tree topology.
