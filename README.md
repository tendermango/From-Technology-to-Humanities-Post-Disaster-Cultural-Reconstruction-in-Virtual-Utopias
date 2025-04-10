# Digital Minaret Reconstruction in Virtual Utopias

This repository contains experimental datasets, models, and visual results from the research project _"Post-Conflict Cultural Reconstruction in Virtual Utopias: A Case Study of the Great Mosque of Aleppo"_.

We present a comprehensive digital heritage reconstruction pipeline involving texture style transfer, 3D local structure editing, and immersive audio fusion.

## Table of Contents

- [Overview](#overview)
- [Structure](#structure)
- [Experiments](#experiments)
  - [4.3 Texture Style Transfer & 3D Reconstruction](#43-texture-style-transfer--3d-reconstruction)
  - [4.4 Local Structure Repaint](#44-local-structure-repaint)
  - [4.5 Environmental Audio Fusion](#45-environmental-audio-fusion)
- [License](#license)

---

## Overview

The project aims to digitally reconstruct the Great Mosque of Aleppo using advanced AI tools. Combining NeRF-based 3D modeling with style-conditioned generation (Stable Diffusion) and immersive audio reconstruction (Jukebox, Hifi-GAN), this research addresses post-war cultural recovery through digital presence and utopian imagination.

## Structure

Each folder corresponds to one major experimental module from the paper:

- **4.3**: Texture Transfer on 3D Surfaces + NeRF Reconstruction
- **4.4**: Local Structure Repaint & Geometry Enhancement
- **4.5**: Environmental Audio Feature Extraction, Fusion, and Enhancement

---

Experiments

4.3 Texture Style Transfer & 3D Reconstruction

We apply Stable Diffusion to minaret datasets using Arabic decorative motifs, followed by NeRF (Nerfacto) reconstruction. Visual results demonstrate the feasibility of architectural style simulation in 3D space.
	•	style_transfer.py: Applies texture transfer on input 2D images
	•	nerf_training.md: Details on NeRF setup, COLMAP preprocessing, and training parameters

4.4 Local Structure Repaint

NeRF-generated 3D models are enhanced with structural refinements and re-trained to improve geometric continuity across domes, towers, and carvings.
	•	local_repaint.py: Stable Diffusion-based local adjustments
	•	nerf_retrain.md: NeRF retraining after modifications

4.5 Environmental Audio Fusion

We process mosque-related environmental audio using STFT and Hifi-GAN to build a layered immersive soundscape.
	•	audio_fusion.py: Frequency separation and re-synthesis
	•	kmeans_visualization.py: 3D cluster visualization using K-means
	•	audio_enhancement.md: Hifi-GAN settings and output details


License

This project is licensed under the MIT License - see the LICENSE file for details.
