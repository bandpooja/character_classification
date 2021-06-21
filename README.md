# MIDAS - coding problem
 
## TASK 2

The repository is an attempt to solve the challenge given by MIDAS for their internship program.

All the code is in `character_classification.ipynb` and some of the other items which were attempted is mentioned in `experiment_log.ipynb`

### Pre-requisits

1. Modules needed to run the notebook are all mentioned in `env.yml` file. I use Anaconda and you can create the environment I used for this project using 
    ```batch
    conda env create -f env.yml
    ```
2. The notebook assumes that the data-folders for the task-2, subtask-1 and 3 are present in the location
    ![alt text](./static/data.png).
    
3. The network and models are fairly small and thus have been pushed to the repository. Model checkpoints are all present in directory **/models**

4. The test data for **subtask-1** should also be present in the location where the notebook is.

### Additional Info
 
 - The static folder contains images which are used in the notebook.

 - predict for class MIDAS-CNN is not written atm because it was not need but it will be useful for prediction and should be straight forward to write.
  
 - Data for [subtask-1](https://www.dropbox.com/s/pan6mutc5xj5kj0/trainPart1.zip) and for [subtask-3](https://www.dropbox.com/s/otc12z2w7f7xm8z/mnistTask3.zip?dl=0) are linked.

 - Data for [testing subtask-1](https://www.dropbox.com/s/qg95ta6dm3f1mek/testPart1.zip?dl=0&file_subpath=%2Ftest%2FSample053)  

### SUBTASK-1: Test evaluation 

The test accuracy for sub-task 1 for my network is **63.44%**

![alt text](./static/final_CM.png)

Where the model lacked, involved a lot of possible confusions to naked-eye is well like `capital and small alphabets`,
other confusions include confusion between `o, 0, O, Q`; confusion between `B, 8` etc.

Atleast for small and capital context will come in extremly handy therefore predicting the character knowing a sequence 
will be something that will help the model in detecting hand-written characters. 

(**Note**: *To use an end-to-end approach for character recognition of hand-written text, will work on it soon*) 