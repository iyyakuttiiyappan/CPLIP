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


## Pretrained Models

The pretrained model can be downloaded from this [[CPLIP Weights](https://drive.google.com/file/d/1INDVr_IlLFFS7cOLEkgtNUk7nH4CIYDe/view?usp=sharing)].


## Citing CPLIP

If you use CPLIP in your research, please cite the following:

```
@inproceedings{javed2024cplip,
  title={CPLIP: Zero-Shot Learning for Histopathology with Comprehensive Vision-Language Alignment},
  author={Javed, Sajid and Mahmood, Arif and Ganapathi, Iyyakutti Iyappan and Dharejo, Fayaz Ali and Werghi, Naoufel and Bennamoun, Mohammed},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={11450--11459},
  year={2024}
}
```

## Acknowledgements

This repository borrows heavily from open-clip, Plip and TiMM's library. Special thanks to the contributors of merlot.

## License

The code and pretrained models are provided under the MIT license. See the LICENSE file for details.
