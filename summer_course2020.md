## Got Behavior? Get Poses ...  <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1572296495650-Y4ZTJ2XP2Z9XF1AD74VW/ke17ZwdGBToddI8pDm48kMulEJPOrz9Y8HeI7oJuXxR7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z5QPOohDIaIeljMHgDF5CVlOqpeNLcJ80NK65_fV7S1UZiU3J6AN9rgO1lHw9nGbkYQrCLTag1XBHRgOrY8YAdXW07ycm2Trb21kYhaLJjddA/DLC_logo_blk-01.png?format=1000w" width="350" title="DLC-live" alt="DLC LIVE!" align="right" vspace = "50">

This document is a **WIP** outline of resources for an informal "spring/summer course" for those wanting to learn to use DeepLabCut while responsibilty isolating due to COVID-19.

www.deeplabcut.org 

We suggest student self organize into groups to work through this together. Perhaps find each other on Gitter or Twitter:
[![Gitter](https://badges.gitter.im/DeepLabCut/community.svg)](https://gitter.im/DeepLabCut/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
[![Twitter Follow](https://img.shields.io/twitter/follow/DeepLabCut.svg?label=DeepLabCut&style=social)](https://twitter.com/DeepLabCut)

## Quick Start:

You need: Anaconda for python3 and DeepLabCut installed (CPU version)
- you should have a [CPU version of DeepLabCut installed on your laptop](https://github.com/AlexEMG/DeepLabCut/blob/master/conda-environments/README.md). We will assume you don't all have GPUs at home, so we will 
utilize cloud-computing resources for those steps. 

## Outline:

### **The basics:**

- **DEMO:** Can I DEMO DEEPLABCUT (DLC) quickly? 
    - Yes: [you can click through this DEMO notebook](https://colab.research.google.com/github/AlexEMG/DeepLabCut/blob/master/examples/COLAB_DEMO_mouse_openfield.ipynb)
    - AND follow along with me: [Video Tutorial!](https://www.youtube.com/watch?v=DRT-Cq2vdWs)

- **Information:** Using the program terminal / cmd on your computer: [Video Tutorial!](https://www.youtube.com/watch?v=5XgBd6rjuDQ)

- **WATCH:** How do you know DLC is installed properly? (i.e. how to use our test script!)[Video Tutorial!](https://youtu.be/IOWtKn3l33s)


<img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1587608364285-A8R2F24K4DCP0KLAYI91/ke17ZwdGBToddI8pDm48kOhrDvKq54Xu9oStUCFZX0R7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0p4XabXLlNWpcJMv7FrN_NLe3GEN018us8vX03EdtIDHsW7dEh7nvL5CemxAxOy1gg/EKlIEXyXUAE0cy3.jpeg?format=1000w" width="350" title="DLC" alt="review!" align="right" vspace = "50">

- **REVIEW PAPER:** The state of animal pose estmiation w/deep learning i.e. "Deep learning tools for the measurement of animal behavior in neuroscience" [arXiv](https://arxiv.org/abs/1909.13868) & [published version](https://www.sciencedirect.com/science/article/pii/S0959438819301151)




- **WATCH:** There are a lot os docs... where to begin: [Video Tutorial!](https://www.youtube.com/watch?v=A9qZidI7tL8) 

### **Module 1: getting started on your own data**

What you need: any videos where you can see the animals/objects, etc. 
You can use our demo videos, grab some from the internet, or use whatever older data you have. Any camera, color/monchrome, etc will work. Find diverse videos, and label what you want to track well :) 

:purple_heart: **NOTE:** if you want to contribute back to community-science, please get in touch with us as we have a LOT of data we want to label to be able to share back with everyone; So, if you want to help sign up here (labeling can be on data we provide or possibly yours): https://forms.gle/KRtdKKYB57ZkaBwH7 :purple_heart:
    
   - **Slides:** [Overview of starting new projects](https://github.com/DeepLabCut/DeepLabCut-Workshop-Materials/blob/master/part1-labeling.pdf)
   - **READ ME PLEASE:** [DeepLabCut, the science](rdcu.be/4Rep)
   - **READ ME PLEASE:** [DeepLabCut, the user guide](https://rdcu.be/bHpHN)
   - **WATCH:** Video tutorial 1: [using the Project Manager GUI](https://www.youtube.com/watch?v=KcXogR-p5Ak)
     - Please go from project creation (use >1 video!) to labeling your data, and then check the labels!
   - **WATCH:** Video tutorial 2: [using ipython/pythonw (more functions!)](https://www.youtube.com/watch?v=7xwOhUcIGio)
      - coming soon, multi-animal DLC: [labeling preview](https://www.youtube.com/watch?v=_qbEqNKApsI)
      - Please go from project creation (use >1 video!) to labeling your data, and then check the labels!
      

### **Module 2: Neural Networks**
 
   - **Slides:** [Overview of creating training and test data, and training networks](https://github.com/DeepLabCut/DeepLabCut-Workshop-Materials/blob/master/part2-network.pdf)
   - **READ ME PLEASE:** [What are convolutional neural networks?](https://towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53) 
   
  Before you create a training/test set, please read/watch:
   - **More information:** [Which types neural networks are available, and what should I use?](https://github.com/AlexEMG/DeepLabCut/wiki/What-neural-network-should-I-use%3F)
   - **WATCH:** Video tutorial 1: [How to test different networks in a controlled way](https://www.youtube.com/watch?v=WXCVr6xAcCA)
     - Now, decide what model(s) you want to test. 
        - IF you want to train on your CPU, then run the step `create_training_dataset`, in the GUI etc. on your own computer. 
        - IF you want to use GPUs on google colab, [**(1)** watch this FIRST/follow along here!](https://www.youtube.com/watch?v=qJGs8nxx80A) **(2)** move your whole project folder to Google Drive, and then [**use this notebook**](https://github.com/AlexEMG/DeepLabCut/blob/master/examples/COLAB_YOURDATA_TrainNetwork_VideoAnalysis.ipynb)
   

### **Module 3: Evalution of network performance**
 
   - **Slides** [Evalute your network](https://github.com/DeepLabCut/DeepLabCut-Workshop-Materials/blob/master/part3-analysis.pdf)
   - **WATCH:** [Evaluate the network in ipython](https://www.youtube.com/watch?v=bgfnz1wtlpo)
      - why evaluation matters; how to benchmark; analyzing an video and using scoremaps, conf. readouts, etc 
   
### **Module 4: Scaling your analysis to many new videos**
 
   - [Analyzing videos in batches, over many folders, setting up automated data processing](https://github.com/DeepLabCut/DLCutils/tree/master/SCALE_YOUR_ANALYSIS) 
   
### **Module 5: Got Poses? Now what ...**
 
   - [Helper code and packages for use on DLC outputs](https://github.com/DeepLabCut/DLCutils)


**Other ideas:**

- Docker, 3D DLC, ...

*compiled and edited by Mackenzie Mathis*
