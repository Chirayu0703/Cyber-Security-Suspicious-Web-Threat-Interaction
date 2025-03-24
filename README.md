# Cybersecurity: Suspicious Web Threat Interactions

## Overview
This project focuses on analyzing suspicious web traffic interactions using Machine Learning techniques. It leverages data collected via AWS CloudWatch to identify potential threats and anomalies in web traffic.

## Technologies Used
- **Programming Language**: Python
- **Machine Learning Libraries**: Scikit-learn, TensorFlow
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Database**: SQL, Excel
- **Development Tools**: VS Code, Jupyter Notebook

## Dataset
- The dataset contains web traffic logs captured from a production web server.
- It includes features like `bytes_in`, `bytes_out`, `src_ip`, `dst_port`, `protocol`, `detection_types`, etc.
- The goal is to classify web traffic as normal or suspicious based on these features.

## Project Workflow
1. **Data Import & Preprocessing**
   - Load dataset using Pandas.
   - Handle missing values and convert data types.
   - Feature extraction (e.g., session duration, average packet size).

2. **Exploratory Data Analysis (EDA)**
   - Traffic pattern visualization.
   - Analysis of suspicious activities by country and ports.
   - Correlation analysis between traffic parameters.

3. **Machine Learning Models**
   - **Anomaly Detection**: Isolation Forest for outlier detection.
   - **Classification Model**: Random Forest for identifying suspicious traffic.
   - **Neural Network**: Deep learning model trained on labeled data.

4. **Model Evaluation**
   - Accuracy and classification reports.
   - Visualization of anomalies.

5. **Findings & Insights**
   - High `bytes_in` with low `bytes_out` may indicate infiltration attempts.
   - Certain countries show frequent suspicious traffic.
   - Non-standard port activity is linked to unauthorized access attempts.

## Installation & Usage
1. Clone the repository:
   ```sh
   git clone <repo-url>
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the analysis:
   ```sh
   python main.py
   ```

## References
- Dataset: [AWS CloudWatch Logs](https://drive.google.com/file/d/1-OpnR9FK8EqGuLFB1k45ctPbl-vuZnC-/view?usp=sharing)
- GitHub Reference: [Web Threat Analysis](https://github.com/Tharunr0/Web-Threat-Analysis-Cyber-Security)
