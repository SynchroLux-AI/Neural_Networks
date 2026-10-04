<h2>$\color{lightyellow}{\text{A Unified, Deep-Learning Pipeline for Cross-Modality Electron-Microscopy}}$</h2>
<h2>$\color{lightyellow}{\text{Metrology of Nanoparticles}}$ </h2>
<h2> $\square$ Period: July 2026 ~ </h2>

Electron microscopy is central to materials and soft-matter research, yet extracting quantitative, comparable information across instruments and imaging modalities remains a persistent bottleneck. 
SEM, TEM, STEM, and tomography each encode structure differently---different contrast mechanisms, resolutions, noise statistics, and detector responses---so measurements are rarely transferable between them.
This fragmentation limits the scientific value of the vast, hard-won micrograph collections already available, and forces repeated, costly acquisition.

This project develops a unified, deep-learning pipeline that operates directly on raw micrographs and bridges these modalities. 
Rather than training separate models per instrument, we learn shared representations of microstructure that transfer across imaging conditions, enabling consistent metrology---segmentation, 
particle and pore statistics, and structure-property prediction---from heterogeneous data. The pipeline combines lightweight, EM-aware convolutional encoders with cross-modality alignment, 
self-supervised pretraining, and uncertainty-aware heads, so that scarce labelled data and differing acquisition settings are handled explicitly.

Our goals are threefold: 
(i) build modality-agnostic backbones that generalise with minimal retraining; 
(ii) align representations across modalities for cross-instrument comparability; and 
(iii) deliver calibrated, interpretable predictions linking microscopy to mechanical, chemical, optical, and rheological properties.
Grounding the models in materials physics and quantifying uncertainty keeps predictions trustworthy and actionable.

By unifying data across modalities, this work aims to turn isolated micrographs into a coherent, reusable metrology resource---accelerating materials discovery and enabling robust, 
reproducible analysis from laboratory to industrial scale.

Collaborating institutions: Seoul National University and Korea Institute of Science and Technology
