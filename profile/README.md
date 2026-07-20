# Concept Collection

A set of small, independent projects: interactive demos, teaching material, and
research code. Most run directly in the browser with nothing to install, and
many are written in MATLAB syntax and run there via [numbl](https://numbl.org).

Projects are grouped below by **application area** — sampling, geometry and
meshing, visual math, neurophysiology, data compression, physics, and more —
rather than by the technology behind them. The most interactive and visual
demos come first; utilities, datasets, and templates are toward the end. Each
links to its repository, and to a live page where there is one.

## Monte Carlo & sampling

- **[hitandrun-interactive](https://github.com/concept-collection/hitandrun-interactive)**
  ([live](https://concept-collection.github.io/hitandrun-interactive/#figure/sampler)).
  Hit-and-run MCMC sampling of a 2-D convex region, with React driving a numbl
  script. Resample, make new regions, or play a step-by-step movie of the
  algorithm.
- **[walnuts-interactive](https://github.com/concept-collection/walnuts-interactive)**
  ([live](https://concept-collection.github.io/walnuts-interactive/#figure/sampler)).
  WALNUTS (the within-orbit adaptive leapfrog No-U-Turn Sampler) drawing from a
  2-D banana target, with React driving a numbl script. Tune the leapfrog step
  and error tolerance, or play a step-by-step movie of the orbit-building.
- **[stan-web-ide](https://github.com/concept-collection/stan-web-ide)**
  ([live](https://concept-collection.github.io/stan-web-ide/)).
  Run [Stan](https://mc-stan.org) sampling in your browser, in a VS Code-style
  IDE.

## Peer-to-peer shared state

- **[hitandrun-commonview](https://github.com/concept-collection/hitandrun-commonview)**
  ([live](https://concept-collection.github.io/hitandrun-commonview/)).
  The hit-and-run figure with a single live view shared by all visitors over a
  WebRTC mesh; one peer runs the sampler via numbl and broadcasts to the rest.
- **[commonview](https://github.com/concept-collection/commonview)**
  ([live](https://concept-collection.github.io/commonview/)).
  A minimal peer-to-peer page where every visitor shares one state (a counter):
  nostr discovery, a WebRTC mesh, and a central-peer authority. The basis for
  hitandrun-commonview.

## Geometry, meshing & PDE solvers

- **[surfacefun-interactive](https://github.com/concept-collection/surfacefun-interactive)**
  ([live](https://concept-collection.github.io/surfacefun-interactive/)).
  surfacefun demos with live sliders, where React and three.js drive a numbl
  script. Refine a cubed-sphere mesh or scale a tangent vector field and watch
  it update.
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
- **[mesh-pde-solver](https://github.com/concept-collection/mesh-pde-solver)**
  ([live](https://concept-collection.github.io/mesh-pde-solver/)).
  Upload a quad surface mesh and solve Poisson or Helmholtz problems on it
  with [surfacefun](https://github.com/danfortunato/surfacefun), entirely in
  the browser; the solution renders in a rotatable 3D view.
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
- **[numbl-surfacefun-intro](https://github.com/concept-collection/numbl-surfacefun-intro)**
  ([live](https://concept-collection.github.io/numbl-surfacefun-intro/)).
  An introduction to [surfacefun](https://github.com/danfortunato/surfacefun),
  which computes with functions on surfaces and solves PDEs on them to high
  order.
- **[numbl-chunkie](https://github.com/concept-collection/numbl-chunkie)**
  ([live](https://concept-collection.github.io/numbl-chunkie/)).
  Examples for [chunkie](https://github.com/fastalgorithms/chunkie): building
  chunker geometries in 2-D and solving Laplace, Helmholtz, and Stokes boundary
  integral equations.
- **[abc-step-1000](https://github.com/concept-collection/abc-step-1000)**
  ([live](https://concept-collection.github.io/abc-step-1000/)).
  The first 1000 STEP files from the
  [ABC dataset](https://deep-geometry.github.io/abc-dataset/) of CAD models
  (Koch et al., CVPR 2019), served gzip-compressed with a JSON manifest for
  direct download.

## Number theory & visual math

- **[finite-field-visualizer](https://github.com/concept-collection/finite-field-visualizer)**
  ([live](https://concept-collection.github.io/finite-field-visualizer/)).
  Color-coded multiplication tables over finite (prime) fields. Step through the
  primes to watch the structure change.
- **[gcd-visualizer](https://github.com/concept-collection/gcd-visualizer)**
  ([live](https://concept-collection.github.io/gcd-visualizer/)).
  A heatmap of the greatest common divisor of every pair (i, j), laid out as a
  color-coded table.

## Neurophysiology data & remote access

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

## Physics & quantum systems

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

## Image processing

- **[numbl-image-filter](https://github.com/concept-collection/numbl-image-filter)**
  ([live](https://concept-collection.github.io/numbl-image-filter/)).
  Upload an image, write a MATLAB-syntax filter, and run it on the image in the
  browser.

## numbl platform: templates & tooling

Utilities and starting points for building your own
[numbl](https://numbl.org) projects.

- **[numbl-web-ide](https://github.com/concept-collection/numbl-web-ide)**
  ([live](https://concept-collection.github.io/numbl-web-ide/)).
  Run MATLAB-syntax .m files in your browser, in a VS Code-style IDE.
- **[jupyterlite-numbl-kernel](https://github.com/concept-collection/jupyterlite-numbl-kernel)**
  ([live](https://concept-collection.github.io/jupyterlite-numbl-kernel/)).
  A JupyterLite kernel that runs numbl in notebook cells entirely in the
  browser, with inline figures and mip packages.
- **[numbl-figure-viewer](https://github.com/concept-collection/numbl-figure-viewer)**
  ([live](https://concept-collection.github.io/numbl-figure-viewer/)).
  Open and explore a figure exported from numbl, including its underlying data.
- **[numbl-project-example](https://github.com/concept-collection/numbl-project-example)**
  ([live](https://concept-collection.github.io/numbl-project-example/)).
  A minimal numbl project deployed to GitHub Pages, meant as a starting
  template.
- **[numbl-embed-example](https://github.com/concept-collection/numbl-embed-example)**
  ([live](https://concept-collection.github.io/numbl-embed-example/)).
  Shows how to embed editable, runnable numbl scripts inside Markdown rendered
  on GitHub Pages.
