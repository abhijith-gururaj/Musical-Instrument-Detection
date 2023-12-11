# Music Instrument Detection
This is a machine learning project to detect and classify musical instruments played in an audio file.  
The project uses a CNN model to detect 11 types of musical instruments:
|  Instrument | Label  |
|---|---|
| Cello  |  cel |
| Clarinet  | cla  |
| Flute | flu |
| Acoustic Guitar | gac |
| Electric Guitar | gel |
| Organ | org |
| Piano | pia |
| Saxophone | sax |
| Trumpet | tru |
| Violin | vio |
| Voice | voi |

## Authors
Abhijith Gururaj, Thomas Stapor, Akhil Palla

## Code Layout
The project comprises of four main jupyter notebooks:
1. preprocessing.ipynb
2. train_model.ipynb
3. predict_labels.ipynb
4. report_metrics.ipynb

All these notebooks should be run in successive order for training, predicting and reporting the performance of the model.

## System Requirements
The notebooks require at least 12GB RAM for execution.
The required python packages for this project are present in requirements.txt

## Instructions to execute and evaluate the model
The project requires the IRMAS Dataset which is available here: https://zenodo.org/records/1290750  
Please download the following zip files from the above link:
1. IRMAS-TrainingData.zip
2. IRMAS-TestingData-Part1.zip
3. IRMAS-TestingData-Part2.zip
4. IRMAS-TestingData-Part3.zip

After extracting the above zip files, the codebase should have the following directory structure before execution:  
![Alt text](images/image.png)  

## Note: The directory IRMAS-TestingData-Part2/ has a nested folder called IRMAS-TestingData-Part2/IRTestingData-Part2/. Please rename the directory IRMAS-TestingData-Part2/**IRTestingData-Part2**/  to IRMAS-TestingData-Part2/**Part2**. This is necessary for the data preprocessing stage.

Please ensure the system requirements are satisfied and execute the notebooks in the following order:
1. preprocessing.ipynb
2. train_model.ipynb
3. predict_labels.ipynb
4. report_metrics.ipynb

The report_metrics.ipynb should display the accuracy and f1-score metrics of the CNN model. 