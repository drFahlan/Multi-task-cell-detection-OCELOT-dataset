Models:

[Tissue segmentation model weights](https://drive.google.com/drive/folders/1N4dMbkNkbmT6gCFQOlgyMPP1awUWvzxD?usp=sharing): U-Net++ with SE_ResNet50 encoder

[Cell detection baseline model weights](https://drive.google.com/file/d/1KgVAe48TANG1iksj79P22WhubE5JjTmc/view?usp=sharing): Attention U-Net with ResNet34 encoder

[Cell detection with data preparation integration model weights](https://drive.google.com/drive/folders/1QZCg0h3hG0n_b72oTFa3tQXHZXLAN76W?usp=sharing): Attention U-Net with ResNet34 encoder, 4 channel input

[Cell detection with post-processing integration](https://drive.google.com/file/d/1KgVAe48TANG1iksj79P22WhubE5JjTmc/view?usp=sharing): Using baseline model but with different post-processing steps.

How to use models:

1. Download the model from the link above
2. Open the corresponding notebook (e.g., open tissue segmentation modeling notebook for tissue segmentation model)
3. Use the weights in the evaluation section by pasting the path of your downloaded weights to the weight calling code
4. Evaluate the model 
