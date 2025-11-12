# MTU Net for hemorrhage classification and segmentation on non contrast head CT

## Features
- EfficientNetV2 encoder with shared multi task head
- FiLM class guided decoding that conditions decoder features on class probabilities
- Self attention blocks in the decoder
- Uncertainty weighted loss that balances classification and segmentation
- Patient wise cross validation and simple inference

## Quick start
```bash
pip install -r requirements.txt
python train.py --img_dir data/images --mask_dir data/masks --labels data/labels.json --out_dir weights
