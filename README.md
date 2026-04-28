# Fish ID Model Weights

Pretrained ML model weights for Fish recognition.

**No application code lives in this repo.** Only the model files.

## Files

All files are tracked in this repository with Git LFS:

| File | Size | Architecture | Runtime | Source |
|------|------|-------------|---------|--------|
| `fish_detector.pte` | 78 MB | YOLO v26 nano | ExecuTorch | [Fishial.AI](https://github.com/fishial/fish-identification) |
| `fish_segmenter.pte` | 50 MB | FPN + ResNet18 | ExecuTorch | [Fishial.AI](https://github.com/fishial/fish-identification) |
| `fish_classifier.pte` | 108 MB | ConvNeXt Tiny v7.1 | ExecuTorch | [Fishial.AI](https://github.com/fishial/fish-identification) |
| `fish_classifier_bioclip.pte` | 329 MB | BioCLIP ViT-B/16 | ExecuTorch | [Imageomics/bioclip](https://github.com/Imageomics/bioclip) |

## How they got here

The Fishial and BioCLIP projects publish the source weights under MIT. We converted them to ExecuTorch `.pte` flatbuffer format so they can run on Android via the ExecuTorch runtime.

## License

All model weights in this repo are redistributed under the **MIT License** of their original publishers:

- Fishial models: Copyright (c) 2021 Wye Foundation - Fishial.AI Project
- BioCLIP model: Copyright (c) 2024 Imageomics Institute

See [fishial/fish-identification/LICENSE](https://github.com/fishial/fish-identification/blob/main/LICENSE) and [Imageomics/bioclip/LICENSE](https://github.com/Imageomics/bioclip/blob/main/LICENSE) for the full text.
