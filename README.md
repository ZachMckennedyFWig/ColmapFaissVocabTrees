# COLMAP Pre-built Vocab Trees (FAISS Conversion)

This repository provides the pre-built vocabulary trees for COLMAP, originally available from [demuc.de/colmap/](https://demuc.de/colmap/), converted from their original FLANN format to FAISS.

---

## What I Did

COLMAP traditionally uses FLANN (Fast Library for Approximate Nearest Neighbors) for its vocabulary tree-based image retrieval. However, newer versions of COLMAP expect **FAISS** (Facebook AI Similarity Search) indices. I have taken the publicly available vocabulary tree files from the COLMAP project and converted them to the **FAISS format**, allowing for direct use with COLMAP installations configured to utilize FAISS for vocabulary tree matching.

---

## Usage

Simply replace your existing COLMAP vocabulary tree files with the **FAISS-converted files** provided in this repository. Ensure your COLMAP installation is configured to use FAISS for vocabulary tree matching.

---

## Citations

If you use these converted vocabulary trees in your research or project, please cite the original **COLMAP** project and the **FAISS** library:

### COLMAP

```bibtex
@inproceedings{schoenberger2016sfm,
  author={Schönberger, Johannes Lutz and Frahm, Jan-Michael},
  title={Structure-from-Motion Revisited},
  booktitle={Conference on Computer Vision and Pattern Recognition (CVPR)},
  year={2016},
}

@inproceedings{schoenberger2016vote,
  author={Schönberger, Johannes Lutz and Price, True and Sattler, Torsten and Frahm, Jan-Michael and Pollefeys, Marc},
  title={A Vote-and-Verify Strategy for Fast Spatial Verification in Image Retrieval},
  booktitle={Asian Conference on Computer Vision (ACCV)},
  year={2016},
}
```

### FAISS

```bibtex
@article{douze2024faiss,
  title={The Faiss library},
  author={Matthijs Douze and Alexandr Guzhva and Chengqi Deng and Jeff Johnson and Gergely Szilvasy and Pierre-Emmanuel Mazaré and Maria Lomeli and Lucas Hosseini and Hervé Jégou},
  year={2024},
  eprint={2401.08281},
  archivePrefix={arXiv},
  primaryClass={cs.LG}
}

@article{johnson2019billion,
  title={Billion-scale similarity search with {GPUs}},
  author={Johnson, Jeff and Douze, Matthijs and J{\'e}gou, Herv{\'e}},
  journal={IEEE Transactions on Big Data},
  volume={7},
  number={3},
  pages={535--547},
  year={2019},
  publisher={IEEE}
}
```
