
## Description

* main.py  
  * main() -- Train the model for node classification task with the proposed Neighborhood Self-Distillation module on six datasets.
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

where the *label_mode* denotes different dataset variants. **(1) 1:** training with 5 labels per class; **(2) 2:** training with 10 labels per class; **(3) 3**: training with 10 labels per class; **(4) 11:** training with label noise ratio 10%; **(5) 12:** training with label noise ratio 20%; **(6) 13:** training with label noise ratio 30%; **(7) 14:** training with label noise ratio 40%; **(8) 15:** training with label noise ratio 50%; **(9) 16:** training with label noise ratio 60%.




