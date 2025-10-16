# Ztarknet 🛡️🐺

**Ztarknet 🛡️🐺** proposes a Starknet-style L2 that executes **Cairo** programs, proves the resulting state transitions with [**Circle STARKs**](https://eprint.iacr.org/2024/278) ([Stwo](https://github.com/starkware-libs/stwo-cairo)), and **settles** those transitions on **Zcash L1** by having full nodes verify the proof natively via a TZE verifier. It reuses an existing Starknet client (e.g., **Madara**) for sequencing/execution and a **Stwo/Cairo** prover for proofs. The L1 verification surface is a **single TZE type** defined by a draft ZIP.

**Why Zcash?** Zcash already offers strong base-layer privacy. Ztarknet explores **programmability and scale** via an L2—with validity proofs checked natively on Zcash using the TZE framework ([ZIP-222](https://zips.z.cash/zip-0222)) and the associated digest changes (ZIP-245/244).
