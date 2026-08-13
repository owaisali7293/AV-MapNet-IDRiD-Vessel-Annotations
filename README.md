# AV-MapNet-IDRiD-Vessel-Annotations
# AV-MapNet IDRiD Refined Retinal Vessel Annotations

This repository provides the **refined retinal vessel annotations for 32 pathological retinal fundus images from the IDRiD dataset** used in the study:

**AV-MapNet: Geodesic Vessel Tokenization and Sequential Refinement for Retinal Vessel Segmentation and Artery–Vein Classification**

The annotations are released to improve the **transparency, reproducibility, and accessibility** of the pathological retinal vessel evaluation performed in this study.

## Annotation Description

The vessel annotations were prepared by **Dr. Nasir Yasin**, Department of Ophthalmology, Aziz Fatimah Medical and Dental College, Faisalabad, Pakistan.

For each selected IDRiD image, retinal vascular structures were manually delineated/refined with particular attention to maintaining anatomically meaningful vessel trajectories.

During annotation, pathological regions that could be confused with retinal vessels were carefully excluded, including:

* Haemorrhagic regions
* Other visible non-vascular pathological structures
* Image regions not considered part of the retinal vascular tree

The resulting maps therefore represent **vessel-only reference annotations** intended for evaluating retinal vessel segmentation in the presence of pathological retinal abnormalities.

## Dataset

The annotations correspond to **32 retinal fundus images** selected from the publicly available **Indian Diabetic Retinopathy Image Dataset (IDRiD)**.

The original IDRiD retinal images are **not redistributed in this repository**. Users should obtain the corresponding retinal fundus images directly from the official IDRiD dataset source.

The image identifiers used for the annotations are retained to allow the vessel maps to be matched with their corresponding original IDRiD images.

## Repository Structure

```text
AV-MapNet-IDRiD-Vessel-Annotations/
│
├── README.md
│
├── IDRiD_XX_vessel.png
│── IDRiD_XX_vessel.png
│   └── ...
│
├── metadata.csv
│
└── examples/
    └── representative vessel annotations
```

### `annotations/`

Contains the refined binary retinal vessel maps corresponding to the selected IDRiD images.

### `metadata.csv`

Provides the correspondence between the original IDRiD image identifiers and the associated refined vessel annotation files.

### `examples/`

Contains representative examples that may be used to inspect the annotation format and vessel delineation.

## Annotation Purpose

These annotations were created specifically to support the **pathological retinal vessel analysis** reported in the AV-MapNet study.

Pathological retinal images present additional segmentation challenges because structures such as haemorrhages, exudates, microaneurysms, and intensity abnormalities may have visual characteristics that resemble retinal vessels.

The refined vessel maps were therefore prepared to provide vessel-focused reference annotations in which visible retinal vascular structures are retained while relevant non-vascular pathological regions are excluded.

These annotations were used for **qualitative pathological vessel segmentation assessment** and should not be interpreted as official vessel annotations provided by the original IDRiD dataset.

## Annotation Attribution

The retinal vessel annotations included in this repository were prepared by:

**Dr. Nasir Yasin**
Department of Ophthalmology
Aziz Fatimah Medical and Dental College
Faisalabad, Pakistan

The annotations were prepared for the pathological retinal image evaluation performed as part of the AV-MapNet study.

## Associated Study

**Title:**
*AV-MapNet: Geodesic Vessel Tokenization and Sequential Refinement for Retinal Vessel Segmentation and Artery–Vein Classification*

**Authors:**
Owais Ali, Di Xiao, Nasir Yasin, Jinglan Zhang, and Yuefeng Li

## Recommended Citation

If you use these annotations in your research, please cite the associated AV-MapNet paper.

```bibtex
@article{ali_avmapnet,
  title   = {AV-MapNet: Geodesic Vessel Tokenization and Sequential Refinement for Retinal Vessel Segmentation and Artery--Vein Classification},
  author  = {Ali, Owais and Xiao, Di and Yasin, Nasir and Zhang, Jinglan and Li, Yuefeng},
  year    = {2026}
}
```

The complete journal citation, DOI, volume, and page information should be added after publication.

## Data Usage

These annotations are provided for **academic and research purposes**.

Users of this repository should separately comply with the access, citation, and usage conditions associated with the original IDRiD dataset.

Only the newly prepared/refined vessel annotations are provided here; ownership and distribution conditions for the original retinal images remain governed by the original IDRiD dataset providers.

## Important Note

These annotations are **research reference maps prepared for the AV-MapNet study**. They are not part of the original official IDRiD annotation set and should therefore be referred to as:

> **Refined IDRiD vessel annotations**

or

> **Manually prepared vessel reference maps**

rather than as official IDRiD vessel ground truths.

## Contact

For questions regarding the annotations or the associated AV-MapNet study, please contact the corresponding authors through the contact information provided in the associated publication.

---

We hope that making these annotations publicly available will support reproducibility and further research on retinal vessel segmentation under pathological imaging conditions.
