# NNZ
Predicting redshifts of galaxies using neural networks! 

The photo-z_MLP notebook trains a Multi-Layer Perception neural network model on SDSS DR8 data to predict photometric redshifts. 

Want to run photo-z_MLP? Here's what you need to do!
1. Download the data required for photo-z_MLP from Zenodo: https://zenodo.org/records/11040878
2. Change the data_dir variable in common.py to the directory where the data is located.
3. You may need to change the file path in for the loadSdssSpecSample() function in sdss_utils.py to where the data is located.
4. If you'd like, you can create a conda environment with all the dependencies using the environment.yml file. You will need to add PyTorch manually afterward (conda install pytorch-nightly::pytorch -c pytorch-nightly) and also Colossus (pip install colossus).  

The spec-z_CNN notebook trains a Convolutional Neural Network model on SDSS DR8 data to predict photometric redshifts. Gathering the data for this model was a pain, so I put them in .npy files. 

Want to run spec-z_CNN? Here's what you need to do!
1. Download the spectra_001_3.npy file with the spectral data from my Google Drive: https://drive.google.com/file/d/1bjd2Mky0_ifAgtcY32CDq1VXlrcWLmRk/view?usp=share_link
2. Put the spectra_001_3.npy file in the same directory that you downloaded this repo.
3. If you'd like to run it on your Mac's GPU, make sure you have the proper version of PyTorch installed (Preview (Nightly) build). You may need to have a specific Python version for this. 3.8 worked for me. If you'd like, you can create a conda environment using the environment.yml file in this repo, then add PyTorch using this command: conda install pytorch-nightly::pytorch -c pytorch-nightly 

Contributions:
common.py, obs_utils.py, and sdss_utils.py were created by Benedikt Diemer (https://github.com/benediktdiemer). 
All other files were created by Kylie Yui Dan (https://github.com/kykyelric). 
