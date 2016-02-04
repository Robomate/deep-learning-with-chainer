## Deep Learning with Chainer  

* Deep Convolutional Neural Networks with Chainer (Python 2 or 3)  
http://nbviewer.jupyter.org/github/masaki-y/Deep-Learning-with-Chainer/blob/master/Chainer-CNN-CIFAR10.ipynb

* Fine-tuning Caffemodel with Chainer (Python 2)  
http://nbviewer.jupyter.org/github/masaki-y/Deep-Learning-with-Chainer/blob/master/Chainer-Fine-Tuning.ipynb

## Dependencies
Python 2 or 3, [chainer](http://chainer.org/) (v1.5), jupyter, matplotlib, scikit-image, progressbar2  
If you don't have these python packages, I recommend you install them by "pip install".  
The chainer "CaffeFunction" class to load caffemodel only supports python 2.  

## Usage
Open a Jupyter's session in your browser.  
```sh
$ jupyter notebook Chainer-CNN-CIFAR10.ipynb
```
Then select the `Run All` from the `cell` in the top menu.  

If you use a GPU, set the GPU ID to `gpu` in the jupyter notebook.
Chainer will switch automatically to GPU mode.
```py
gpu = -1 # gpu device ID (cpu if this negative)
xp = cuda.cupy if gpu >= 0 else np  
```
