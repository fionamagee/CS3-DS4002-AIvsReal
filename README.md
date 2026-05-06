# CS3-DS4002

This repository contains the case study, deliverable, data, and reference materials necessary to complete the Case Study on detecting AI-generated images.

## Important Information
The two attached PDFs include both the **Prompt and Deliverable** for the case study as well as a **Rubric** to follow in order to meet all requirements successfully.

## Data
The necessary data is located in the `DATA` folder. This case study uses the **Defactify Image Dataset**, a publicly available collection of real and AI-generated images hosted on Hugging Face. Because the full dataset (~96,000 images) is too large to host on GitHub, the `DATA` folder contains:
- A small sample subset (`sample_images/`) so students can verify their pipeline works before downloading the full dataset.
- A loader script (`download_dataset.py`) that pulls the full dataset from Hugging Face.
- A data dictionary (`data_dictionary.md`) describing the columns and labels.

## Reference Materials
The `Reference Materials` folder contains helpful resources organized into three subfolders:
- **Context** — articles on why AI-image detection matters (misinformation, deepfakes, the limits of human detection).
- **Data context** — documentation about the Defactify dataset and the generative models that produced the images.
- **Technical** — guides on CNNs, Vision Transformers, transfer learning, and ensembling for image classification.
