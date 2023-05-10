# Initializing SSD Disk (Windows)

Youtube Video:

[Fix new SSD not showing up in Windows | EASY | NO DOWNLOADS](https://www.youtube.com/watch?v=pu5IbAlw1Nk)
Note: For only Linux installation, there is no need to initialize SSD.


# Format SSD from prompt (Windows)

Youtube Video:

[Completely format hard drive removing all partitions (including OEM)](https://www.youtube.com/watch?v=6lTrZopRtE8)
Note: For only Linux installation, there is no need to initialize SSD.

# Fans Speed NVIDIA X Server Settings (Linux)

Youtube Video:

[fix manual fan control nvidia driver "Failed to set new Fan Speed" in Ubuntu 22.04](https://www.youtube.com/watch?v=A1QJtteOUz4)

Note: VIM application uses Shift + Enter to type and :+x to save changes.

# 1.- Install Linux Ubuntu

[Installing Ubuntu 20.4 LTS](https://www.youtube.com/watch?v=FAknvXs4M1w)

# 2.- Install NVIDIA GPU drivers

Youtube Video:

[Install Nvidia Driver Ubuntu 20.04 | Linux | Complete Installation & Setup | 100% Working](https://www.youtube.com/watch?v=FAknvXs4M1w)


# 3.- Install Tensorflow

Youtube Video:

[2020, TensorFlow 2.2 NVIDIA GPU (CUDA)/CPU, Keras, & Python 3.7 in Linux Ubuntu](https://www.youtube.com/watch?v=dj-Jntz-74g&t=357s)

Before to proceed with instructions, check the latest compatibility versions of tensorflow through conda

[Tensorflow compatibility chart](https://www.tensorflow.org/install/source)

[tensorflow-gpu Conda Version](https://anaconda.org/anaconda/tensorflow-gpu)

Software versions:

+ **miniconda 3.8**
+ **tensorflow-2.1.0**
+ **phyton 3.7.16**
+ **cuDNN	7.6.5**
+ **CUDA 10.1.243**


1.- Download [Miniconda 3.8](https://docs.conda.io/en/latest/miniconda.html)

2.- Open Terminal and change directory: **cd ./Downloads/**

3.- Install miniconda: **chmod -x ./name-of-file.sh**

4.- Install conda navigator: **conda install anaconda-navigator**
 
 + To open anaconda navigator type: **anaconda-navigator

5.- Install Jupiter Notebook: **conda install -y jupyter**

6.- Create *tensorflow environment* inside conda: **conda create --name tensorflow python=3.7**

7.- Enter the created *tensorflow environment*: **conda activate tensorflow**

8.- Add Jupyter support to the *tensorflow environment*: **conda install -c conda-forge nb_conda**

9.- Install *tensorflow-gpu*: **conda install -c anaconda tensorflow-gpu**

+ *tensorflow-gpu* installs CUDA 10.0 and cuDNN 7.0

10.- Download [toolsTensorflow.yml](https://raw.githubusercontent.com/brainnlabs/SSD-Initialization/main/toolsTensorflow.yml) and paste it inside **miniconda3** folder inside home.

11.- Run the following terminal command: **conda env update --file toolsTensorflow.yml** 

12.- Register your environment to show inside jupyter notebook: **python -m ipykernel install --user --name tensorflow --display-name "Python 3.7 (tensorflow)"**

13.- Testing *tensorflow* environment: **jupyter notebook**

# 4.- Install Pytorch

Youtube Vide:

[How to Install PyTorch on Linux for CPU or GPU - No Driver Install Needed](https://www.youtube.com/watch?v=YTvVxYneu7w)







