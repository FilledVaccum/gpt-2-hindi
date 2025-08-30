# GPT-2 Hindi

A GPT-2 model implementation for Hindi text generation learning from Andrej Karpathy

## Overview

This project implements a GPT-2 model fine-tuned for Hindi language text generation. The model uses a large Hindi text dataset to generate coherent Hindi text based on input prompts. It barely have 10 million parameters 

## Repository Structure

```
├── data/
│   ├── hindi_input.txt     # Hindi training dataset (managed by DVC)
│   └── .gitignore
├── src/
│   ├── Hindi_GPT.ipynb     # Main notebook with model implementation
│   └── gpt_hindi_2_output.txt  # Sample model output
├── .dvc/                   # DVC configuration
├── .gitattributes
└── .gitignore
```

## Features

- Hindi text generation using GPT-2 architecture
- Large-scale Hindi dataset processing
- Jupyter notebook implementation
- Github LFS because I tried DVC integration for data version control but it did not work, need to spend more time

<img width="1512" height="498" alt="Screenshot 2025-08-30 at 7 25 04 PM" src="https://github.com/user-attachments/assets/ad33426d-0e64-475d-a6fd-f2a98cac7986" />
<img width="1512" height="682" alt="Screenshot 2025-08-30 at 7 25 35 PM" src="https://github.com/user-attachments/assets/50e99232-d1e0-4c76-a839-7d2187dd6f27" />
<img width="1512" height="834" alt="Screenshot 2025-08-30 at 7 26 35 PM" src="https://github.com/user-attachments/assets/672f57fa-ef33-4465-9119-83585726604c" />


## Requirements

- Python 3.x
- huggingface-hub
- pandas
- transformers
- torch

## Usage

1. Clone the repository:
```bash
git clone https://github.com/FilledVaccum/gpt-2-hindi.git
cd gpt-2-hindi
```

2. Install dependencies:
```bash
pip install huggingface-hub pandas transformers torch
```

3. Run the notebook:
```bash
jupyter notebook src/Hindi_GPT.ipynb
```

## Data

The Hindi training dataset is managed using github lfs and contains approximately 518MB of Hindi text data. The dataset is stored as `hindi_input.txt` in the `data/` directory.

Learning - Data in Fineweb2 by common crawl is really not good quality dataset for hindi language

## Model Output

The model generates Hindi text based on input prompts. Sample outputs are available in `src/gpt_hindi_2_output.txt`.

## Contributing

Feel free to submit issues and pull requests to improve the model or add new features.

## License

This project is open source. Please check the repository for specific license information.
