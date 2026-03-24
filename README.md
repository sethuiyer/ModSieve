# ModSieve

A number-theoretic pre-filter for NP-hard optimization problems. Proves subset sum impossibility via modular arithmetic without exhaustive search.

## Overview

ModSieve applies modular arithmetic as a pre-filter to prove impossibility in subset sum instances. For structured inputs, this can eliminate impossible targets in O(n·p) time — linear in the input size — rather than exponential search.

## Theory

For a prime p and set W, the reachable residues W/p = { Σw mod p | w' ⊆ W } are computed via dynamic programming. If t mod p ∉ W/p, then no subset of W sums to t.

See the [full mathematical foundations](./index.html) for details.

## Usage

Open `index.html` in a browser. The page contains two tabs:

- **Mathematics** — Theoretical foundations and proof structure
- **Algorithm & Code** — Implementation details and Python code

## References

- Tao & Vu, *Additive Combinatorics*
- Cormen et al., *Introduction to Algorithms*

## License

MIT
