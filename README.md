# PerCom-2023
Best performing parameter combindations for Enhanced CPC and other baselines in the paper: `Investigating Enhancements to Contrastive Predictive Coding for Human Activity Recognition`

## Supervised classifiers

| Dataset | Method | learning_rate | weight_decay |
| ---------- |  ---------- | ---------- | ---------- | 
| HHAR | Conv | 0.001 | 1e-5 |
| HHAR | DeepConvLSTM | 0.001 | 1e-5 |
| HHAR | GRU | 0.001 | 1e-5 |
| MHEALTH | Conv | 0.0005 | 1e-4 |
| MHEALTH | DeepConvLSTM | 0.001 | 0.0 |
| MHEALTH | GRU | 0.001 | 1e-4 |
| Mobiact| Conv | 0.0005 | 1e-4 |
| Mobiact | DeepConvLSTM | 0.001 | 0.0 |
| Mobiact | GRU | 0.001 | 0.0 |
| Motionsense | Conv | 0.001 | 1e-5 |
| Motionsense | DeepConvLSTM | 0.001 | 0.0 |
| Motionsense | GRU | 0.0005 | 0.0 |
| Myogym | Conv | 0.0005 | 0.0 |
| Myogym| DeepConvLSTM | 0.0005 | 0.0 |
| Myogym| GRU | 0.001 | 0.0 |
| PAMAP2 | Conv | 0.001 | 1e-5 |
| PAMAP2 | DeepConvLSTM | 0.0005 | 1e-5 |
| PAMAP2 | GRU | 0.001 | 1e-5 |

 ----
 
 ## Multi-task self-supervision (MLP classifier)
 
 | Dataset | learning_rate | weight_decay | class. learning_rate | class. weight_decay | 
| ---------- | ---------- | ---------- | ---------- | ---------- | 
| HHAR |  5e-4 | 5e-4 | 5e-4 | 1e-4 |
| MHEALTH | 5e-4 | 3e-4 | 3e-4 | 1e-4 |
| Mobiact| 5e-4 | 3e-4 | 3e-4 | 1e-4 |
| Motionsense | 3e-4 | 1e-4 | 3e-4 | 5e-4 |
| Myogym | 5e-4 | 5e-4 | 5e-4 | 1e-4 |
| PAMAP2 | 5e-4 | 5e-4 | 3e-4 | 1e-4 |

 ## Autoencoder (MLP classifier)
 
 | Dataset | learning_rate | weight_decay | class. learning_rate | class. weight_decay | 
| ---------- | ---------- | ---------- | ---------- | ---------- | 
| HHAR | 0.001 | 0 | 0.0005 | 0.0001 |
| MHEALTH | 0.0001 | 1e-05 | 0.0005 | 0.0001 |
| Mobiact| 0.0001 | 1e-05 | 0.0005 | 0.0001 |
| Motionsense | 0.0001 | 1e-05 | 0.0005 | 0.0001 |
| Myogym | 0.0001 | 0.0001 | 0.0005 | 0 |
| PAMAP2 | 0.0001 | 1e-05 | 0.0005 | 0.0001 |

## CPC (MLP classifier)

| Dataset | k | learning_rate | weight_decay | batch_size | class. learning_rate | class. weight_decay | kernel_size | 
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| HHAR | 32 | 0.0001 | 0.0001 | 64 | 0.0001 | 0 | 3 |
| MHEALTH | 48 | 0.0005 | 0 | 128 | 0.0005 | 0 | 5 |
| Mobiact| 48 | 0.0005 | 0.0001 | 128 | 0.0005 | 0 | 3 |
| Motionsense | 48 | 0.001 | 0 | 256 | 0.0001 | 1e-05 | 3 |
| Myogym | 64 | 0.0005 | 0 | 64 | 0.0005 | 1e-05 | 3 |
| PAMAP2 | 32 | 0.001 | 1e-05 | 256 | 0.0005 | 1e-05 | 3 |

## SimCLR (MLP classifier)
 
| Dataset | learning_rate | weight_decay | batch_size | class. learning_rate | class. weight_decay | 
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | 
| HHAR | 0.0001 | 0 | 4096 | 0.0005 | 0 |
| MHEALTH | 0.0001 | 0 | 4096 | 0.0005 | 0 |
| Mobiact| 0.005 | 1.00E-05 | 1024 | 0.0005 | 0 |
| Motionsense | 0.005 | 0 | 1024 | 0.0001 | 0 |
| Myogym | 0.005 | 0 | 4096 | 0.0005 | 0.0001 |
| PAMAP2 | 0.001 | 0 | 1024 | 0.0005 | 0.0001 |

## Enhanced CPC
 | Dataset | k | num_neg | num_conv_agg_layers | learning_rate | weight_decay | class. learning_rate | class. weight_decay |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| HHAR | 12 | 15 | 5 | 0.0001 | 0.0001 | 0.0005 | 0 |
| MHEALTH | 12 | 15 | 6 | 0.0005 | 0.0001 | 0.0005 | 0 |
| Mobiact| 12 | 10 | 5 | 0.0005 | 0 | 0.001 | 0.0001 |
| Motionsense | 10 | 10 | 6 | 0.00005 | 0 | 0.0001 | 0 |
| Myogym | 12 | 10 | 2 | 0.0001 | 0.00001 | 0.0005 | 0 |
| PAMAP2 | 10 | 15 | 6 | 0.00005 | 0.0001 | 0.0001 | 0 |

