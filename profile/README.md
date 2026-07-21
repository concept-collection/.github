# Concept Collection

This is a collection of random proof-of-concept projects, most of which are demos that can be run entirely in the web browser (client side). Many of them are centered around the [numbl project](https://numbl.org).

## jupyterlite-numbl-kernel

Here's a proof of concept for running MATLAB syntax in Jupyter entirely client side (no kernel, no server). It uses numbl and JupyterLite.

[Repository](https://github.com/concept-collection/jupyterlite-numbl-kernel) · [Live](https://concept-collection.github.io/jupyterlite-numbl-kernel/)

## Interactive MCMC samplers

Here are a couple of demonstrations of MCMC samplers that you can watch run. They use numbl (MATLAB syntax in the browser) to do the sampling client-side in the browser. In the case of WALNUTS (the within-orbit adaptive leapfrog No-U-Turn Sampler), we use the exact MATLAB code that is a companion to the paper.

- **[hitandrun-interactive](https://github.com/concept-collection/hitandrun-interactive)** · [live](https://concept-collection.github.io/hitandrun-interactive/#figure/sampler)
- **[walnuts-interactive](https://github.com/concept-collection/walnuts-interactive)** · [live](https://concept-collection.github.io/walnuts-interactive/#figure/sampler)

## Embedding & hosting numbl projects

Here are a couple of projects that let you embed or host your own numbl/MATLAB projects entirely client side.

- **[numbl-embed-example](https://github.com/concept-collection/numbl-embed-example)** · [live](https://concept-collection.github.io/numbl-embed-example/)
- **[numbl-project-example](https://github.com/concept-collection/numbl-project-example)** · [live](https://concept-collection.github.io/numbl-project-example/)

## VS Code–style IDEs

Here are a couple of VS Code–style IDEs that run entirely in the browser — one for MATLAB syntax (via numbl), one for Stan.

- **[numbl-web-ide](https://github.com/concept-collection/numbl-web-ide)** · [live](https://concept-collection.github.io/numbl-web-ide/)
- **[stan-web-ide](https://github.com/concept-collection/stan-web-ide)** · [live](https://concept-collection.github.io/stan-web-ide/)

## surfacefun examples

[Surfacefun](https://surfacefun.readthedocs.io/en/latest/) is a MATLAB package for computing with functions defined on surfaces and solving PDEs on them to high order. Here are some examples that run surfacefun via numbl in the browser.

- **[numbl-surfacefun-intro](https://github.com/concept-collection/numbl-surfacefun-intro)** · [live](https://concept-collection.github.io/numbl-surfacefun-intro/)
- **[surfacefun-interactive](https://github.com/concept-collection/surfacefun-interactive)** · [live](https://concept-collection.github.io/surfacefun-interactive/)
- **[mesh-pde-solver](https://github.com/concept-collection/mesh-pde-solver)** · [live](https://concept-collection.github.io/mesh-pde-solver/)

## chunkie examples

[Chunkie](https://chunkie.readthedocs.io/en/latest/) is a MATLAB package for solving boundary integral equations in two dimensions. Here are some examples that run chunkie via numbl in the browser.

- **[numbl-chunkie](https://github.com/concept-collection/numbl-chunkie)** · [live](https://concept-collection.github.io/numbl-chunkie/)

## Matrix multiplication benchmark

Here's a benchmark of matrix-matrix multiply (GEMM) in the browser across several implementations: a plain JavaScript loop, WebGPU, hand-written C compiled to WASM (SIMD and threads), and a real BLAS (libFLAME) compiled to WASM, with a native reference for comparison.

- **[matmul-bench](https://github.com/concept-collection/matmul-bench)** · [live](https://concept-collection.github.io/matmul-bench/)

## Lazy reading of remote HDF5 files

Here's a demo of reading large remote HDF5 files, such as [NWB](https://www.nwb.org/) neurophysiology files, directly in the browser using HTTP range requests, with no full download and no backend. It shows the approach that [neurosift](https://neurosift.app/) uses to browse these files.

- **[remote-hdf5-lazy-read](https://github.com/concept-collection/remote-hdf5-lazy-read)** · [live](https://concept-collection.github.io/remote-hdf5-lazy-read/)

## Scientific data compression

- **[ans-visualizer](https://github.com/concept-collection/ans-visualizer)**
  ([live](https://concept-collection.github.io/ans-visualizer/)).
  A step-by-step visualizer for the Asymmetric Numeral Systems (ANS)
  entropy-coding algorithm ([Duda et al., 2015](https://ieeexplore.ieee.org/abstract/document/7170048)).
- **[benchcompress](https://github.com/concept-collection/benchcompress)**
  ([results](https://concept-collection.github.io/benchcompress/),
  [paper (WIP)](https://concept-collection.github.io/benchcompress/paper)).
  A benchmarking framework that measures compression ratio and encode/decode
  throughput for compression algorithms on scientific data arrays.
- **[ephys_compression_tests](https://github.com/concept-collection/ephys_compression_tests)**
  ([results](https://concept-collection.github.io/ephys_compression_tests/)).
  Compression benchmarks for electrophysiology recordings.

## Other projects

### numbl platform: templates & tooling

Utilities and starting points for building your own
[numbl](https://numbl.org) projects.

- **[numbl-figure-viewer](https://github.com/concept-collection/numbl-figure-viewer)**
  ([live](https://concept-collection.github.io/numbl-figure-viewer/)).
  Open and explore a figure exported from numbl, including its underlying data.

### Peer-to-peer shared state

- **[hitandrun-commonview](https://github.com/concept-collection/hitandrun-commonview)**
  ([live](https://concept-collection.github.io/hitandrun-commonview/)).
  The hit-and-run figure with a single live view shared by all visitors over a
  WebRTC mesh; one peer runs the sampler via numbl and broadcasts to the rest.
- **[commonview](https://github.com/concept-collection/commonview)**
  ([live](https://concept-collection.github.io/commonview/)).
  A minimal peer-to-peer page where every visitor shares one state (a counter):
  nostr discovery, a WebRTC mesh, and a central-peer authority. The basis for
  hitandrun-commonview.

### Geometry, meshing & PDE solvers

- **[mesh-studio](https://github.com/concept-collection/mesh-studio)**
  ([live](https://concept-collection.github.io/mesh-studio/)).
  Build CAD primitives or import STEP/IGES with
  [OpenCASCADE.js](https://ocjs.org/), then inspect them in 3D — including each
  face's true NURBS surface (polynomials on faces), not just its triangulation.
- **[mesh-converter](https://github.com/concept-collection/mesh-converter)**
  ([live](https://concept-collection.github.io/mesh-converter/)).
  Convert meshes between 19 formats (PLY, OBJ, STL, VTK, Gmsh, XDMF, …) with
  [meshio](https://github.com/nschloe/meshio) running in-browser on Pyodide;
  inspect meshes in 3D and see what a lossy export would drop.
- **[qhull-wasm-demo](https://github.com/concept-collection/qhull-wasm-demo)**
  ([live](https://concept-collection.github.io/qhull-wasm-demo/)).
  Demos and benchmarks for [qhull-wasm](https://github.com/magland/qhull-wasm),
  which compiles [Qhull](http://www.qhull.org) to WebAssembly. Includes 2-D
  Delaunay triangulation, 3-D convex hull, and a Delaunay benchmark with
  matching scripts for MATLAB, Octave, and numbl.
- **[numbl-distmesh](https://github.com/concept-collection/numbl-distmesh)**
  ([live](https://concept-collection.github.io/numbl-distmesh/)).
  Every example from Persson and Strang's
  [DistMesh](https://github.com/popersson/DistMesh), meshing 2-D regions and
  surfaces from signed distance functions.
- **[abc-step-1000](https://github.com/concept-collection/abc-step-1000)**
  ([live](https://concept-collection.github.io/abc-step-1000/)).
  The first 1000 STEP files from the
  [ABC dataset](https://deep-geometry.github.io/abc-dataset/) of CAD models
  (Koch et al., CVPR 2019), served gzip-compressed with a JSON manifest for
  direct download.

### Neurophysiology data & remote access

- **[dandiset_000986](https://github.com/concept-collection/dandiset_000986)**
  ([visualizations](https://concept-collection.github.io/dandiset_000986/)).
  Reproducible figures and visualizations for
  [DANDI Dandiset 000986](https://dandiarchive.org/dandiset/000986), a set of
  mouse auditory cortex recordings.

### Physics & quantum systems

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

### Image processing

- **[numbl-image-filter](https://github.com/concept-collection/numbl-image-filter)**
  ([live](https://concept-collection.github.io/numbl-image-filter/)).
  Upload an image, write a MATLAB-syntax filter, and run it on the image in the
  browser.

### Number theory & visual math

- **[finite-field-visualizer](https://github.com/concept-collection/finite-field-visualizer)**
  ([live](https://concept-collection.github.io/finite-field-visualizer/)).
  Color-coded multiplication tables over finite (prime) fields. Step through the
  primes to watch the structure change.
- **[gcd-visualizer](https://github.com/concept-collection/gcd-visualizer)**
  ([live](https://concept-collection.github.io/gcd-visualizer/)).
  A heatmap of the greatest common divisor of every pair (i, j), laid out as a
  color-coded table.
