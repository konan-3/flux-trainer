# flux-trainer
Flux LoRA trainer and full-finetuning.

For now this is a utility wrapper around [kohya](https://github.com/kohya-ss/sd-scripts/tree/sd3) that deals with:
- dataset downloading
- captioning
- easily passing in training args
- packaging and uploading output .tar files

## Setup instructions:
```
conda create --name flux python=3.10
conda activate flux
git clone https://github.com/edenartlab/flux-trainer.git
cd flux-trainer
pip install -r requirements.txt
git clone https://github.com/kohya-ss/sd-scripts.git
cd sd-scripts
git checkout sd3
pip install -r requirements.txt
```

## Training instructions:
1. Create a folder of training images
2. adjust train_config.yaml
3. run main.py (in the root of flux-trainer)
