## Simple Blackbox Attack

all the required packages from the requirements.txt are needed to be installed.

# 1. whitebox.ipynb
This notebook can be executed, the data is fetched over the web by the python notebook.
To try the whitebox attack, a CNN based Neural Network model has been trained over the Mnist dataset which generates about 98% validation accuracy. Later this model has been used to attack on.

# 2. subset_target.ipynb
this notebook runs targeted attack on the subset of imagenet dataset, with 'mobilenet_v2' pre-trained model.
to run this notebook, two pickle files will be required to be present in the same directory: labels.pkl, idx

` testset = dset.ImageFolder('/content/drive/MyDrive/SMAI_proj/subset/val', IMAGENET_TRANSFORM)`
the path to the images directory has to be changed in the notebook before running the notebook.

` attacker = Simba('mobilenet_v2')`
here the attacked model can be changed

` class Simba:`
`  def __init__(self, model_name, epsilon = 0.1):`
here the epsilon value of the attack can be changed

# 3. subset_untarget.ipynb
this notebook runs un-targeted attack on the subset of imagenet dataset, with 'mobilenet_v2' pre-trained model.
to run this notebook, two pickle files will be required to be present in the same directory: labels.pkl, idx

` testset = dset.ImageFolder('/content/drive/MyDrive/SMAI_proj/subset/val', IMAGENET_TRANSFORM)`
the path to the images directory has to be changed in the notebook before running the notebook.

` attacker = Simba('mobilenet_v2')`
here the attacked model can be changed

` class Simba:`
`  def __init__(self, model_name, epsilon = 0.1):`
here the epsilon value of the attack can be changed

# 4. tinyimage_target.ipynb
this notebook runs targeted attack on the subset of tinyimagenet dataset, with 'mobilenet_v2' pre-trained model.
to run this notebook, three pickle files will be required to be present in the same directory: labels.pkl, idx, mapping

` testset = dset.ImageFolder('/content/drive/MyDrive/SMAI_proj/Imagenet16v2/val', IMAGENET_TRANSFORM)`
the path to the images directory has to be changed in the notebook before running the notebook.

` attacker = Simba('mobilenet_v2')`
here the attacked model can be changed

` class Simba:`
`  def __init__(self, model_name, epsilon = 0.1):`
here the epsilon value of the attack can be changed

# 5. tinyimage_untarget.ipynb
this notebook runs un-targeted attack on the subset of tinyimagenet dataset, with 'mobilenet_v2' pre-trained model.
to run this notebook, three pickle files will be required to be present in the same directory: labels.pkl, idx, mapping

` testset = dset.ImageFolder('/content/drive/MyDrive/SMAI_proj/Imagenet16v2/val', IMAGENET_TRANSFORM)`
the path to the images directory has to be changed in the notebook before running the notebook.

` attacker = Simba('mobilenet_v2')`
here the attacked model can be changed

` class Simba:`
`  def __init__(self, model_name, epsilon = 0.1):`
here the epsilon value of the attack can be changed

# 6. targetV2.ipynb
in this notebook we have tried various strategies to reduce the number of queries for targeted attackes uing the subset_imagenet dataset
