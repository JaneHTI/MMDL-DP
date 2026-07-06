# MMDL-DP: A PyTorch Implementation

This is a PyTorch/GPU implementation of the paper "A multimodal deep learning framework for psychopathology risk stratification and forecasting from birth to early adulthood".

## 📋 Requirements

conda env create -f environment.yml

conda activate MMDLPP

## 📁 Project Structure

```
MMDL-DP/
├── data/
│   ├── ABCD/                         # demo data from ABCD cohort
│   │   ├── abcd_demo_clinical.xlsx   # Clinical variables
│   │   ├── abcd_demo_fc.h5           # Functional connectivity (FC)
│   │   └── abcd_demo_sc.h5           # Structural connectivity (SC)
│   │   └── abcd_demo_t1.mat          # Brain morphology
├── lib/
│   ├── Bio_ClinicalBert/
│   │   ├── download_link.txt         # Pretrained Bio_ClinicalBert model
│   ├── dataset_graph.py              # Organize connectivity data into a graph
│   ├── dataset_load.py               # Load dataset
│   ├── loss.py                       # Loss function for model training
│   ├── model_clinic.py               # Model for clinical variables
│   ├── model_t1.py                   # Model for brain morphology
│   ├── model_conn.py                 # Model for FC or FC
│   ├── model_fusion.py               # Model for fusing features from multiple modalities
├── checkpoints/
│   │   ├── download_link.txt         # Pretrained psychopathology risk stratification model in ABCD cohort
├── utils/
│   ├── statics.py
├── demo_main.py                     # Model training and testing, along with detailed specifications of configuration parameters and core functional components.
├── environment.yml                  # Python dependencies
└── README.md
```

## 🚀 Quick Start

- Executing the script demo_main.py directly enables evaluation of the pretrained model—trained on the ABCD dataset—on the provided sample data.

- All required configuration parameters are pre-specified within the source code.

- The output includes the probability of psychopathology risk for each sample, along with aggregated statistical results stored in the checkpoint file.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.txt](LICENSE.txt) file for details.
