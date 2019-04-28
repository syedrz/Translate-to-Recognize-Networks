# Translate-to-Recognize Networks

Pytorch implementations of Translate-to-Recognize Networks for RGB-D Scene Recognition (CVPR 2019).

![blockchain](images/framework.jpg)
![blockchain](images/gen.jpg)
## Usage
1. Download Reset18 pre-trained on [Places dataset](https://github.com/CSAILVision/places365) if necessary.  
2. Data processing.  
   * We use ImageFolder format, i.e., [class1/images.., class2/images..], to store the data, 
use ***util.splitimages.py*** to help change the format if neccessary.
   * Use ***util.conc_modalities.py*** to concatenate each paired RGB and depth images to one image for more efficient data loading.
3. Configuration.  
Almost all the settings of experiments are configurable by the files in the ***config*** package.
4. Train.  
`python train.py`

## Development Environment
* NVIDIA TITAN XP
* cuda 9.0
* python 3.6.5
* pytorch 0.4.1
* torchvision 0.2.1
* tensorboardX


