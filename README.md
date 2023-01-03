# starknet-security-materials

A collection of works discussing the security aspects of StarkNet

## Audits

Under the Audits folder you can find:

* An audit for StarkWare's solidity STARK verifier
* An audit for StarkWare's solidity Cairo and the SHARP verifiers
* An audit for StarkWare's Cairo STARK/Cairo verifiers (these are used in recursive proofs)

## Math

Under the Math folder you can find papers related to the STARK protocol. We can devide these into two categories:

FRI - the low degree testing protocol used in STARK
* Fast Reed-Solomon Interactive Oracle Proofs of Proximity; the original paper introducing FRI
* DEEP-FRI- Sampling Outside the Box Improves Soundness; this paper introduces a variant of FRI which provides better soundness gurantees
* Proximity Gaps for Reed–Solomon Codes; this paper gives the state of the art soundness bounds for the soundness of FRI (see section 8.2)

STARK
* Scalable, transparent, and post-quantum secure computational
integrity; the original paper introducing the STARK protocol
* ethSTARK; describes a specific construction of STARK, simillar to what is used in production (to follow closely our production system, see the STARK verifier audit by CryptoExperts).

## Cairo

Under the Cairo folder you can find the following two papers:

* Cairo – a Turing-complete STARK-friendly CPU architecture; the paper introducing the Cairo CPU architecture
* A Verified Algebraic Representation of Cairo Program Execution; this paper proves the correctness of the polynomial constraints ecncoding of the Cairo VM via the Lean proof assistent. For the exact formalization of the Cairo semantics that was used, see our [formal proofs](https://github.com/starkware-libs/formal-proofs) repo.
