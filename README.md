# Deep learning of geological structures from seismic reflection data

Here we share code, tutorials and examples showing how to interpret geological structures (e.g. faults, salt bodies and horizones) in 2-D and/or 3-D seismic reflection data using deep learning. The corresponding manuscript is available at: XXX.

## Getting started
One of the easiest ways of getting started is to use Colab, where most of the things we need (GPU, Cuda, Tensorflow) are already set up, so you won't need to set it up on your own machine. This tutorial, which is based on the excellent https://course.fast.ai/, shows you how to train your first deep learning model to interpret salt in 2-D seismic reflection data.

### Colab ###
1. First, you need sign in to your Google account. If you're not signed in, you can sign in [here](https://myaccount.google.com/?utm_source=sign_in_no_continue)

2. Next, head on to the [Colab Welcome Page](https://colab.research.google.com/notebooks/welcome.ipynb#recent=true). Now, you should see a page looking like this:

![alt text](https://github.com/thilowrona/seismic_deep_learning/blob/master/s1.png)

3. Now click on ´Github´ at the top of the orange pop-up and search for XXX. Once you click on the file named XXX, you've opened your first Jupyter notebook! These  notebooks are an awesome combination of code and documentation allowing us work on, describe and share our projects.

4. Before running anything, you need to tell Colab that would like to use a GPU (important to train our models quickly). This is done by clicking on the ‘Runtime’ tab, selecting ‘Change runtime type’, changing hardware accelerator to ´GPU´ and clicking ´save´. Excellent! Colab is now set up!


### Notebook ###
1. Before using your notebook, you need to install the necessary packages. You can do this by creating a code cell (i.e. clicking ´+ code´ in top left corner), running this command:
```console
 !curl -s https://course.fast.ai/setup/colab | bash
```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and runnign the cell (i.e. clicking the play symbol or pressing ‘Ctrl+Enter‘).

2. When you run the first cell, you will face a pop-up saying ‘Warning: This notebook was not authored by Google’; you should click on ‘Run Anyway’ to get rid of the warning.

3. Next we want to save our notebook. If you click on ‘File’ and then ‘Save’, you will see a pop-up saying ´CANNOT SAVE CHANGES´. Now, click on ‘SAVE A COPY IN DRIVE’. This opens up a new tab with the same file, but this time located in your Drive. If you want to continue working after saving, use the file in the new tab. Your notebook will be saved in a folder called Colab Notebooks in your Google Drive by default.

4. Last, we would like to load and save files (e.g. our seismic and interpretation). If you run a script which creates/ downloads files, the files will NOT persist after the allocated instance is shutdown. To save files, you need to permit your Colaboratory instance to read and write files to your Google Drive. Luckily, Colaboratory has a UI for permanently mounting your Google Drive.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Click on the files icon on the left sidebar:

![alt text](https://github.com/thilowrona/seismic_deep_learning/blob/master/s2.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and click on the ´Mount Drive´ icon in the top right corner. After clicking the button you’ll be asked to authorize Colaboratory to access your Google Drive. Once you do, your notebook will automatically mount that drive whenever the runtime is loaded, and the sidebar will show the contents of your drive. Accessing data on your drive is then simply a matter of pointing at the right path. Add the following code snippet at the beginning of every notebook:
```console
root_dir = "drive/My Drive/"
base_dir = root_dir + 'fastai-v3/'
```







