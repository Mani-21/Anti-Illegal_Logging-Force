# Anti-Illegal_Logging-Force
Machine learning based audio identifying model.Reports Rangers if any suspicious sounds heard.
# Dataset
The ESC dataset is a collection of short environmental recordings available in a unified format (5-second-long clips, 44.1 kHz, single channel, Ogg Vorbis compressed @ 192 kbit/s).<br/>
ESC-10: a labeled set of 400 environmental recordings (10 classes, 40 clips per class) (this is a subset of ESC-50 - created initialy as a proof-of-concept/standardized selection of easy recordings),<br/>
https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YDEPUT<br/>
https://github.com/karolpiczak/ESC-50
# Dependencies
=>Python
=>Keras
=>Librosa
=>scikit-learn
=>Tensor-flow
# Set-up
1.Download all the files.\n<br/>
2.Combine folders 001 to 009 and name the folder as dataset.<br/>
3.A sample wav file for each class has been generated and kept within sample_wav folder for reference.<br/>
4.To visualize the waveform in the form of a plot. <br/>
python plot_data.py -o "dataset/001 - Dog bark/1-30226-A.ogg"<br/>
5.To train and classify, execute main.py as<br/>
python main.py cnn  // for training CNN<br/>
python main.py mlp  // for training MLP<br/>
6.Once training is done, the trained models are automatically saved in h5 format.<br/>
