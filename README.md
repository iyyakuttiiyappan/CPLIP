# CPLIP: Zero-Shot Learning for Histopathology with Comprehensive Vision-Language Alignment

## Abstract

This paper proposes Comprehensive Pathology Language Image Pre-training (CPLIP), a new unsupervised technique designed to enhance the alignment of images and text in histopathology for tasks such as classification and segmentation. This methodology enriches vision-language models by leveraging extensive data without needing ground truth annotations. CPLIP involves constructing a pathology-specific dictionary, generating textual descriptions for images using language models, and retrieving relevant images for each text snippet via a pre-trained model. The model is then fine-tuned using a many-to-many contrastive learning method to align complex interrelated concepts across both modalities. Evaluated across multiple histopathology tasks, CPLIP shows notable improvements in zero-shot learning scenarios, outperforming existing methods in both interpretability and robustness and setting a higher benchmark for the application of vision-language models in the field.

## News

- **2024-03-20:** Initial code/data release.


## Requirements

- Install Python environment:
 
- Install requirements.


## Evaluation
The zero_shot_classifier function creates a zero-shot classifier by computing the embeddings for a set of class names using specified text templates.

Sure! Here’s the updated README file with the section for downloading the pretrained model:

---

# Zero-Shot Classifier

## Overview

The `zero_shot_classifier` function creates a zero-shot classifier by computing the embeddings for a set of class names using specified text templates.

## Inputs

- **model**: A model used to encode text into embeddings.
- **tokenizer**: A tokenizer used to tokenize the text.
- **classnames**: A list of class names to be used for classification.
- **templates**: A list of text templates with placeholders for class names.
- **device**: The device (CPU/GPU) to perform computations on.

## Processing

1. **Class Name Iteration**:
   - The function iterates over each class name.
   - For each class name, it replaces the placeholder in each template with the class name to generate texts.

2. **Tokenization**:
   - The generated texts are tokenized.
   - These texts are then converted to tensors suitable for the model.

3. **Text Encoding**:
   - The model encodes the texts into embeddings.
   - These embeddings are normalized.

4. **Embedding Averaging**:
   - The embeddings for each class are averaged.
   - The averaged embeddings are normalized again.

5. **Collection**:
   - The normalized embeddings are collected into a tensor representing zero-shot classification weights.

## Pretrained Models



## Testing



## Citing CPLIP

If you use CPLIP in your research, please cite the following:

```
@misc{sajid2024cplip,
  title={CPLIP: Zero-Shot Learning for Histopathology with Comprehensive Vision-Language Alignment},
  author={Sajid Javed, Arif Mahmood, Iyyakutti Iyappan Ganapathi, Fayaz Ali Dharejo1, Naoufel Werghi, Mohammed Bennamoun},
  year={2024},
  }
```

## Acknowledgements

This repository borrows heavily from open-clip, Plip and TiMM's library. Special thanks to the contributors of merlot.

## License

The code and pretrained models are provided under the MIT license. See the LICENSE file for details.
