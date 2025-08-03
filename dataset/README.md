[OCELOT dataset](https://lunit-io.github.io/research/ocelot_dataset/) is the dataset that we are using in this research, and is available on the link provided.

# Data acquisition and annotation:
The OCELOT dataset was collected from hundreds of Hematoxylin and Eosin (H&E) stained Whole-Slide-Images (wSIs) available in The Cancer Genome Atlas (TCGA) database. From the slides, extracted 1 to 3 Regions of Interest (RoIs) to become a large FoV. From each large FoV, select 1 RoI inside it with a width of 4 times smaller to become the small FoV pair.

And from the extracted samples, which include large FoVs and their small FoV pair, annotation was performed. A total of 67 board-certified pathologists perform a tissue region annotation on the large FoV and a cell point annotation on the small FoV.

<p align="center">
  <img src="../images/sampel.drawio.png" width="400" >
</p>

<p align="center"><em>Figure 1. A sample from OCELOT dataset</em></p>

# Data description

From the collected data, we acquired a total of 663 samples with the distribution given in the table below

<div align="center">
<p><em>Table 1: OCELOT dataset sample distribution by organ</em></p>
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

</div>

Each sample of the OCELOT dataset consists of: a large FoV with its tissue region annotation, and a small FoV with cell point annotation. see Figure 1.

large FoV: 
- Image resolution around 0.77 Microns-per-Pixel (MPP)
- Tissue region annotation in .png file with 3 classes: non-cancer area (1), cancer area (2), unknown (255).

<div align="center">
<p><em>Table 2: Tissue region annotation class distribution</em></p>

| Pixel Intensity | Train                    | Val                      | Test                     |
|------------------|--------------------------|---------------------------|---------------------------|
| 1                | 235409146 (56.13%)       | 79082000 (55.05%)         | 67427541 (51.03%)         |
| 2                | 166661770 (39.74%)       | 57805340 (40.24%)         | 58590757 (44.35%)         |
| 255              | 17359484 (4.14%)         | 6767572 (4.71%)           | 6102278 (4.62%)           |

</div>


small FoV:
- Image resolution around 0.19 MPP
- Cell point annotation in a .csv file with 2 classes: non-tumor cells (1), and tumor cells (2)

<div align="center">

<p><em>Table 3: Cell point annotation class distribution</em></p>

<table>
  <thead>
    <tr>
      <th>Organ</th>
      <th>train</th>
      <th>val</th>
      <th>test</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>bladder</td>
      <td>4888 | 7713<br>(7.4% | 11.7%)</td>
      <td>1706 | 2259<br>(6.9% | 9.1%)</td>
      <td>1392 | 2819<br>(6.2% | 12.5%)</td>
    </tr>
    <tr>
      <td>kidney</td>
      <td>3982 | 13672<br>(6.0% | 20.8%)</td>
      <td>1238 | 6109<br>(5.0% | 24.7%)</td>
      <td>1602 | 3209<br>(7.1% | 14.3%)</td>
    </tr>
    <tr>
      <td>endometrium</td>
      <td>6634 | 12591<br>(10.1% | 19.1%)</td>
      <td>2522 | 4874<br>(10.2% | 19.7%)</td>
      <td>2883 | 3472<br>(12.8% | 15.4%)</td>
    </tr>
    <tr>
      <td>prostate</td>
      <td>3060 | 3919<br>(4.6% | 6.0%)</td>
      <td>1259 | 1874<br>(5.1% | 7.6%)</td>
      <td>1590 | 1107<br>(6.7% | 4.9%)</td>
    </tr>
    <tr>
      <td>stomach</td>
      <td>2743 | 2169<br>(4.2% | 3.3%)</td>
      <td>1177 | 78<br>(4.8% | <span style="color:red;"><strong>0.3%</strong></span>)</td>
      <td>1079 | 918<br>(4.8% | 4.1%)</td>
    </tr>
    <tr>
      <td>head-and-neck</td>
      <td>2025 | 2441<br>(3.1% | 3.7%)</td>
      <td>498 | 1118<br>(<span style="color:red;"><strong>2.0%</strong></span> | 4.5%)</td>
      <td>1138 | 1349<br>(5.1% | 6.0%)</td>
    </tr>
    <tr>
      <td><strong>Total</strong></td>
      <td><strong>23332 | 42505</strong><br>(35.4% | 64.6%)</td>
      <td><strong>8400 | 16312</strong><br>(34.0% | 66.0%)</td>
      <td><strong>9603 | 12874</strong><br>(42.7% | 57.3%)</td>
    </tr>
  </tbody>
</table>

</div>

# Data exploration
We conduct a data exploration to get to know the RoI or the segmentation target characteristics and challenges.



