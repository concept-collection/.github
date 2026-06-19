# Concept Collection

A set of small, independent projects: interactive demos, teaching material, and
research code. Most run directly in the browser with nothing to install. The
recurring themes are running MATLAB-syntax code in the browser with
[numbl](https://numbl.org), tooling for scientific data, and visualizing
mathematical structure.

Each project below links to its repository, and to a live page where there is
one.

## Run-in-browser MATLAB (numbl)

MATLAB-syntax projects that run in the browser via [numbl](https://numbl.org).

- **[numbl-quantum-optics](https://github.com/concept-collection/numbl-quantum-optics)**
  ([live](https://concept-collection.github.io/numbl-quantum-optics/)).
  Runnable scripts accompanying the article "Quantum optics in MATLAB"
  ([arXiv:2309.14354](https://arxiv.org/abs/2309.14354)), covering quantum
  states, operators, and dynamics.
- **[numbl-open-quantum-systems](https://github.com/concept-collection/numbl-open-quantum-systems)**
  ([live](https://concept-collection.github.io/numbl-open-quantum-systems/)).
  Code from "Coding closed and open quantum systems in MATLAB"
  ([arXiv:1911.04906](https://arxiv.org/abs/1911.04906)), including Ising
  dynamics, cavity-QED phase transitions, and Lindblad and non-Markovian
  evolution.
- **[numbl-distmesh](https://github.com/concept-collection/numbl-distmesh)**
  ([live](https://concept-collection.github.io/numbl-distmesh/)).
  Every example from Persson and Strang's
  [DistMesh](https://github.com/popersson/DistMesh), meshing 2-D regions and
  surfaces from signed distance functions.
- **[numbl-surfacefun-intro](https://github.com/concept-collection/numbl-surfacefun-intro)**
  ([live](https://concept-collection.github.io/numbl-surfacefun-intro/)).
  An introduction to [surfacefun](https://github.com/danfortunato/surfacefun),
  which computes with functions on surfaces and solves PDEs on them to high
  order.
- **[surfacefun-interactive](https://github.com/concept-collection/surfacefun-interactive)**
  ([live](https://concept-collection.github.io/surfacefun-interactive/)).
  surfacefun demos with live sliders, where React and three.js drive a numbl
  script. Refine a cubed-sphere mesh or scale a tangent vector field and watch
  it update.
- **[numbl-chunkie](https://github.com/concept-collection/numbl-chunkie)**
  ([live](https://concept-collection.github.io/numbl-chunkie/)).
  Examples for [chunkie](https://github.com/fastalgorithms/chunkie): building
  chunker geometries in 2-D and solving Laplace, Helmholtz, and Stokes boundary
  integral equations.
- **[numbl-image-filter](https://github.com/concept-collection/numbl-image-filter)**
  ([live](https://concept-collection.github.io/numbl-image-filter/)).
  Upload an image, write a MATLAB-syntax filter, and run it on the image in the
  browser.
- **[numbl-project-example](https://github.com/concept-collection/numbl-project-example)**
  ([live](https://concept-collection.github.io/numbl-project-example/)).
  A minimal numbl project deployed to GitHub Pages, meant as a starting
  template.
- **[numbl-embed-example](https://github.com/concept-collection/numbl-embed-example)**
  ([live](https://concept-collection.github.io/numbl-embed-example/)).
  Shows how to embed editable, runnable numbl scripts inside Markdown rendered
  on GitHub Pages.

## Data compression

- **[benchcompress](https://github.com/concept-collection/benchcompress)**
  ([results](https://concept-collection.github.io/benchcompress/),
  [paper (WIP)](https://concept-collection.github.io/benchcompress/paper)).
  A benchmarking framework that measures compression ratio and encode/decode
  throughput for compression algorithms on scientific data arrays.
- **[ephys_compression_tests](https://github.com/concept-collection/ephys_compression_tests)**
  ([results](https://concept-collection.github.io/ephys_compression_tests/)).
  Compression benchmarks for electrophysiology recordings.
- **[ans-visualizer](https://github.com/concept-collection/ans-visualizer)**
  ([live](https://concept-collection.github.io/ans-visualizer/)).
  A step-by-step visualizer for the Asymmetric Numeral Systems (ANS)
  entropy-coding algorithm ([Duda et al., 2015](https://ieeexplore.ieee.org/abstract/document/7170048)).

## Neurophysiology data and remote access

- **[remote-hdf5-lazy-read](https://github.com/concept-collection/remote-hdf5-lazy-read)**
  ([live](https://concept-collection.github.io/remote-hdf5-lazy-read/)).
  Shows how [neurosift](https://neurosift.app/) browses large remote
  [NWB](https://www.nwb.org/)/HDF5 files in the browser using HTTP range
  requests, with no full download and no backend.
- **[dandiset_000986](https://github.com/concept-collection/dandiset_000986)**
  ([visualizations](https://concept-collection.github.io/dandiset_000986/)).
  Reproducible figures and visualizations for
  [DANDI Dandiset 000986](https://dandiarchive.org/dandiset/000986), a set of
  mouse auditory cortex recordings.

## Mathematical visualizers

- **[finite-field-visualizer](https://github.com/concept-collection/finite-field-visualizer)**
  ([live](https://concept-collection.github.io/finite-field-visualizer/)).
  Color-coded multiplication tables over finite (prime) fields. Step through the
  primes to watch the structure change.
- **[gcd-visualizer](https://github.com/concept-collection/gcd-visualizer)**
  ([live](https://concept-collection.github.io/gcd-visualizer/)).
  A heatmap of the greatest common divisor of every pair (i, j), laid out as a
  color-coded table.

## Computational geometry

- **[qhull-wasm-demo](https://github.com/concept-collection/qhull-wasm-demo)**
  ([live](https://concept-collection.github.io/qhull-wasm-demo/)).
  Demos and benchmarks for [qhull-wasm](https://github.com/magland/qhull-wasm),
  which compiles [Qhull](http://www.qhull.org) to WebAssembly. Includes 2-D
  Delaunay triangulation, 3-D convex hull, and a Delaunay benchmark with
  matching scripts for MATLAB, Octave, and numbl.
