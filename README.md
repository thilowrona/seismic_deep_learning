# Deep learning of geological structures from seismic reflection data

Here we share code, tutorials and examples showing how to interpret geological structures (e.g. faults, salt bodies and horizones) in 2-D and/or 3-D seismic reflection data using deep learning. The corresponding manuscript is available at: XXX.

## Getting started
One of the easiest ways of getting started is to use Colab, where most of the things we need (GPU, Cuda, Tensorflow) are already set up, so you won't need to set it up on your own machine. This tutorial, which is based on the excellent https://course.fast.ai/, shows you how to train your first deep learning model to interpret salt in 2-D seismic reflection data.

### Colab ###
1. First, you need sign in to your Google account. If you're not signed in, you can sign in [here](https://myaccount.google.com/?utm_source=sign_in_no_continue)

2. Next, head on to the [Colab Welcome Page](https://colab.research.google.com/notebooks/welcome.ipynb#recent=true). Now, you should see a page looking like this:! [alt text](https://github.com/thilowrona/seismic_deep_learning/blob/s1.png)






and click on ‘Github’. In the ‘Enter a GitHub URL or search by organization or user’ line enter ‘fastai/course-v3’. You will see all the courses notebooks listed there. Click on the one you are interested in using.











### Install Python ###
First, you need Python 3. You could either 

1. Install **Python 3**
2. Install required packages listed in ```requirements.txt```. You can install these packages with:

``` pip install -r /path/to/requirements.txt ```

3. Clone git repository:

```git clone https://github.com/thilowrona/seismic_deep_learning/```
