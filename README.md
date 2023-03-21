# MLGproject

## Running
 - If running from local, set env variable `DATASET_PATH` to path of your local dataset folder.
 - If running from colab, just run and use Google GPU :)

### Config
There are two configs:
 - Test config: specify training configuration (epochs, batch size, etc.)
 - Model config: specify model configuration (layers, activation functions, etc.)
 
 It's best to re-run from Model definition cell to avoid errors and unexpected behaviour.

## Todo
 - Something is wrong with device type.
 - I think we shouldn't use list of graphs, but rather `torch_geometric.data.Data` object. (cell subgraph splitting) It's probably more efficient. 

## Dataset
Is available at [Kaggle](https://www.kaggle.com/datasets/ellipticco/elliptic-data-set?resource=download)

