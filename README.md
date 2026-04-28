# Fish Id Model Weights

**No application code lives in this repo.** Only the model files.

## Files

All files are attached to the [v1.0 release](https://github.com/ProspatLtd/Fishy-models/releases/tag/v1.0):

| File | Size | Architecture | Source |
|------|------|-------------|--------|
| `fish_detector.pte` | 78 MB | YOLO v26 nano (TorchScript Lite) | [Fishial.AI](https://github.com/fishial/fish-identification) |
| `fish_segmenter.pte` | 50 MB | FPN + ResNet18 (TorchScript Lite) | [Fishial.AI](https://github.com/fishial/fish-identification) |
| `fish_classifier.pte` | 108 MB | ConvNeXt Tiny v7.1 (TorchScript Lite) | [Fishial.AI](https://github.com/fishial/fish-identification) |
| `fish_classifier_bioclip.pte` | 329 MB | BioCLIP ViT-B/16 (TorchScript Lite) | [Imageomics/bioclip](https://github.com/Imageomics/bioclip) |

## How they got here

The Fishial and BioCLIP projects publish the source weights under MIT. We converted them to PyTorch Lite Interpreter format (`.pte`) so they can run on Android via `pytorch_android_lite`. Details of the conversion pipeline are in the main [Fishy README](https://github.com/ProspatLtd/Fishy).

## License

All model weights in this repo are redistributed under the **MIT License** of their original publishers:

- Fishial models: Copyright (c) 2021 Wye Foundation - Fishial.AI Project
- BioCLIP model: Copyright (c) 2024 Imageomics Institute

See [fishial/fish-identification/LICENSE](https://github.com/fishial/fish-identification/blob/main/LICENSE) and [Imageomics/bioclip/LICENSE](https://github.com/Imageomics/bioclip/blob/main/LICENSE) for the full text.
