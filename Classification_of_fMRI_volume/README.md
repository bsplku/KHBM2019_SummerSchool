This code is for weight sparsity control in multi layer perceptron (MLP).  
You may easily utilize the weight sparsity control follwing several steps described below.  


#  



# 1. Introduction of sensorimotor experiment  
    **1-1. Task paradigm** 
      - Left-hand clenching (LH), right-hand clenching, auditory attention (AD), and visual stimulus (VS) tasks.  
            
    **1-2. Blood-oxygenation-level-dependent (BOLD) fMRI data** 
      - Scanner spcification and imaging sequence.  
            
    **1-3. Preprocessing of BOLD FMRI data** 
      - Preprocessing via SPM.  
  
___
  
  
# 2. Sensorimotor task classification using MLP (Tensorflow)  
  
    ** 2-1. Input data **
      - Showing the brain volume data and converting to actual input of MLP.  
    
    ** 2-2. Import libraries **
      - Importing necessary libraries.  
    
    ** 2-3. Define a classifier **
      - Builing an MLP network for a classification.  
    
    ** 2-4. Define training parameters** 
      - Declaring parameters such as cost and error.  
    
    2-5. Define Hoyer's sparsity control function
      - Calculating Hoyer's sparsity level and adjust beta.  
    
    2-6. Set hyperparameters for training
      - Setting hyperparameters such as learning rate and target sparsity level.  
  
    2-7. Create a model using definitions above
      - Creating actual model before training.  
    
    2-8. Learning
      - Starting the training.
      - The optimal sparsity set is found using validation set.  
    
    2-9. Save parameters and summary as text file
      - Saving the hyperparameters and summary in a text file.   
        
    2-10. Weight featrue map interpretation  
      - Custruvting and plotting weight feature maps for the interpretation
