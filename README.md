# MLGproject
article: https://medium.com/@nm8144/a7a40caeb959

## Running
 - If running from local, set env variable `DATASET_PATH` to path of your local dataset folder.
 - If running from colab, just run and use Google GPU :)
 - Running GAT: very important, to make sure `concat=False` in `GATConv` layer. Otherwise, it will not work. See [here](https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.nn.conv.GATConv.html#torch_geometric.nn.conv.GATConv) for more info.

### Config
There are two configs:
 - Test config: specify training configuration (epochs, batch size, etc.)
 - Model config: specify model configuration (layers, activation functions, etc.)
 
 It's best to re-run from Model definition cell to avoid errors and unexpected behaviour.

## Todo
- DONE :)

## Dataset
Is available at [Kaggle](https://www.kaggle.com/datasets/ellipticco/elliptic-data-set?resource=download)

