

Dataset Information
Overview
For this project, the N-CMAPSS (Numerical Propulsion System Simulation) dataset, which simulates aircraft engine Remaining Useful Life (RUL) degradation using multivariate sensor time series data from NASA, will be utilized.
It is a dataset containing simulated aircraft engine degradation trajectories under different operating conditions and faults, and therefore used as a benchmark in predictive maintenance and prognostic studies.
Dataset Source
NASA Prognostics Center of Excellence
N-CMAPSS Dataset: https://data.nasa.gov/
Dataset Characteristics
* Multivariate time-series sensor data
* Aircraft engine degradation simulation
* Run-to-failure trajectories
* Operating conditions
* RUL labels
Features Used
In this project, the following features are being used:
* 14 sensor readings
* Number of sequence time steps: 50
* About 200,000 samples
Input shape:
(50, 14)
Output:
Remaining Useful Life (RUL)
Preprocessing Steps
The following preprocessing was done:
1. Extracting sensor data
2. Handling missing values
3. Min-max normalization
4. Sliding window creation for sequences
5. Time-based train/test split
6. Converting into PyTorch tensors
Dataset Split
Dataset	Shape
Training set	(159960, 50, 14)
Test set	(39990, 50, 14)
Directory Structure
After downloading the dataset, place the files inside:
text data/ ├── raw/ ├── processed/ └── dataset_instructions.md
Notes
The original NASA N-CMAPSS dataset cannot be uploaded to this repository due to licensing and file size reasons.
Please download the dataset from the official NASA website and preprocess it using the scripts contained in this repository prior to training the models.
Citation
In case you make use of N-CMAPSS dataset, kindly cite:
Saxena, A., Goebel, K., Simon, D., & Eklund, N. "Damage Propagation Modeling for Aircraft Engine Run-to-Failure Simulation." International Conference on Prognostics and Health Management (PHM), 2008.
Research Objective
The objective of this research project is to predict the Remaining Useful Life (RUL) of aircraft engines by learning the patterns of degradation from multivariate sensor readings utilizing various deep learning architectures such as CNN, LSTM, Transformer, Attention mechanisms, and proposed CNN-Transformer-Attention Hybrid model.
