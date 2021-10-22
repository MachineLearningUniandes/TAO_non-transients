# About the dataset

We compile a total of 3807 transient objects (AGN,BZ,CV,SN and OTHER, located [here](https://github.com/MachineLearningUniandes/TAO_transients).) and 12500 non-transient objects (NON).

| Class | Total Objects |
|:-----:|:-------------:|
|  AGN  |      606      |
|   BZ  |      239      |
|   CV  |      772      |
|   SN  |      1372     |
| OTHER |      818      |
|  NON  |     12500     |


## Non-Transients Objects

For non-Transients objects, you can find in the fits images' headers the next information: 

| Header Dict | Description                                  | Type  |
|-------------|----------------------------------------------|-------|
| CRTS_ID     | Catalina Real-time Transient Survey  ID from was extrated the non-transient object.     | str  |
| RA_(J2000)  | Right Ascension (degrees).                   | str  |
| Dec_(J2000) | Declination (degrees).                       | str  |
| N_Images    | Total number of images for this non-Transient object.     | str  |
| Img_Ref    | Image of reference where was identified the non-transient object.     | str  |

Also, in hdu 1, you can find a table that contains information to identify the images of non-transients by MJD, date, field id, or cutout.

| Table of Content HDU:1 (Table) | Description                                                                | Type |
|-------------------------|-----------------------------------------------------------------------------------|------|
| HDU_Ext                 | Extension number of the image in the fits file.                                   | int  |
| Date                    | Date of observation in YYMMMDD format.                                            | str  |
| MJD                     | Modified Julian Date.                                                             | float  |
| Field_ID                | Field identifier.                                                                 | str  |
| Cutout                  | The cutout matrix location. Each cutout covers an area of ABOUT 5 x 5 arcminutes. | str  |


# How to read the dataset?

An example of how to read the data set is [here](https://github.com/MachineLearningUniandes/TAO_transients/blob/master/data/Read_dataset.ipynb).
