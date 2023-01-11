# PyMCR_wrapper
wrapper for PyMCR including SVD for initial guesses

# Requierd packages
Requires installation of pymcr (and numpy, matplotlib and scipy)
https://pypi.org/project/pyMCR/
Should be just pip install pymcr or python -m pip install pymcr

# starting out
When you download this repository by clicking code -> download zip and run it without changing things it should do MCR on a test data set
this way you can see if everything works. Then you can try to change the input of dat in the first cell. Make sure the format of the data is the same!
It should just have on the x-axis the intensities for different wavelength/raman shift values and on the y-axis difference spectra in time. Like:

![image](https://user-images.githubusercontent.com/60261797/211803037-1d3df785-d1b7-4318-acef-68d1be20f103.png)

# small summary of MCR
In essence MCR aims to reduce the data into component spectra and how these spectra change in time (traces). PyMCR requires guess spectra and traces, which are made using singular value decomposition. 

![kin_1h_processesResiduals](https://user-images.githubusercontent.com/60261797/211803866-b9945a52-b038-4f22-8b0f-e29d58748509.png)

# future idea
-Do different N component calculations in parallel.
-More advanced guesses
-non notebook version
