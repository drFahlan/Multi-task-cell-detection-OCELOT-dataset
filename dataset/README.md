[OCELOT dataset](https://lunit-io.github.io/research/ocelot_dataset/) is the dataset that we are using in this research, and is available on the link provided.

# Data acquisition and annotation:
The OCELOT dataset was collected from hundreds of Hematoxylin and Eosin (H&E) stained Whole-Slide-Images (wSIs) available in The Cancer Genome Atlas (TCGA) database. From the slides, extracted 1 to 3 Regions of Interest (RoIs) to become a large FoV. From each large FoV, select 1 RoI inside it with a width of 4 times smaller to become the small FoV pair.

And from the extracted samples, which include large FoVs and their small FoV pair, annotation was performed. A total of 67 board-certified pathologists perform a tissue region annotation on the large FoV and a cell point annotation on the small FoV.

<p align="center">
  <img src="../images/sampel.drawio.png" width="400" alt="Figure 1: A sample from OCELOT dataset">
</p>

<p align="center"><em>Figure 1. A sample from OCELOT dataset</em></p>

# Data description

| Organ         | Train | Val | Test |
|---------------|-------|-----|------|
| bladder       | 82    | 29  | 24   |
| endometrium   | 86    | 29  | 23   |
| head-and-neck | 27    | 9   | 10   |
| kidney        | 122   | 41  | 41   |
| prostate      | 47    | 17  | 16   |
| stomach       | 36    | 12  | 12   |
| **Total**     | 400   | 137 | 126  |
