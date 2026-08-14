# Concept Collection

This is a collection of random small projects and demos, most of which can be run entirely in the web browser (client side). Many of them are centered around the [numbl project](https://numbl.org).

## Interactive numerical methods

Methods from the numerical literature that you can watch run and adjust, computed client side by numbl (MATLAB syntax in the browser).

- **[hitandrun-interactive](https://github.com/concept-collection/hitandrun-interactive)** · [live](https://concept-collection.github.io/hitandrun-interactive/#figure/sampler) · the hit-and-run MCMC sampler
- **[walnuts-interactive](https://github.com/concept-collection/walnuts-interactive)** · [live](https://concept-collection.github.io/walnuts-interactive/#figure/sampler) · the WALNUTS sampler, running the paper's own companion MATLAB code
- **[barycentric-rational](https://github.com/concept-collection/barycentric-rational)** · [live](https://concept-collection.github.io/barycentric-rational/) · Floater-Hormann rational interpolation, pole-free on any nodes; the method is a MATLAB script you edit in the page

## numbl tooling: Jupyter, embedding, IDEs

Ways to write, run, and share MATLAB-syntax code in the browser, all client side (plus a Stan variant of the IDE).

- **[jupyterlite-numbl-kernel](https://github.com/concept-collection/jupyterlite-numbl-kernel)** · [live](https://concept-collection.github.io/jupyterlite-numbl-kernel/) · MATLAB syntax in Jupyter, no kernel server
- **[numbl-embed-example](https://github.com/concept-collection/numbl-embed-example)** · [live](https://concept-collection.github.io/numbl-embed-example/) · embed numbl in your own page
- **[numbl-project-example](https://github.com/concept-collection/numbl-project-example)** · [live](https://concept-collection.github.io/numbl-project-example/) · host a numbl project as a static site
- **[numbl-web-ide](https://github.com/concept-collection/numbl-web-ide)** · [live](https://concept-collection.github.io/numbl-web-ide/) · a VS Code–style IDE for MATLAB syntax
- **[stan-web-ide](https://github.com/concept-collection/stan-web-ide)** · [live](https://concept-collection.github.io/stan-web-ide/) · the same IDE for Stan
- **[numbl-figure-viewer](https://github.com/concept-collection/numbl-figure-viewer)** · [live](https://concept-collection.github.io/numbl-figure-viewer/) · open a figure exported from numbl, underlying data included

## surfacefun & chunkie examples

[Surfacefun](https://surfacefun.readthedocs.io/en/latest/) (functions and PDEs on surfaces) and [chunkie](https://chunkie.readthedocs.io/en/latest/) (boundary integral equations in 2D) are MATLAB packages; these examples run them in the browser via numbl.

- **[numbl-surfacefun-intro](https://github.com/concept-collection/numbl-surfacefun-intro)** · [live](https://concept-collection.github.io/numbl-surfacefun-intro/)
- **[surfacefun-interactive](https://github.com/concept-collection/surfacefun-interactive)** · [live](https://concept-collection.github.io/surfacefun-interactive/)
- **[mesh-pde-solver](https://github.com/concept-collection/mesh-pde-solver)** · [live](https://concept-collection.github.io/mesh-pde-solver/)
- **[numbl-chunkie](https://github.com/concept-collection/numbl-chunkie)** · [live](https://concept-collection.github.io/numbl-chunkie/)

## MRI pulse sequences

[Pulseq](https://pulseq.github.io/) is an open framework for defining MRI pulse sequences. Here you can write pulseq sequences in MATLAB syntax and run them in the browser via numbl to generate a `.seq` file, upload and interactively explore an existing one, or simulate one on a digital phantom to see the raw k-space it acquires.

- **[seqlab](https://github.com/concept-collection/seqlab)** · [live](https://concept-collection.github.io/seqlab/)
- **[mri-scanner](https://github.com/concept-collection/mri-scanner)** · [live](https://concept-collection.github.io/mri-scanner/)

## Spherical harmonics on the GPU

Here are spherical harmonic transforms reimplemented from scratch as WebGPU compute shaders, modeled on [SHTNS](https://nschaeff.bitbucket.io/shtns/), together with a live reaction-diffusion solver built on them: Turing patterns forming on a sphere, with diffusion handled implicitly in spectral space where the Laplace-Beltrami operator is diagonal. turing-surface extends the solver from the round sphere to closed surfaces given by spherical-harmonic embeddings, and turing-surface-cache narrows it to a discrete menu of parameter choices whose solutions at a chosen end time are shared between all visitors through a cloud cache.

- **[shtns-webgpu](https://github.com/concept-collection/shtns-webgpu)** · [live](https://concept-collection.github.io/shtns-webgpu/)
- **[turing-sphere](https://github.com/concept-collection/turing-sphere)** · [live](https://concept-collection.github.io/turing-sphere/)
- **[turing-surface](https://github.com/concept-collection/turing-surface)** · [live](https://concept-collection.github.io/turing-surface/)
- **[turing-surface-cache](https://github.com/concept-collection/turing-surface-cache)** · [live](https://concept-collection.github.io/turing-surface-cache/)

## Browser compute benchmarks

How fast the browser can crunch numbers.

- **[math-webgpu-sandbox](https://github.com/concept-collection/math-webgpu-sandbox)** · [live](https://concept-collection.github.io/math-webgpu-sandbox/) · MATLAB-syntax scripts compiled to fused WebGPU kernels, timed with the script's own `tic`/`toc`; paste the same script into real MATLAB to compare
- **[matmul-bench](https://github.com/concept-collection/matmul-bench)** · [live](https://concept-collection.github.io/matmul-bench/) · GEMM in plain JavaScript, WebGPU, SIMD and threaded WASM, and a WASM BLAS, with a native reference

## Lazy reading of remote HDF5 files

Here's a demo of reading large remote HDF5 files, such as [NWB](https://www.nwb.org/) neurophysiology files, directly in the browser using HTTP range requests, with no full download and no backend. It shows the approach that [neurosift](https://neurosift.app/) uses to browse these files.

- **[remote-hdf5-lazy-read](https://github.com/concept-collection/remote-hdf5-lazy-read)** · [live](https://concept-collection.github.io/remote-hdf5-lazy-read/)

## Scientific data compression

Here are a few projects on compressing scientific data: a step-by-step visualizer for the [Asymmetric Numeral Systems (ANS)](https://ieeexplore.ieee.org/abstract/document/7170048) entropy-coding algorithm, an interactive study of how compressible quantized noisy time series are, a framework for benchmarking compression algorithms on scientific data arrays, and compression benchmarks for electrophysiology recordings.

- **[ans-visualizer](https://github.com/concept-collection/ans-visualizer)** · [live](https://concept-collection.github.io/ans-visualizer/)
- **[timeseries-compressibility](https://github.com/concept-collection/timeseries-compressibility)** · [live](https://concept-collection.github.io/timeseries-compressibility/)
- **[benchcompress](https://github.com/concept-collection/benchcompress)** · [results](https://concept-collection.github.io/benchcompress/) · [paper (WIP)](https://concept-collection.github.io/benchcompress/paper)
- **[ephys_compression_tests](https://github.com/concept-collection/ephys_compression_tests)** · [results](https://concept-collection.github.io/ephys_compression_tests/)

## Speech to text in the browser

Here's a dictation notepad that transcribes as you speak and never sends your audio anywhere: Whisper and Moonshine run locally via [transformers.js](https://github.com/huggingface/transformers.js), on WebGPU where it's available. The transcript accumulates into a document you can edit and copy.

- **[voicenote](https://github.com/concept-collection/voicenote)** · [live](https://concept-collection.github.io/voicenote/)

## Other projects

### Peer-to-peer shared state

- **[commonroom](https://github.com/concept-collection/commonroom)**
  ([live](https://concept-collection.github.io/commonroom/)).
  Serverless group video calls: pick a room name, share the link, and everyone
  in the room is connected over a full WebRTC mesh (up to 8 people), with
  room-wide shared settings.
- **[commonroom-recorder](https://github.com/concept-collection/commonroom-recorder)**
  ([run with npx](https://concept-collection.github.io/commonroom-recorder/)).
  Command-line bot that joins a commonroom call as a visible muted participant
  and records each participant's audio (plus the chat) to files for
  transcription.
- **[commoncall](https://github.com/concept-collection/commoncall)**
  ([live](https://concept-collection.github.io/commoncall/)).
  Serverless video calls: enter an ID, see who else is on the page, and call
  them — call setup rides over nostr relays, media flows peer-to-peer via WebRTC.
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

- **[mri-spins](https://github.com/concept-collection/mri-spins)**
  ([live](https://concept-collection.github.io/mri-spins/)).
  Interactive MRI physics: a 3D sample of spins evolving under the Bloch
  equations, with RF pulses, gradients, relaxation, a live signal trace, and a
  spoiled gradient echo sequence with scanner-like gradient sounds.
- **[acoustic-scattering-2d](https://github.com/concept-collection/acoustic-scattering-2d)**
  ([live](https://concept-collection.github.io/acoustic-scattering-2d/)).
  2D acoustic wave scattering off a room, a disk, slits, or a lens, in real
  physical units: a MATLAB time-stepper compiled through numbl to WebGPU
  compute kernels. Drop a microphone anywhere in the field and listen back in
  real time, at the pitch a microphone there would actually have heard.
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
- **[random-points-in-disk](https://github.com/concept-collection/random-points-in-disk)**
  ([live](https://concept-collection.github.io/random-points-in-disk/)).
  How many random points does it take before a disk looks like a disk? Voxel-density
  heatmaps of uniform random sampling, next to the 1/&radic;&mu; noise prediction.
