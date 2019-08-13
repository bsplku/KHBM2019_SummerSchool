This code uses the weight sparsity control in a multi layer neural network for classification.  
You may easily utilize the weight sparsity control follwing several steps described below.  


___ 



# 1. Introduction of sensorimotor experiment  
   __1-1. Task paradigm__  
     - Left-hand clenching (LH), right-hand clenching, auditory attention (AD), and visual stimulus (VS) tasks.  
            
   __1-2. Blood-oxygenation-level-dependent (BOLD) fMRI data__  
     - Scanner spcification and imaging sequence.  
            
   __1-3. Preprocessing of BOLD FMRI data__  
      - Preprocessing via SPM.  
  
##
  
  
# 2. Sensorimotor task classification using MLP (Tensorflow)  
  
   __2-1. Input data__  
     - Showing the brain volume data and converting to actual input of MLP.  
    
   __2-2. Import libraries__  
     - Importing necessary libraries.  
    
   __2-3. Define a classifier__  
     - Builing an MLP network for a classification.  
    
   __2-4. Define training parameters__  
     - Declaring parameters such as cost and error.  
    
   __2-5. Define Hoyer's sparsity control function__  
     - Calculating Hoyer's sparsity level and adjust beta.  
    
   __2-6. Set hyperparameters for training__  
     - Setting hyperparameters such as learning rate and target sparsity level.  
  
   __2-7. Create a model using definitions above__  
     - Creating actual model before training.  
    
   __2-8. Learning__  
     - Starting the training.
     - The optimal sparsity set is found using validation set.  
    
   __2-9. Save parameters and summary as text file__  
     - Saving the hyperparameters and summary in a text file.   
        
   __2-10. Weight featrue map interpretation__  
     - Custruvting and plotting weight feature maps for the interpretation
     
  ##
