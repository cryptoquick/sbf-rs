# Spatial Bloom Filter
[![pipeline status](https://gitlab.com/cryptoquick/sbf-rs/badges/master/pipeline.svg)](https://gitlab.com/cryptoquick/sbf-rs/commits/master)
[![coverage report](https://gitlab.com/cryptoquick/sbf-rs/badges/master/coverage.svg)](https://gitlab.com/cryptoquick/sbf-rs/commits/master)
[![Crate](https://img.shields.io/crates/v/sbf.svg)](https://crates.io/crates/sbf)
[![API](https://docs.rs/sbf/badge.svg)](https://docs.rs/sbf)

SBF is a probabilistic data structure
that maps elements of a space to indexed disjoint subsets of that space.

This is a reimplementation of the [C library](https://github.com/spatialbloomfilter/libSBF-cpp) by the original research group.

This repository is forked from [GitLab](https://gitlab.com/bertof/sbf-rs) and [Github](https://github.com/bertof/sbf-rs)

## Crate features

This crate allows the following features:

- `md4_hash` Allows to use a md4 based hashing algorithm;
- `md5_hash` Allows to use a md5 based hashing algorithm;
- `blake3_hash` Allows to use a [Blake3](https://github.com/BLAKE3-team/BLAKE3) based hashing algorithm;
- `serial` Enables `serde` integration;
- `metrics` Generates and updates an internal metrics object, useful in simulations and benchmarks of the library.

By default only `md5_hash` is enabled.
