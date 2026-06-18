# Concept Collection

Small, self-contained projects: interactive demos, teaching material, and
research code. Most run in the browser with no install, built around
[numbl](https://numbl.org) (MATLAB in the browser), scientific-data tooling, and
mathematical visualization.

Each entry links to its source repository and, where available, a live page.

## Run-in-browser MATLAB (numbl)

MATLAB-syntax projects that run in the browser via [numbl](https://numbl.org).

- **[numbl-quantum-optics](https://github.com/concept-collection/numbl-quantum-optics)**
  ([live](https://concept-collection.github.io/numbl-quantum-optics/)).
  Companion to the article "Quantum optics in MATLAB"
  ([arXiv:2309.14354](https://arxiv.org/abs/2309.14354)): quantum states,
  operators, and dynamics as runnable scripts.
- **[numbl-open-quantum-systems](https://github.com/concept-collection/numbl-open-quantum-systems)**
  ([live](https://concept-collection.github.io/numbl-open-quantum-systems/)).
  Companion to "Coding closed and open quantum systems in MATLAB"
  ([arXiv:1911.04906](https://arxiv.org/abs/1911.04906)): Ising dynamics,
  cavity-QED phase transitions, Lindblad and non-Markovian dynamics.
- **[numbl-distmesh](https://github.com/concept-collection/numbl-distmesh)**
  ([live](https://concept-collection.github.io/numbl-distmesh/)).
  Companion to Persson and Strang's
  [DistMesh](https://github.com/popersson/DistMesh): every README example,
  meshing 2-D regions and surfaces from signed distance functions.
- **[numbl-surfacefun-intro](https://github.com/concept-collection/numbl-surfacefun-intro)**
  ([live](https://concept-collection.github.io/numbl-surfacefun-intro/)).
  An introduction to [surfacefun](https://github.com/danfortunato/surfacefun):
  computing with functions on surfaces and solving PDEs on them to high order.
- **[surfacefun-interactive](https://github.com/concept-collection/surfacefun-interactive)**
  ([live](https://concept-collection.github.io/surfacefun-interactive/)).
  surfacefun demos with live sliders (React and three.js driving a numbl
  script): refine a cubed-sphere mesh, scale a tangent vector field.
- **[numbl-chunkie](https://github.com/concept-collection/numbl-chunkie)**
  ([live](https://concept-collection.github.io/numbl-chunkie/)).
  Examples for [chunkie](https://github.com/fastalgorithms/chunkie): boundary
  integral equations in 2-D, building chunker geometries and solving Laplace,
  Helmholtz, and Stokes problems.
- **[numbl-image-filter](https://github.com/concept-collection/numbl-image-filter)**
  ([live](https://concept-collection.github.io/numbl-image-filter/)).
  Filter an image with a numbl/MATLAB script in the browser. Upload your own
  image and write the filter.
- **[numbl-project-example](https://github.com/concept-collection/numbl-project-example)**
  ([live](https://concept-collection.github.io/numbl-project-example/)).
  A minimal numbl project deployed to GitHub Pages; a starter template.
- **[numbl-embed-example](https://github.com/concept-collection/numbl-embed-example)**
  ([live](https://concept-collection.github.io/numbl-embed-example/)).
  How to embed editable, runnable numbl scripts inside Markdown rendered on
  GitHub Pages.

## Data compression

- **[benchcompress](https://github.com/concept-collection/benchcompress)**
  ([results](https://concept-collection.github.io/benchcompress/),
  [paper (WIP)](https://concept-collection.github.io/benchcompress/paper)).
  A benchmarking framework for compression algorithms on scientific data
  arrays: compression ratio and encode/decode throughput.
- **[ephys_compression_tests](https://github.com/concept-collection/ephys_compression_tests)**
  ([results](https://concept-collection.github.io/ephys_compression_tests/)).
  Compression benchmarks for electrophysiology recordings.
- **[ans-visualizer](https://github.com/concept-collection/ans-visualizer)**
  ([live](https://concept-collection.github.io/ans-visualizer/)).
  A visualizer for the Asymmetric Numeral Systems (ANS) entropy-coding
  algorithm ([Duda et al., 2015](https://ieeexplore.ieee.org/abstract/document/7170048)).

## Neurophysiology data and remote access

- **[remote-hdf5-lazy-read](https://github.com/concept-collection/remote-hdf5-lazy-read)**
  ([live](https://concept-collection.github.io/remote-hdf5-lazy-read/)).
  How [neurosift](https://neurosift.app/) browses large remote
  [NWB](https://www.nwb.org/)/HDF5 files in the browser using HTTP range
  requests, with no full download and no backend.
- **[dandiset_000986](https://github.com/concept-collection/dandiset_000986)**
  ([visualizations](https://concept-collection.github.io/dandiset_000986/)).
  Reproducible figures and visualizations for
  [DANDI Dandiset 000986](https://dandiarchive.org/dandiset/000986)
  (mouse auditory cortex recordings).

## Mathematical visualizers

- **[finite-field-visualizer](https://github.com/concept-collection/finite-field-visualizer)**
  ([live](https://concept-collection.github.io/finite-field-visualizer/)).
  Color-coded multiplication tables over finite (prime) fields; step through
  primes to see the structure change.
- **[gcd-visualizer](https://github.com/concept-collection/gcd-visualizer)**
  ([live](https://concept-collection.github.io/gcd-visualizer/)).
  A color-coded GCD table: the greatest common divisor of every pair (i, j)
  shown as a heatmap.
