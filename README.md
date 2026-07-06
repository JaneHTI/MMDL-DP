# MMDL-DP: A PyTorch Implementation

This is a PyTorch/GPU implementation of the paper "A multimodal deep learning framework for psychopathology risk stratification and forecasting from birth to early adulthood".

## Install

conda env create -f environment.yml

conda activate MMDLPP

## Files and Usage

- demo_main.py # Model training and testing, along with detailed specifications of configuration parameters and core functional components.
  
- lib          # Data loading and model setting.
- - dataset_graph.py
  data_load.py
  loss.py
  model_clinic.py
  model_conn.py
  model_fusion.py
  model_t1.py
  
- data         # Data
  
- checkpoints  # Trained model
  
- utils        # Function for result analysis.

## **License**

**AGPL-3.0 License:** See the [LICENSE](https://github.com/IMMULab/BMUNet/blob/main/LICENSE) file for more details.

## Note

The Mirai model(`mirai_model/snapshots/mgh_mammo_MIRAI_Base_May20_2019.p`) is used as pretrained model for Mammography module, where [onconet](https://github.com/yala/Mirai) is the Mirai model code
