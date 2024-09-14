# orddc_2024


# Optimized Road Damage Detection Challenge ([ORDDC'2024](https://orddc2024.sekilab.global/)) Submission

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

Create a new Conda environment named orddc_2024 with **Python 3.10** and activate it:
```bash
conda create -n orddc_2024 python=3.10 -y
conda activate orddc_2024
```

### 3. Install the required packages

Install all the required packages using the requirements.txt file:
```bash
pip install -r requirements.txt
```

## Detection / Submission

1. Run the inference script using one of the following commands, depending on the phase you are working on.

### For Phase 1 Best Result
> Execute the Phase 1 inference script with:
```bash
python inference_script_v2_Phase1.py ./images ./output_csv_file_Phase1.csv
```
Output: ./Phase1_output_Approach23_Conf_0.3.csv
* Note: When running **inference_script_v2_Phase1.py**, the CSV file **Phase1_output_Approach23_Conf_0.3.csv** will be downloaded along with the models.

#### Phase 1. submission results (F1-Score)
| Model(img_size)      | Nano | Small | Medium | Large | XLarge |
|:------------:|:------:|:-------:|:--------:|:-------:|:--------:|
| YOLOv5(640)     |  ✓(tiny)   |   ✓   |   ✓    |   ✓   |   ✓    |
| YOLOv8(640)     |  ✓   |   ✓   |   ✓    |   ✓   |   ✓    |
| YOLOv10(640)    |  ✓   |   ✓   |   ✓    |   ✓   |   ✓    |
**F1 Score**: 0.7664

### For Phase 2 Best result
> Execute the Phase 2 inference script with:
```bash
python inference_script_v2_Phase2.py ./images ./output_csv_file_Phase2.csv
```
#### Phase 2. Submission Results (F1-Score and Inference Speed)

| Model(img_size)      | Nano | Small |
|:----------:|:----:|:-----:|
| YOLOv5(640)     |      |   ✓   |
| YOLOv8(960)     |   ✓  |       |

| F1-Score (6 countries)  | Inference Speed (6 countries) (sec/image) |
|:-----------------------:|:----------------------------------------:|
| 0.7017                  | 0.0432                                   |


### Positional Arguments:
- **./images**: Path to the directory containing images for inference
- **./output_csv_file_Phase1.csv**: output CSV file name including directory name