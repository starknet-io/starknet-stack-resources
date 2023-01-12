# starknet-stack-resources

A collection of works discussing the major components inside StarkNet

## The STARK Protocol

Under the Math folder you can find papers related to the STARK protocol. We can devide these into two categories:

FRI - the low degree testing protocol used in STARK
* [Fast Reed-Solomon Interactive Oracle Proofs of Proximity](./Math/FRI/Fast%20Reed-Solomon%20Interactive%20Oracle%20Proofs%20of%20Proximity.pdf); the original paper introducing FRI
* [DEEP-FRI- Sampling Outside the Box Improves Soundness](./Math/FRI/DEEP-FRI-%20Sampling%20Outside%20the%20Box%20Improves%20Soundness.pdf); this paper introduces a variant of FRI which provides better soundness gurantees
* [Proximity Gaps for Reed–Solomon Codes](./Math/FRI/Proximity%20Gaps%20for%20Reed–Solomon%20Codes.pdf); this paper gives the state of the art soundness bounds for the soundness of FRI (see section 8.2)

STARK
* [Scalable, transparent, and post-quantum secure computational integrity](./Math/STARK/Scalable%2C%20transparent%2C%20and%20post-quantum%20secure%20computational%20integrity.pdf); the original paper introducing the STARK protocol
* [ethSTARK](./Math/STARK/ethSTARK.pdf); describes a specific construction of STARK, simillar to what is used in production (to follow closely our production system, see the STARK verifier audit by CryptoExperts)

### Audits

Under the Audits folder you can find:

* [An audit](./Audits/EVM_STARK_Verifier_v4.0_Audit_Report.pdf) for StarkWare's solidity STARK verifier
* [An audit](./Audits/Cairo%20&%20SHARP%20Verifiers.pdf) for StarkWare's solidity Cairo and the SHARP verifiers
* [An audit](./Audits/STARK_Cairo%20Verifiers%20(in%20Cairo)%20Audit%20Report.pdf) for StarkWare's Cairo STARK/Cairo verifiers (these are used in recursive proofs)

## Cairo

Under the Cairo folder you can find the following two papers:

* [Cairo – a Turing-complete STARK-friendly CPU architecture](./Cairo/Cairo%20–%20a%20Turing-complete%20STARK-friendly%20CPU%20architecture.pdf); the paper introducing the Cairo CPU architecture
* [A Verified Algebraic Representation of Cairo Program Execution](./Cairo/A%20Verified%20Algebraic%20Representation%20of%20Cairo%20Program%20Execution.pdf); this paper proves the correctness of the polynomial constraints ecncoding of the Cairo VM via the Lean proof assistant. For the exact formalization of the Cairo semantics that was used, see our [formal proofs](https://github.com/starkware-libs/formal-proofs) repo.

## Bug Bounty

A successful audit doesn't gurantee that the underlying code is free of bugs. For that purpose, we started a [bug bounty](https://immunefi.com/bounty/starknet/) program for StarkNet. Currently, the bounty program focuses on the StarkNet OS and related L1 contracts that define the protocol. In the future it may be extended to cover some of the mathematical foundations described above. You're welcome to report issues in our [discord](https://discord.gg/qypnmzkhbc).

## License

This project is licensed under the **Apache 2.0**.

See [LICENSE](LICENSE) for more information.
