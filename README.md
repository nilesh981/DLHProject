# Deep Learning for Healthcare Final Project
**Group ID:** 162 <br/>
**Paper ID:** 208 <br/>
**Paper Name:** SafeDrug: Dual Molecular Graph Encoders for Safe Drug Recommendations <br/>
**Difficulty:** Hard <br/>

## Team Members

 - Venkat Nilesh Dadi (vdadi2)
 - Surya Sindhu Mallimanugula (ssm13)
 
 ## Citation
 Yang, Chaoqi & Xiao, Cao & Ma, Fenglong & Glass, Lucas & Sun, J.. (2021). SafeDrug: Dual Molecular Graph Encoders for Safe Drug Recommendations: n. pag. <br/>
 **Paper Link:** [[2105.02711] SafeDrug: Dual Molecular Graph Encoders for Safe Drug Recommendations (arxiv.org)](https://arxiv.org/abs/2105.02711) <br/>
 **Paper Repo:** https://github.com/ycq091044/SafeDrug <br/>

## Dependencies 

 1. Anaconda Navigator
 2. rdkit
 3. scikit-learn
 4. dill
 5. dnc
 6. numpy
 7. pandas
 8. torch
 9. cuda ( [Installation Guide Windows :: CUDA Toolkit Documentation (nvidia.com)](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)
 10. torchvision 
 11. torchaudio
 
 ## Data Download Instructions
 
 1. **MIMIC-III Data** - Go to https://physionet.org/content/mimiciii/1.4/ and download PROCEDURES_ICD.csv.gz, PRESCRIPTIONS.csv.gz, and DIAGNOSES_ICD.csv.gz. <br/>
 2. **RXCUI2atc4.csv** - https://github.com/sjy1203/GAMENet <br/>
 3. **drug-atc.csv** - https://github.com/sjy1203/GAMENet <br/>
 4. **rxnorm2RXCUI.txt** - https://github.com/sjy1203/GAMENet <br/>
 5. **drugbank_drugs_info.csv** - https://www.dropbox.com/s/angoirabxurjljh/drugbank_drugs_info.csv?dl=0 <br/>
 6. **drug-DDI.csv** - https://drive.google.com/file/d/1mnPc0O0ztz0fkv3HF-dpmBb8PLWsEoDz/view?usp=sharing <br/>
 
## Preprocessing Code

For the data preprocessing, download the MIMIC-III data and link the files in the directory to the code.
Then run - ``` python processing.py ```

##  Model

The model goes through training and eval in the same instance. To run the code, we need to call ```python SafeDrug --model_name MODEL_NAME``` or run the model directly using ```python MODEL_NAME.py```

## Results

| Results by | DDI Rate | Jaccard Similarity | F1 Score | Training Time |
|---|---|---|---|---|
| Authors | 0.0589 | 0.5213 | 0.6768 | 138.77s |
| Average Epoch | 0.06084 | 0.51239 | 0.66891 | 337.67s |
| Best Epoch | 0.05955 | 0.5122 | 0.66708 | 337.51s |
