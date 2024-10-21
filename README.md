# MSI-GCN-delivery-flow

This repository contains the PyTorch implementation for our working paper titled *“Multiple-Spatial-Interaction Graph Convolutional Networks for Instant Delivery Flow Prediction”*.

We construct a heterogeneous graph convolutional network that considers four types of spatial interactions related to the spatiotemporal characteristics of instant delivery within urban units. With this approach, we achieve improved prediction accuracy for both the demand and flow of instant delivery. Furthermore, the model can be applied to future flow prediction under scenarios involving land-use changes.


![Pipeline](/assets/key_vision.png)

## 1. Requirements
- pytorch
- numpy
- pandas

## 2. Dataset
We provide the dataset of instant delivery flow prediction in this repository.

| File Name / Folder                          | Content                                                             |
| ------------------------------------------- | ------------------------------------------------------------------- |
| `./edge_data/dcorr_edges.csv`               | Distance correlation edges between nodes                             |
| `./edge_data/delivery.csv`                  | Instant delivery data for urban units                                |
| `./edge_data/fcorr_edges.csv`               | Flow correlation edges between nodes                                 |
| `./edge_data/in_flow_edges.csv`             | In-flow edges representing delivery flow into nodes                  |
| `./edge_data/out_flow_edges.csv`            | Out-flow edges representing delivery flow out of nodes               |
| `./edge_data/pcorr_edges.csv`               | Proximity correlation edges between nodes                            |
| `./edge_data/proximity_edges.csv`           | Physical proximity edges between nodes                               |
| `./node_data/Node_feats5ring_standerised.csv` | Standardized node features, including spatial characteristics         |
| `MSIGCN_main.ipynb`                         | Jupyter notebook containing the main implementation of the MSI-GCN model |

