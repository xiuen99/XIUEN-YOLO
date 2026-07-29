# Code for 

This repository contains the source code used in the manuscript:

> **"An Insulator Defect Detection Method for Transmission Lines in Complex Weather Conditions Based on Improved YOLOv8n"**
>
> Submitted to **PLOS ONE**.

## Overview

This repository provides the implementation used for model training, validation, and inference described in the manuscript.

The code is based on the Ultralytics YOLO framework and includes our modifications for the proposed method.

---

## Repository Structure

```
cfg/            Configuration files
models/         Model definitions
engine/         Training and inference engine
utils/          Utility functions
data/           Dataset processing utilities
assets/         Example images
```

---

## Requirements

Recommended environment:

- Python 3.10
- PyTorch >= 2.0
- CUDA 11.x (optional)
- Ultralytics
- OpenCV
- NumPy

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Dataset

The dataset used in this study is **not included** in this repository due to publication restrictions.

Please prepare the dataset according to the structure described in the manuscript and configure the dataset path in the corresponding YAML file under `cfg/datasets/`.

---

## Training

Example:

```bash
python train.py
```

or

```bash
yolo train model=yoloM4+CBAM+BIFPN.yaml data=It needs to be prepared by yourself because GITHUB can only upload up to 25MB.
```

Please modify the configuration according to your experiment.

---

## Inference

Example:

```bash
python predict.py
```

or

```bash
yolo predict model=best.pt source=test.jpg
```

---

## Reproducing the Results

To reproduce the experiments reported in the manuscript:

1. Install the required dependencies.
2. Prepare the dataset following the manuscript.
3. Configure dataset paths.
4. Train the model using the provided configuration.
5. Evaluate using the same metrics reported in the paper.

Random seeds and parameter settings are provided in the configuration files whenever applicable.

---

## Citation

If you use this code, please cite:

```
Author et al.
Title.
PLOS ONE.
```

---

## License

This project is released under the MIT License.

---

## Contact

For questions regarding this repository, please contact:15207182499

Xiuyang Yuan

Email: yuanxiuyang1021@126.com
