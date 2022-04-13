Codes in this repo has been written by Tay Hui Yi for SP3176 - The Universe, under Prof. Lim Zhi Han.

The poster was done in collaboration with Muhammad B Salman Sabeer and Shao Nandi.

# Introduction to Solar Jets 
Solar jets are narrow ejections of plasma in the solar atmosphere **(Figure 1)**, which arise from a sudden energy release and mass eruption in the solar atmosphere via the reconfiguration of the magnetic field lines at the jet base **(Figure 2)**. Solar jets are major factors that contribute to the mass and energy input in the upper solar atmosphere and solar wind. The atmospheric image taken from the Sun can be divided into active regions mainly caused by solar jets and quiet areas without them (Tsiropoula et al., 2012).

<img src="https://github.com/TayHuiYi/Solar-Jet-Hunters/blob/cfe7f77eeffa0228f1b0d7019e4920e3d3b018b6/SolarJetImage.jpeg" width="400" height="220">

**Figure 1.** *Solar Jet on the sides of the Sun (Generated using JHelioviewer).*

<img src="https://cfn-live-content-bucket-iop-org.s3.amazonaws.com/journals/0004-637X/883/1/104/revision1/apjab3a4df6_lr.jpg?AWSAccessKeyId=AKIAYDKQL6LTV7YY2HIK&Expires=1650472894&Signature=OfQvZyOG%2BUzqpBu61%2FToDxH9Rc0%3D" width="400" height="220">

**Figure 2.** *Schematic depiction of solar jet formation (Shen et al., 2019).*

# Research Question and Objective
The objective of this study is to investigate the atmospheric activity of the Sun via solar jet observations from the Earth. Solar jet energy outputs are mainly measured from their X-ray radiation intensities based on the constitution of solar jets (Friedman, 1963). The project aims to reveal the atmospheric solar activity on the side of the Sun facing Earth via the image analysis of solar jets for a specified time period. To support the study, it is shown that the atmospheric solar activity corresponds with the variation of X- ray intensity measured from the same side of the Sun within the same time period. As such, a potential method to study solar atmospheric activity may be determined by the occurrence of solar jets and its density on the Sun.

# Data collection
1. Data was collected from 1st Dec 2010 to 31st July 2011.
2. Videos are accessible on the JHelioviewer software which collates and compresses the raw data generated by the Atmospheric Imaging Assembly instrument at 171Å (AIA 171Å) from the Solar Dynamic Observatory (SDO).
3. High resolution,stereoscopic videos were taken as the projection of the Sun’s hemisphere on the focal plane of the telescope.
4. A total of 8 videos were taken, where each video represents 1 month in the specified time period.
5. Variation in X-ray intensity of the Sun during the specified time period was obtained by the X-ray Sensor A on the GOES satellite (GOES-XRSA).

# Description of the Program
The Python notebook aims to analyse the relative ratio of active regions on the sun as compared to the whole area of the sun. The algorithm is elucidated as follows. 

1. Splitting of videos into its individual frames for image analysis.
2. Image thresholding is conducted to obtain the respective regions, namely the active region of the sun and the whole area of the sun. 
3. Calculate solar atmospheric activity using the given formula: 
    ```javascript
       Solar Atmospheric Activity = Area of Active Region/Area of the whole Sun
    ```
4. Remove glitchy frames.  
5. Observe the change in solar atmospheric activity over time.

# Graph of Atmospheric Solar Activity against Time 
<img src="https://github.com/TayHuiYi/Solar-Jet-Hunters/blob/27efde9081ad8d301fc44e2ce01a8a49cff23403/FinalFigure.png" width="400" height="250">

## Additional Information
- Videos used in the Python notebook for image analysis can be found in "Solar Jet Videos.zip"
- A summary poster of the study can be found in "Poster.pdf"

## References 
Friedman, H., Solar X-ray emission, in The Solar Corona, edited by J. W. Evans, pp. 45-58, Academic Press, New York and London, 1963.

Shen, Y., Qu, Z., Yuan, D., Chen, H., Duan, Y., Zhou, C., Tang, Z., Huang, J., & Liu, Y. (2019). Stereoscopic Observations of an Erupting Mini-filament-    driven Two-sided-loop Jet and the Applications for Diagnosing a Filament Magnetic Field. The Astrophysical Journal, 883(1), 104. https://doi.org/10.3847/1538-4357/ab3a4d

Tsiropoula, G., Tziotziou, K., Kontogiannis, I., Madjarska, M. S., Doyle, J. G., & Suematsu, Y. (2012). Solar Fine-Scale Structures. I. Spicules and Other Small-Scale, Jet-Like Events at the Chromospheric Level: Observations and Physical Parameters. Space Science Reviews, 169(1), 181-244. https://doi.org/10.1007/s11214-012-9920-2
