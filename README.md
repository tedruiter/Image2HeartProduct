# Image to Heart 


## Introduction
The goal of this project is to automatically segment the heart of a patient. This is done by training a fully convolutional network on labeled MRI scans of the heart.  


## Setting up project
### Virtual environment

**Creating a virtual environment**

To use this code you first have to make a virtual environment in the folder named 'Image2HeartProduct'. Make sure to name it venv (will be done by default) so git knows to ignore it. The command for creating a virtual environment is:

```
py -m venv venv
```



**Activating the virtual environment** 



**Downloading the packages**

In the 'Image2HeartProduct' folder you will find a 'requirements.txt' file. These are the packages required to run the code except for Pytorch. To download PyTorch you can check there <a href="https://pytorch.org/get-started/locally/">Website</a>. To automatically download the packages you can run the command (make sure the terminal is running in the folder 'Image2HeartProduct')

```
pip install -r requirements.txt
```

For further information about creating a virtual environment you can look at some tutorials or the python documentation.

**Pretrained weights**
The weights file is not included in this repository due to its size. To get the weights you can either train it yourself or send an email to request them. 

## Running the model

**Training the model**

After setting up the project you can train the model using 'train_model.py' within the folder 'Code/Model'. The current parameters work the best, but if you want to edit them you can find them in the main function. This will automatically save the model when it has finished training. 


**Using model on patients**

After training you can used the saved model to segment the cardiac structures of patients. This can be done by running the run_model.py file. Make sure to check if the name of the model is correct.
