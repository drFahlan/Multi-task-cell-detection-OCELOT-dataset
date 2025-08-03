[OCELOT dataset](https://lunit-io.github.io/research/ocelot_dataset/) is the dataset that we are using in this research, and is available on the link provided.

# Data acquisition and annotation:
The OCELOT dataset was collected from hundreds of Hematoxylin and Eosin (H&E) stained Whole-Slide-Images (wSIs) available in The Cancer Genome Atlas (TCGA) database. From the slides, extracted 1 to 3 Regions of Interest (RoIs) to become a large FoV. From each large FoV, select 1 RoI inside it with a width of 4 times smaller to become the small FoV pair.

And from the extracted samples, which include large FoVs and their small FoV pair, annotation was performed. A total of 67 board-certified pathologists perform a tissue region annotation on the large FoV and a cell point annotation on the small FoV.

<p align="center">
  <img src="../images/sampel.drawio.png" width="400" alt="Figure 1: A sample from OCELOT dataset">
</p>

<p align="center"><em>Figure 1. A sample from OCELOT dataset</em></p>

# Data description

From the collected data, we acquired a total of 663 samples with the distribution given in the table below

<div align="center">

<table>
  <thead>
    <tr>
      <th>Organ</th>
      <th>Train</th>
      <th>Val</th>
      <th>Test</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>bladder</td><td>82</td><td>29</td><td>24</td></tr>
    <tr><td>endometrium</td><td>86</td><td>29</td><td>23</td></tr>
    <tr><td>head-and-neck</td><td>27</td><td>9</td><td>10</td></tr>
    <tr><td>kidney</td><td>122</td><td>41</td><td>41</td></tr>
    <tr><td>prostate</td><td>47</td><td>17</td><td>16</td></tr>
    <tr><td>stomach</td><td>36</td><td>12</td><td>12</td></tr>
    <tr><td><strong>Total</strong></td><td><strong>400</strong></td><td><strong>137</strong></td><td><strong>126</strong></td></tr>
  </tbody>
</table>

<p><em>Table 1: OCELOT dataset sample distribution by organ</em></p>

</div>

Each sample of the OCELOT dataset consists of: a large FoV with its tissue region annotation, and a small FoV with cell point annotation. see Figure 1.

large FoV: 
- Image resolution around 0.77 Microns-per-Pixel (MPP)
- Tissue region annotation in .png file with 3 classes: non-cancer area (1), cancer area (2), unknown (255).

<div align="center">

| Pixel Intensity | Train                    | Val                      | Test                     |
|------------------|--------------------------|---------------------------|---------------------------|
| 1                | 235409146 (56.13%)       | 79082000 (55.05%)         | 67427541 (51.03%)         |
| 2                | 166661770 (39.74%)       | 57805340 (40.24%)         | 58590757 (44.35%)         |
| 255              | 17359484 (4.14%)         | 6767572 (4.71%)           | 6102278 (4.62%)           |


</div>


small FoV:
- Image resolution around 0.19 MPP
- Cell point annotation in a .csv file with 2 classes: non-tumor cells (1), and tumor cells (2)
