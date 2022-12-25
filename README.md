# Understanding Classical Music with Machine Learning

* Using machine learning on the [MusicNet](https://paperswithcode.com/dataset/musicnet) dataset to tackle the problem of pitch detection. 
* Given a 0.3-second .wav audio snippet, our model detects which of 45 possible pitches is playing. 
* Performed data preprocessing, transformed data using the spectral Q-transform, and implemented a variety of models (logistic regression, CNNs, RNNs, PCA) on the data. 
* Evaluated models using precision, recall, and AUC metrics. Our best model (PCA)  significantly beat our baseline, with an AUC of 0.936.

Made by Ayanav Roy & Xander Uyttendaele for CIS 520: Machine Learning, at the University of Pennsylvania.

## Overview of Repository
* [520_Final_Project_Report.pdf](520_Final_Project_Report.pdf): Final report containing (a) background on music information retrieval, (b) our steps for data preprocessing, (c) our models and their respective accuracies, (d) our conclusions and possible extensions of this work. 
* [Walkthrough_Jupyter_Notebook.ipynb](Walkthrough_Jupyter_Notebook.ipynb): Notebook which explains the MusicNet dataset and our best model (PCA) for note recognition.
* [Data_Loading_Final.ipynb](<Data Loading Final.ipynb>): Loading MusicNet into repository.
* Our models:
  * [Baseline Model.ipynb](<Baseline Model.ipynb>): Naive model, which just uses the Q-transform frequency data directly. 
  * [TrainLogisticRaw.ipynb](TrainLogisticRaw.ipynb): Logistic regression on a portion of the raw data. 
  * [LogisticafterQTransform.ipynb](LogisticafterQTransform.ipynb): Logistic regression on our Q-transform spectral data. 
  * [CNNafterQTransform.ipynb](CNNafterQTransform.ipynb): Convolution neural network on our Q-transform spectral data.
  * [RNNafterQTransform.ipynb](RNNafterQTransform.ipynb): Recurrent neural network on our Q-transform spectral data.
  * [PCA.ipynb](PCA.ipynb): Principal component analysis on our Q-transform spectral data.