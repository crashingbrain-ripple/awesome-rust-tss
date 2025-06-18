# awesome-rust-tss [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
A curated list of distributed key generation and threshold signatures implementations in Rust


## DKG list
* [aggregatable-dkg (Kobi Gurkan)](https://github.com/kobigurk/aggregatable-dkg): Aggregatable DKG and VUF
* [EthDKG (Philipp Schindler)](https://github.com/PhilippSchindler/EthDKG): An Ethereum-based Distributed Key Generation Protocol in python
* [dkg-on-evm (Orbs Network)](https://github.com/orbs-network/dkg-on-evm): DKG for BLS threshold signature scheme on the EVM using solidity
* [gennaro-dkg](https://github.com/mikelodder7/gennaro-dkg) LetProtocol's implementation of Gennaro's distributed key generation
* [vsss-rs](https://github.com/mikelodder7/vsss-rs) Verifiable secret sharing crate that implements Feldman, Pedersen and Shamir secret sharing

## TSS list
* [multi-party-ecdsa (ZenGo X)](https://github.com/ZenGo-X/multi-party-ecdsa): Rust implementation of {t,n}-threshold ECDSA 
* [multi-party-bls (ZenGo X)](https://github.com/ZenGo-X/multi-party-bls): Threshold BLS signatures in Rust
* [celo-threshold-bls-rs (Celo)](https://github.com/celo-org/celo-threshold-bls-rs): celo's Threshold BLS Signatures and DKG in Rust
* [NuBLS (NuCypher)](https://github.com/nucypher/NuBLS): Rust implementation of BLS-based threshold protocols such as threshold encryption and threshold proxy encryption
* [threshold-signatures (ING Bank)](https://github.com/ing-bank/threshold-signatures): Threshold Signature Scheme for ECDSA (Rust)
* [frost-dalek (Isis Lovecruft)](https://github.com/isislovecruft/frost-dalek) A Rust implementation of FROST: Flexible Round-Optimised Schnorr Threshold signatures using the Ristretto group
* [threshold_crypto (PoA network)](https://github.com/poanetwork/threshold_crypto): A Rust pairing-based threshold cryptosystem for collaborative decryption and signatures used in HoneybadgerBFT implementation
* [tofn (Axelar Network)](https://github.com/axelarnetwork/tofn) : A threshold cryptography library in Rust, implementing GG20
* [tss-wasm](https://github.com/0xEigenLabs/tss-wasm): A hardware friendly [multi-party-ecdsa (ZenGo X)](https://github.com/ZenGo-X/multi-party-ecdsa), only implementing GG18.
* [mpecdsa (Jack Doerner)](https://gitlab.com/neucrypt/mpecdsa) : 2-of-n and t-of-n threshold ECDSA implementations (Rust)
* [OpenTSS](https://github.com/LatticeX-Foundation/opentss): Rust implementation of {t,n}-threshold ECDSA using DMZ+21 protocol
* [silent-shard-dkls23-II](https://github.com/silence-laboratories/silent-shard-dkls23-ll): A Rust library for Multi-PArty-TSS ECDSA based on DKLS23
* [dkls23](https://github.com/silence-laboratories/dkls23): Rust implementation of DKLs23 by Silence Laboratories. Includes DKG
* [multi-party-schnorr](https://github.com/silence-laboratories/multi-party-schnorr): A high-performance threshold EdDSA/Schnorr signature library based on Lindell's algorithm
* [cggmp21 (DFNS)](https://github.com/LFDT-Lockness/cggmp21): Rust implementation of CGGMP21 Threshold ECDSA algorithm used by DFNS
* [lit-frost](https://github.com/LIT-Protocol/lit-frost): Implementation of FROST signing protocol (EdDSA) by Lit Protocol
* [synedrion](https://github.com/entropyxyz/synedrion): A threshold signing library based on the CGGMP'24 scheme.

## DKR list
* [Fouque-Stern DKR (ZenGo)](https://github.com/ZenGo-X/fs-dkr)

---

## TSS crates
  
| Repo  | Algorithms | License | BigInt dependency 
|---|---|---|---|
| multi-party-ecdsa | GG18, GG20, CCLST, Lindell  | GPL-3 | curv > GMP/num-bigint |
| multi-party-bls | BLS | GPL-3 | <li>ff-zeroize <li>curv > GMP/num-bigint  |
| openTSS | DMZ+21 | GPL-3 | curv > GMP/num-bigint  |
| silent-shard-dkls23-II | DKLs23 | SLL (Own non-commercial license) | <li>sl-mpc-mate > elliptic-curve > crypto-bigint |
| dkls23 | DKLs23 | SLL (Own non-commercial license) | <li>sl-mpc-mate > elliptic-curve > crypto-bigint |
|multi-party-schnorr| Lindell | SLL | <li>crypto-bigint |
| cggmp21 | CGGMP21 | <li> MIT <li>Apache 2.0 | <li>generic-ec > elliptic-curve > crypto-bigint |
| lit-frost | FROST | Apache 2.0 | <li>frost-ed25519 > curve25519-dalek <li> frost-ed448 > ed448-goldilocks > elliptic-curve > crypto-bigint <li> frost-p256 > p256 >elliptic-curve > crypto-bigint <li> frost-p384 > p384 > elliptic-curve > crypto-bigint <li> ... |
| synedrion | CGGMP24 | AGPL-3 | elliptic-curve > crypto-bigint |