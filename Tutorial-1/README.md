# Tutorial 1: Salt mapping #
This tutorial describes how you can map salt bodies in 2-D seismic reflection data using a deep convolutional neural network. 

1. First, we go to the [Colab Welcome Page](https://colab.research.google.com/notebooks/welcome.ipynb#recent=true). On the Github tab, we search for:
https://github.com/thilowrona/seismic_deep_learning/blob/master/Tutorial-1/tutorial-1-salt.ipynb

2. Again, we need to tell Colab to use a GPU. This is done by clicking on the ‘Runtime’ tab, selecting ‘Change runtime type’, changing hardware accelerator to ´GPU´ and clicking ´save´. Excellent! Colab is now set up!

3. Before using your notebook, you need to install the necessary packages. You can do this by creating a code cell (i.e. clicking ´+ code´ in top left corner), running this command:
```console
 !curl -s https://course.fast.ai/setup/colab | bash
```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; and runnign the cell (i.e. clicking the play symbol or pressing ‘Ctrl+Enter‘). When you run the first cell, you will face a pop-up saying ‘Warning: This notebook was not authored by Google’; you should click on ‘Run Anyway’ to get rid of the warning.

4. Next we want to save our notebook. If you click on ‘File’ and then ‘Save’, you will see a pop-up saying ´CANNOT SAVE CHANGES´. Now, click on ‘SAVE A COPY IN DRIVE’. This opens up a new tab with the same file, but this time located in your Drive. If you want to continue working after saving, use the file in the new tab. Your notebook will be saved in a folder called Colab Notebooks in your Google Drive by default.

5. Last, we would like to load and save files (e.g. our seismic and interpretation). If you run a script which creates/ downloads files, the files will NOT persist after the allocated instance is shutdown. To save files, you need to permit your Colaboratory instance to read and write files to your Google Drive. Luckily, Colaboratory has a UI for permanently mounting your Google Drive.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Click on the files icon on the left sidebar:

![alt text](https://github.com/thilowrona/seismic_deep_learning/blob/master/s2.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and click on the ´Mount Drive´ icon in the top right corner. After clicking the button you’ll be asked to authorize Colaboratory to access your Google Drive. Once you do, your notebook will automatically mount that drive whenever the runtime is loaded, and the sidebar will show the contents of your drive. Accessing data on your drive is then simply a matter of pointing at the right path. Add the following code snippet at the beginning of every notebook:
```console
root_dir = "drive/My Drive/"
base_dir = root_dir + 'fastai-v3/'
```
