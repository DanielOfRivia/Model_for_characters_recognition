## Usage instructions
To use the model install all packages from `requirements.txt` and run the script with the:
py inference.py --input `your data folder`
## Author information
Made by Danylo Ustymenko on 21 May 2023
## Data used
Emnist datapackage[https://pypi.org/project/emnist/] was used. The digits and letters datasets were combined into one. The images have the size of (28, 28, 1).
## Methods and ideas 
 The data pipelines which normalize the data and optimize training time were used. The model consists of convolutional layers with ReLU activation function and dense layers. The early stopping was used to avoid overfitting. The images passed to the `inference.py` are resized using bilinear interpoplatio to the size of 28x28. 
## Challenges faced
First, I wanted to use NIST dataset that contained images of size 128x128. I downloaded it, but my computational powers do not allow me to train any kind of models, so I decided to use the google colab for training. However, uploading data to colab or google drive was really slow(maybe the reason is my hardware, but overall it would have taken 100 hours appriximately based on the google drive's information), that's why I used the package as an alternetive. 
As further improvement for this model spatial transformers may be used. Experiments with the model architecture should give improvements in performance as well.
