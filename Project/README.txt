This project aims to generate music using two models trained on different combinations of datasets. To ensure the code runs as intended, follow the directions below:

1. Upload to and run the source code in Google Colab.

2. Create a copy of the following folder in your Google Drive. This contains the EDM Beatport Key Dataset, converted into MIDI files. The Colabcode will then ask for permission to access this folder when the third block of code is run.

https://drive.google.com/drive/folders/1VPhpF4uI4ZXB6mtJHSmdvLoledghHxQJ?usp=sharing


The models are trained on either MAESTRO or Beatport. To switch the dataset that the models are trained on, replace line 67 in the second blockunder "MusicVAE" and line 77 in the first block under "LSTM Model" with the below lines according to your preference:

train_ds_EDM,

train_ds_MAESTRO,

After training, the models generate music when given an input. To change the dataset from which the inputs originate, change input_notes_EDM to input_notes_MAESTRO or vice versa to match the training datasets of the models on lines 101 and 102 in the first block under "Generate Music."

The sample files fed into the models may be changed as well. This can be adjusted by changing the number on line 82, also in the first block under "Generate Music."
