# SpaMOMA

### Unifying and aligning spatial multi-omics slices via image-based feature matching

------------------------------------------------------------------------



## 📚 Tutorials

``` {toctree}
:maxdepth: 1

Tutorials/Installation
Tutorials/API
Tutorials/Tutorial1_Aligning_eight_spatial_transcriptomics_slices_of_mouse_hippocampus
Tutorials/Tutorial2_Aligning_spatial_transcriptomics_slices_of_mouse_olfactory_bulb
Tutorials/Tutorial3_Aligning_spatial_transcriptomics_data_and_spatial_epigenomics_data_of_mouse_coronal_brain_slices
Tutorials/Tutorial4_Aligning_spatial_transcriptomics_data_and_spatial_proteomics_data_of_mouse_thymus_slices
Tutorials/Tutorial5_Aligning_spatial_transcriptomics_data_to_spatial_metabolomics_data_of_mouse_brain_slices
Tutorials/Tutorial6_Aligning_spatial_transcriptomics_data_to_H&E_image_of_human_breast_cancer_data_from_Xenium
Tutorials/Tutorial7_Aligning_spatial_transcriptomics_spatial_epigenomics_data_and_H&E_image_of_mouse_embryonic_brain_data_from_MISAR-seq
```

------------------------------------------------------------------------

## 🔎 Overview

![SpaMOMA Architecture](./assets/architecture.png)

Simultaneous spatial profiling of multiple omics within the same cell or spot offers unprecedented opportunities to dissect spatiotemporal interplay among different omics, and to decode molecular properties in microenvironments. However, direct co-profiling of spatial multi-omics faces challenges due to limited sample input, signal crosstalk, and the trade-off between spatial resolution and omics coverage. Profiling different omics from consecutive tissue slices offers a practical alternative but introduces challenges to accurately align distorted slices across modalities. 

Here, we present SpaMOMA, a computational framework for **unpaired spatial multi-omics slice alignment**. SpaMOMA designs a coarse-to-fine alignment strategy based on test-time adaptation to tailor image feature matching model to spatial pattern images, enabling automated and high-precision alignment without manual landmarks or matched features across different omics. 

Extensive benchmarks across diverse spatial omics datasets and histology images demonstrate that SpaMOMA:

-   Resolves global orientation ambiguities
-   Achieves accurate local alignment
-   Consistently outperforms existing alignment methods

Beyond spatial alignment, SpaMOMA facilitates downstream analyses including:

-   📍 Coordinate-based omics-to-omics translation
-   🧬 Multi-omics spatial domain identification
-   🔬 Histology-guided spot resolution enhancement

This scalable and robust framework lowers technical barriers for unpaired spatial multi-omics integration and paves the way for comprehensive multimodal tissue analysis.

------------------------------------------------------------------------

## ✉️ Contact

If you have any questions or need support, please feel free to contact:

**Jianxing Zhang**\
📩 24126421@bjtu.edu.cn
