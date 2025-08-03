[OCELOT dataset](https://lunit-io.github.io/research/ocelot_dataset/) is the dataset that we are using in this research, and is available on the link provided.

# Data acquisition and annotation:
The OCELOT dataset was collected from hundreds of Hematoxylin and Eosin (H&E) stained Whole-Slide-Images (wSIs) available in The Cancer Genome Atlas (TCGA) database. From the slides, extracted 1 to 3 Regions of Interest (RoIs) to become a large FoV. From each large FoV, select 1 RoI inside it with a width of 4 times smaller to become the small FoV pair.

And from the extracted samples, which include large FoVs and their small FoV pair, annotation was performed. A total of 67 board-certified pathologists perform a tissue region annotation on the large FoV and a cell point annotation on the small FoV.

<p align="center">
  <img src="../images/sampel.drawio.png" width="400" alt="Figure 1: A sample from OCELOT dataset">
</p>

<p align="center"><em>Figure 1. A sample from OCELOT dataset</em></p>

# Data description

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

<p><em>Tabel sebaran sampel <strong>OCELOT dataset</strong> pada tiap organ</em></p>

</div>

