#### Introduction
This repository contains a school project focused on coloring black-and-white movies with convolutional neural networks. It consists of two parts:

* report.pdf, which contains a survey of this topic.
* main.ipynb, which contains an implementation of the paper "Pixel-level Semantics Guided Image Colorization" by Jiaojiao Zhao, Li Liu, Cees G.M. Snoek, Jungong Han and Ling Shao.

#### Requirements
Tensorflow 2.0 and various machine learning libraries.

#### Installation
For example, with [conda](https://docs.conda.io/en/latest/) run
````
conda install tensorflow-gpu numpy scipy scikit-image scikit-learn matplotlib jupyter
````
or
````
conda env create -f environment.yml
````

#### Usage
There is only a single notebook with everything in it, so run
````
jupyter notebook main.ipynb
````
with possibly also
````
conda activate MVI
````
beforehand.

### Additional files
PASCAL VOC2012 dataset for training: \
http://host.robots.ox.ac.uk/pascal/VOC/voc2012/VOCtrainval_11-May-2012.tar \
Command for unpacking:
````
tar -xvf VOCtrainval_11-May-2012.tar -C data
````
That is, the folder structure should either be data/VOCdevkit/, or the filepaths in the notebook should be changed.

Mirror: \
http://pjreddie.com/media/files/VOCtrainval_11-May-2012.tar

Weights for the colorization branch initialized with k-means: \
https://drive.google.com/file/d/1ohX4aMzp-QwENu42Q1nLviWBUwXBsfk7/view?usp=sharing

Pretrained weights for the colorization branch: \
https://drive.google.com/file/d/1D--ZfxCdGdSk8vDJGopEQwgCi_wdsKOC/view?usp=sharing

8 short comparison videos for the networks by Zhang et al. / Jason Antic / Chenyang et al.: \
https://drive.google.com/file/d/1TBHowKLJJqGX1aAoRMkKqD54ICPQ3fsh/view?usp=sharing
