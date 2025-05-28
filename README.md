
## Description
* model.py  
  * MLP() -- A pure MLP-based architecture 
* dataset.py  

  * dataloader() -- Load six datasets as well as their variants with different label rates and label noise.
* utils.py  
  * SetSeed() -- Set seeds for reproducible results.



## Running the code

1. Install the required dependency packages

3. To get the results on a specific *dataset*, please run with proper hyperparameters:

  ```
python main.py --dataset data_name
  ```

where the *data_name* is one of the 6 datasets (Cora, Citeseer, Coauthor-CS, and Coauthor-Phy, Amazon-Com, and Amazon-Photo). Use  *Cora* dataset an example: 

```
python main.py --dataset cora
```

3. To get the results on datasets with different label rates, label noise, and struture disturbance, please run with:

  ```
python main.py --model_mode
  ```



