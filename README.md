# jojo-gan

## Improvements

Added support for `restyle` GAN inverter which performs better than the already existing `e4e`. This also improves the overall performance of JoJoGAN. Also created well-documented and modular Python scripts to easily pre-train and fine-tune JoJoGAN. 

## Usage

- First, put the target image in the <a href="test_input">test_input</a> directory. 
- Then download necessary data and models using `python3 download_data.py`.
- To use a pretrained JoJoGAN model, run `python3 pretrained_style.py`. To use some other pretrained style, change the value of the style parameter in line 105 from the set of options mentioned in the comment above it.
- Otherwise, to fine-tune a StlyeGAN2 model for a custom style, run `python3 finetune_style.py`. The styles need to be present in the <a href="style_images"> style_images </a> directory and mentioned in line 117 as a list.

## Acknowledgements

This code borrows from <a href="https://github.com/mchong6/JoJoGAN">JoJoGAN</a> and <a href="https://github.com/yuval-alaluf/restyle-encoder">ReStyle</a>.
