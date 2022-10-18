## Caltech Pedestrian Dataset images-Converter

This repository is based on [caltech-pedestrian-dataset-converter](https://github.com/mitmul/caltech-pedestrian-dataset-converter) repository. It is impemented to prepare the images of caltech pedestrian dataset specifically for [Pedestron](https://github.com/hasanirtiza/Pedestron) project.

### Download Caltech Datasets 
1- Download caltech pedestrian videos from [caltech-pedestrians](https://drive.google.com/drive/folders/1cnQHqa8BkVx90-6-UojHnbMB0WhksSRc).

2- The annotation files (train.json and test.json) is provided by [Pedestron](https://github.com/hasanirtiza/Pedestron/tree/master/datasets/Caltech) repository.

### Virtualenv 
git clone https://github.com/Nazila-H/Caltech-images-convertor.git<br />
cd Caltech-images-convertor<br />
conda create -name caltech python==3.8<br />
conda activate caltech<br />
pip install -r requirements.txt<br />

### How to ... 

`$ python convert_seqs.py` converts .seq video files to .jpg frames that they are ready to use for Pedestron project. They will end up in the `images` folder.

### Folder structure 
```shell   
data/
|__images/   # 128419 train-images
   |__set00_V000_I00000.jpg 
   |__set00_V000_I00001.jpg
   |__ ...
   |__set05_V012_I01706.jpg
or   
|__images/   # 121465 test_images
   |__set06_V000_I00000.jpg
   |__set06_V000_I00001.jpg
   |__ ...
   |__set10_V011_I01733.jpg

data/   
|__set00/  # for training 
|__set01/
|__set02/
|__set03/
|__set04/
|__set05/ 
or 
|__set06/  # for test 
|__set07/
|__set08/
|__set09/
|__set10/

```

