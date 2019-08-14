This code uses the weight sparsity control in a multi-layer neural network for classification.  
You may easily utilize the weight sparsity control follwing several steps described below.  


___ 

# Prerequisites

  - Type 'git clone https://github.com/bsplku/KHBM2019_SummerSchool' in the command line, or go to the link and manually download .zip file, and then unzip it

  - Go to 'https://colab.research.google.com' and log-in to Google
 
  - File - Open notebook - UPLOAD - Choose file:  .../KHBM2019_SummerSchool-master/Classification_of_fMRI_volume/dnnwsp_hsp_tensorflow.ipynb
 
  - Edit - Notebook Settings: Set Runtime type as 'Python 3' and Hardware accelerator as GPU
  
  - Go to https://drive.google.com to see and download the results

##

# 1. Introduction of sensorimotor experiment  
   __1-1. Task paradigm__  
     - Left-hand clenching (LH), right-hand clenching, auditory attention (AD), and visual stimulus (VS) tasks.  
            
   __1-2. Blood-oxygenation-level-dependent (BOLD) fMRI data__  
     - Scanner spcification and imaging sequence.  
            
   __1-3. Preprocessing of BOLD fMRI data__  
      - Preprocessing via SPM.  
  
##
  
  
# 2. Task classification using neural network (Tensorflow)  
  __2-0. Mounting Google drive to save the results__  
     - Go to the link and copy & paste the authorization code. 
    
   __2-1. Input data__  
     - Once more, go to the link and copy & paste the authorization code.  
     - Load data from the downloaded file.  
     - Plot the volume data using Nilearn library.
     
   __2-2. Import libraries__  
     - Importing necessary Python libraries.  
    
   __2-3. Define a classifier__  
     - Define a neural network classifier.  
    
   __2-4. Define training parameters__  
     - Define training parameters such as cost(= loss) and so on.  
    
   __2-5. Define Hoyer's sparsity control function__  
     - Define the function of calculating and updating beta based on Hoyer's sparseness.  
    
   __2-6. Set hyperparameters for training__  
     - Specify your model spec (Here is the part that you might want to modify for your own model).  
  
   __2-7. Initialize a model using definitions above__  
     - Actually build the model from the definitions and specifications.  
    
   __2-8. Start learning__  
     - Start training (This block will automatically find the optimal sparsity from the validation performances, and then test with selected one).  
    
   __2-9. Save parameters and summary as text file__  
     - Save the hyperparameter values that you set and classification errors from validation and test phases in a text file.   
        
   __2-10. Weight feature map interpretation__  
     - Calcualte the weight feature maps from the trained weight parameters and visualize it by Nibabel
  
     
  ##
