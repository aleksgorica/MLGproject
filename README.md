# MLGproject

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
 - I think we shouldn't use list of graphs, but rather `torch_geometric.data.Data` object. (cell subgraph splitting) It's probably more efficient.
 - Decide on BatchNorm ot LayerNorm
 - Change GAT aggregation to sum? (mean is implicit on `concat=false`, sum needs extra code/GATConv modification)
- Try different optimizers? (look at colabs)
- K-fold splitting or validation set?
- Seaborn palette for nicer plots
- Discuss about preprocessing (preprocess before DataFrame -> Graph or in model forward pass?)
- Printing F1 score on train, test set for each epoch instead of CrossEntropy
## Dataset
Is available at [Kaggle](https://www.kaggle.com/datasets/ellipticco/elliptic-data-set?resource=download)

