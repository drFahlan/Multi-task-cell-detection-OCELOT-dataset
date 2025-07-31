# The Effect of Adding Large Field-of-View (FoV) on the Performance of Tumor Cell Detection: A Case Study on the OCELOT Dataset

##abstract
Following the release of the OCELOT dataset by [1],
 only a few studies analyzed the effect of adding a large FoV on the
 performance of the tumor cell detection model. As a result, the
 strengths and weaknesses of this approach remain underexplored.
 Therefore, in this study, we develop cell detection models that
 utilize both small and large FoV, and analyze the effect of adding
 large FoV on the tumor cell detection model performance. We
 successfully developed the tumor cell detection model that utilizes
 both small FoV and large FoV by integrating a cancer area
 probability map from the tissue segmentation model to the data
 preparation step, and the post-processing step of the cell detection
 pipeline. Furthermore, the analysis of adding a large FoV
 shows an improvement of the cell detection model performance
 across most evaluation metrics, particularly the mF1-score, which
 increased from 0.5724 to 0.6929. In most samples, the addition
 of a large FoV gives a detection performance improvement.
 However, there are cases where the addition of a large FoV did
 not give a significant improvement, such as when both cell classes
 were randomly distributed, or when the cancer area probability
 map was inaccurate. Hopefully, these findings can give valuable
 information for future research that involves multi-scale cell
 detection to decide and build a cell detection approach.
