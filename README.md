# NNZ
Predicting redshifts of galaxies using neural networks! 

The photo-z_MLP notebook trains a Multi-Layer Perception neural network model on SDSS DR8 data to predict photometric redshifts. 

Want to run photo-z_MLP? Here's what you need to do!
1. Download the data required for photo-z_MLP from Zenodo: https://zenodo.org/records/11040878
2. Change the data_dir variable in common.py to the directory where the data is located.
3. You may need to change the file path in for the loadSdssSpecSample() function in sdss_utils.py to where the data is located. 

Contributions:
common.py, obs_utils.py, and sdss_utils.py were created by Benedikt Diemer (https://github.com/benediktdiemer). 
photo-z_MLP.ipynb and this README file were created by Kylie Yui Dan (https://github.com/kykyelric). 
