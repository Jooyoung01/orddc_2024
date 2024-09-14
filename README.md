# orddc_2024


# Optimized Road Damage Detection Challenge (ORDDC'2024)

*The models will be automatically downloaded when you run the script.*

## Setup

### 1. Download the Project

You can either unzip the provided ZIP file or clone the repository from GitHub.

**Option 1: Unzip the ZIP File**

```bash
unzip orddc_2024.zip -d ./
cd orddc_2024
```
**Option 2: Clone from GitHub**
```bash
git clone https://github.com/Jooyoung01/orddc_2024.git
cd orddc_2024
```

### 2. Create and Activate the Conda Environment

Create a new Conda environment named orddc_2024 with Python 3.10 and activate it:
```bash
conda create -n orddc_2024 python=3.10 -y
conda activate orddc_2024
```

### 3. Install the required packages

Install all the required packages using the requirements.txt file:
```bash
pip install -r requirements.txt
```

## Usage

1. Run the inference script using one of the following commands, depending on the phase you are working on.

> For Phase 1 Best Result
Execute the Phase 1 inference script:

```bash
python inference_script_v2_Phase1.py ./images ./predictions.csv
```
Output: ./Phase1_output_Approach23_Conf_0.3.csv
* Note: When running **inference_script_v2_Phase1.py**, the CSV file **Phase1_output_Approach23_Conf_0.3.csv** will be downloaded along with the models.

> For Phase 2 Best result : 
Execute the Phase 2 inference script:
```bash
python inference_script_v2_Phase2.py ./images ./predictions.csv
```
### Positional Arguments:
- **image_path**: Path to the directory containing images for inference
- **output_csv_file**: output CSV file name including directory name