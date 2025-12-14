# ALPR / Number Plate Detection (Faster R-CNN)

This repository contains code for training and evaluating a number plate detector based on Faster R-CNN, including baseline training, fine-tuning, and evaluation on DIP-processed images.

## Project Structure

- `numberplate-fasterrcnn/`  
  Baseline training code (train the initial Faster R-CNN model).

- `finetune_numberplate_fasterrcnn_clean/`  
  Fine-tuning code (train the model starting from the baseline/pretrained weights).

- `eval*` files (any file starting with `eval`)  
  Evaluation scripts for testing recognition/detection performance on DIP-processed images (DIP = Digital Image Processing).

## How to Use (High Level)

1. Train the baseline model using the code in `numberplate-fasterrcnn/`.
2. Fine-tune the model using the code in `finetune_numberplate_fasterrcnn_clean/`.
3. Run evaluation on DIP-processed images using the scripts that start with `eval`.

## Notes

- Some evaluation scripts may require paths to images and labels/annotations depending on how the dataset is organized.
- If you have multiple evaluation folders, run the corresponding `eval*` scripts for each folder.
