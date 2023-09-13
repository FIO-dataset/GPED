# Introduction
This SAR ship dataset was created using 94 SAR images, which contains 44 Chinese Gaofen-3 images, 27 RADARSAT-2 images, 3 Sentinel-1A images, and 20 TerraSAR-X images. It includes 1557 ship slices with multiple polarization modes and different resolutions, including 810 cargo ships, 505 tankers, and 242 container ships. All ship slices were saved as single-precision floating-point amplitude SAR images. It can be used to evaluate the generalization performance of ship recognition algorithms.

The dataset's construction process is described in detail in the paper [Evaluation and Improvement of Generalization Performance of SAR Ship Recognition Algorithms](https://ieeexplore.ieee.org/document/9927347), which is briefly described below:
1.	Each SAR image was cropped into ship slices of suitable size. Due to the difference in the resolution of the SAR images from distinct data sources, the size of the ship slices ranged from 50×50 pixels to 200×200 pixels. All ship slices are saved in JPEG format after quantization processing.
2.	For each SAR image, the corresponding AIS messages from the same zone were retrieved in a 30-minute window centered on the SAR acquisition time.
3.	Linear interpolation and extrapolation processes were performed to unify the temporal and spatial positions of the AIS data with SAR images. Then, we obtained 2441 ship slices and their corresponding AIS data.
4.	Based on AIS data, The LabelImg tool was used to generate label of ship slices. The annotation of ships was stored in XML format. Finally, the corresponding labels for each ship slice are obtained.

## Cite as

**If you feel this dataset is useful, please cite as the following format.**

C. Zhang, X. Zhang, J. Zhang, et al., "Evaluation and Improvement of Generalization Performance of SAR Ship Recognition Algorithms," in IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, doi: 10.1109/JSTARS.2022.3216623.


## Contact

Please contact us if you have any questions: xi.zhang@fio.org.cn (Prof. Zhang).
