# No.58: Exact Outer Multiset Dimension of the Three-Dimensional Grid Family P₂ □ P₃ □ Pₙ

Ryutaro Yonezu — Independent Researcher. Preprint v1.0, 2026-11-07.

[Zenodo Preprint](https://zenodo.org/records/24024946) · [DOI: 10.5281/zenodo.24024946](https://doi.org/10.5281/zenodo.24024946) · [GitHub Release v1.0](https://github.com/yonezaemon1-hub/no58-outer-multiset-dimension-3d-grid/releases/tag/v1.0)

[Paper PDF](No58_v1.0_PREPRINT_20261107.pdf) · [Reproducibility ZIP](No58_v1.0_REPRODUCIBILITY_20261107.zip) · [SHA256](SHA256SUMS.txt)

For every integer **n ≥ 6**, **odim(P₂ □ P₃ □ Pₙ) = 4**. A landmark set distinguishes every pair of distinct vertices **outside** the set using **unordered distance multisets**, retaining multiplicities. The claim covers this three-path family only.

Computer-assisted proof. Independent AI review is user-supplied and scope-limited: the latest publication instruction reports v0.5 MODEL / PROOF / COMPUTATION PASS. Earlier collision-witness rederivation was PARTIAL; complete independent formalization and third-party rederivation of every branch are not claimed. **Not human peer-reviewed. NOVELTY INCONCLUSIVE. REFERENCES PARTIAL. All rights reserved.**

Windows PowerShell 5.1 reproduction is supported by user-supplied PASS records for frozen v0.3/Audit D and the v0.5 difference checks (24/24 branches, 268,528 configurations). Private transcripts are excluded; see `WINDOWS_REPRODUCTION_SUMMARY.txt`. This does not claim a new independent Windows execution of the v1.0 runner.

## Proof and finite evidence

- Lemma 0 excludes every set of size at most two by a unit-cube sign argument.
- Collision lifting reduces triples with fewer than two corners to n = 2,…,35. The exhaustive certificate rejects 13,921,300 triples.
- An exact ordinal calculation splits 336 types into 272 with a local obstruction and 64 survivors, covered by A/B/C and E0,…,E4 under reflections.
- Twenty-four affine branches, including even-N B(N) branch 24, give distinct exterior collision vertices. Symbolic inverse slack formulas give all-parameter coverage. The 268,528-case scan is corroboration, not extrapolation.
- Explicit upper constructions cover odd n ≥ 7, even n ≥ 10, and n = 6,8. Original distance-sum and separate exact rational permutation certificates are included.

## Public files

The fixed paper PDF and reproducibility ZIP are in this repository and its v1.0 Release. Download and extract the ZIP to run the certificates. The contents and paths below refer to that extracted distribution. A standalone TeX source and SHA256 list are also provided.

## Run the main certificates

Requirements: Python 3.10 or newer, its standard library, and g++ or clang++ with C++17 support. No paid API, cloud computation, solver, or third-party Python package is required.

From the extracted directory, run:

```text
python reproduce.py
```

On Unix, `python3 reproduce.py` is also suitable. On Windows, `py -3 reproduce.py` can select Python. A C++17 compiler must be on PATH. Do not use Python `-O`: assertions in frozen certificates must remain enabled. The runner verifies hashes and file inventory before computation and writes generated intermediates only into a temporary working directory.

For manual execution, compile `frozen_v03/No58_lower_corner_lemma_v03.cpp` with C++17 and run it. Run the five Python programs listed in `reproduce.py` without modifying their bytes. A standalone v0.5 arithmetic run creates a certificate JSON in its current working directory; run it in a temporary directory to preserve the distribution inventory.

## Contents and chronology

`source/` contains the complete v1.0 TeX manuscript. `frozen_v03/`, `auditD_frozen/`, and `v05/` preserve supplied files byte for byte. `provenance/` contains the original full and review ZIPs and their identifying hashes. `validation/` records environment-independent output of six release-preparation executions. `REVIEW_SCOPE.md` records evidence boundaries and literature checks. `SHA256SUMS_REPRO.txt` covers every other file in this ZIP.

Historical HOLD / audit-pending statements inside frozen files describe those earlier stages and remain unchanged for provenance. The researcher explicitly authorized v1.0 publication on 2026-11-07 with the limitations above. Author-side Audits A/B/C/D are not reclassified as independent external reviews. No missing reviewer transcript has been reconstructed.

## Literature boundary

The outer multiset parameter is prior art (Gil-Pons et al., 2019). Klavžar–Kuziak–Yero (2023) determine the two-path case. Mora et al. (2022) study ordered metric resolution, Marcelo et al. (2025) ordinary multiset dimension on cylinders, Peng (2026) two-cycle tori, and Araujo-Pardo et al. (2026) general bounds/circulants. The supplied Farhan et al. survey (2026), Problem 10, motivates products of more than two paths. This result is a candidate partial response for one special infinite family. It makes no priority guarantee or claim to solve the entire problem. Some full texts and the latest citation graph remain unchecked; the survey and Peng arXiv records could not be independently fetched during publication preparation. Full references and exact access limits are in the manuscript and `REVIEW_SCOPE.md`.

Copyright © 2026 Ryutaro Yonezu. **All rights reserved.** Public availability is not a grant of an open-source or Creative Commons license.
