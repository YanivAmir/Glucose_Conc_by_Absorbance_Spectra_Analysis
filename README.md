## Prediction of Glocuse Concetrations using midIR Absorbance Spectra and RandomForest Regressor

A dataset of spectra absorbance in the midIR range with known glucose concentrations will be used to train a predictive model. The dataset contains glucose concentrations ranging from 80 to 195 mg/dl. Each concentration contains 80 repeated measurements of broad spectrum absorbance in the 950 to 1200 cm^-1 wavenumber range at 1 cm^-1 resolution.

RandomForestRegressor will be used for initial model training. The random forest built-in feature importance calculations, along with feature permutation importance calculations, will be used to identify the most important absorbance region/s for determining glucose concentrations and the laser's optimal wavenumber width.

Finally, the ability of the absorbance spectra provided to be used to predict glucose concentrations in phantom skin models will be discussed.

#### Task 1: Perform predictive modeling and predict glucose concentrations from solution absorbance spectra. Performance is reported in terms of Mean Absolute Relative Difference (MARD).

#### Task 2: When lasers are manufactured, the trade-off between the number of wavenumbers they span and their cost must be considered. Does the predictive performance change with the number of wavenumbers available? What is the minimum number you would recommend?

#### Task 3: Evaluating the ability of the device to capture glucose information on a new type of skin model in the lab.


#### Sample Results:

![image](https://github.com/user-attachments/assets/6f76c09e-5448-4030-84fc-e953fb3cc32a)

Both feature importance calculations agree that the region of 1025-1040 cm^-1 is the most important region in the spectrum for predicting glucose concentrations in solution. The two feature importance methods also agree on the top other regions, though they vary in their relative importance compared to the 1025-1040 cm^-1 region.

![image](https://github.com/user-attachments/assets/a5131103-bd59-4fc7-a7bc-4a2a9cb21ac4)

Relating to the 2nd Task, the optimal laser position is at the 1035 cm^-1 wavenumber (compare the MARD scores of other 4 single laser results). This result is not surprising given the results of the feature importance calculations, and further substantiates the results so far.

![image](https://github.com/user-attachments/assets/68d4cc49-b742-4761-8c95-430af22a9995)

Skin models absorbance spectra in the midIR range
