# Image Processing — Algorithms Implemented from Scratch

Implementations of classic image-processing algorithms built
**from scratch in NumPy** — no OpenCV/skimage black boxes. Each topic is a
self-contained Jupyter notebook with the problem statement, the implementation,
and visual results.

## Algorithms implemented

| # | Topic | Techniques implemented manually |
|---|-------|----------------------------------|
| 1 | **Histogram Equalization / Matching** | Manual histogram + CDF remapping; tiled histogram-matching reconstruction |
| 2 | **Image Enhancement** | Salt-&-pepper + Gaussian noise; manual median filter; directional (edge-preserving) smoothing with 8 oriented masks |
| 3 | **Binary Images** | Connected-components labeling; morphological erosion/dilation; skeletonization |
| 4 | **Edge Detection & Hough Transform** | Full Canny pipeline (gradients → non-max suppression → hysteresis); gradient-guided Hough circle detection |
| 5 | **Fast Fourier Transform** | Frequency-domain denoising — detect periodic-noise peaks and apply notch filters |

Each `Assignment-*/` folder holds two notebooks: `assignment.ipynb` (the problem
statement) and `solution.ipynb` (my implementation).

## Tech

`numpy`, `scipy`, `matplotlib`, `Pillow`, `requests`.

## Running

The notebooks were written for **Google Colab** and run top-to-bottom (each
function is defined in its own cell). Open any `solution.ipynb` and run all
cells in order (`Runtime → Restart session and run all` on Colab).

## Credit

The original problem statements come from the course repository
[`dnevo/ImageProcessing`](https://github.com/dnevo/ImageProcessing); the
implementations in each `solution.ipynb` are my own.
