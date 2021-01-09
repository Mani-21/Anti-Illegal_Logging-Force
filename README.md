# Anti-Illegal_Logging-Force
Machine learning based audio identifying model.Reports Rangers if any suspicious sounds heard.
# Dataset
The ESC dataset is a collection of short environmental recordings available in a unified format (5-second-long clips, 44.1 kHz, single channel, Ogg Vorbis compressed @ 192 kbit/s).
ESC-10: a labeled set of 400 environmental recordings (10 classes, 40 clips per class) (this is a subset of ESC-50 - created initialy as a proof-of-concept/standardized selection of easy recordings),
https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YDEPUT
https://github.com/karolpiczak/ESC-50
# Dependencies
=>Python
=>Keras
=>Librosa
=>scikit-learn
=>Tensor-flow
# Set-up
1.Download all the files.\n
2.Combine folders 001 to 009 and name the folder as dataset.\n
3.A sample wav file for each class has been generated and kept within sample_wav folder for reference.\n
4.To visualize the waveform in the form of a plot. \n
python plot_data.py -o "dataset/001 - Dog bark/1-30226-A.ogg"\n
5.To train and classify, execute main.py as\n
python main.py cnn  // for training CNN\n
python main.py mlp  // for training MLP\n
6.Once training is done, the trained models are automatically saved in h5 format.\n
