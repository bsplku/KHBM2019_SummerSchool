
Deep neural network (DNN) with weight sparsity control (DNN-WSP; i.e., L1-norm regularization) improved 
the classification performance using whole-brain resting-state functional connectivity patterns of 
schizophrenia patient and healthy groups. Also, initializing DNN's weights through stacked auto-encoder enhanced 
the classification performance (Jang et al., Neuroimage 2017, Kim et al., Neuroimage, 2016). 

The DNN code is for regression analysis to predict emotional responses (i.e., scores) from whole-brain fMRI data. In the code, there are two options: a node-wise and layer-wise control of weight sparsity via Hoyer sparseness (Kim and Lee, PRNI2016 & ICASSP2017). The DNN code was implemented using TensorFlow. 

In this tutorial, we are going to use Google Colaboratory Notebook [https://colab.research.google.com/] Colaboratory allows you to execute TensorFlow code in your browser with a single click. Google colab is a cloud based data science work space similar to the jupyter notebook. Each colab session is equipped with a virtual machine running 13 GB of ram and either a CPU, GPU, or TPU processor. These work spaces are great for building and sharing machine learning or deep learning projects with colleagues and associates [https://www.youtube.com/watch?v=f1UK8KPt-KU&app=desktop].

==

st01_Generating_input_data_using_fMRI4D.ipynb: To generate 2-D data from 4-D fMRI data

st02_TF_dnnwsp_emotion_study.ipynb: To run DNN model for regression analysis

st03_DNNwsp_result_check.ipynb: To check and interpret results  

emt_valence_sample.mat: Valence emotion responses rated from a subjects [80 samples]

mask_map.nii: Binary in-brain mask 

[beta_maps_80trials.nii](http://bspl.korea.ac.kr/beta_maps_80trials.nii): 4D beta maps obtained for each sound stimulus [53 x 63 x 46 x 80; xdim, ydim, zdim, samples, respectively]
