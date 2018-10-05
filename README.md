# Image-Caption-Generator

Generate Image Captions; i.e Image-to-Text generation.    
This is not image description, but `Caption Generation`.

## Dependencies:
1. `Python 3.x`
2. `Jupyter`
3. `Keras`
4. `Numpy`
5. `Matplotlib`
6. `h5py`
7. `PIL`

## Dataset and Extra UTils:
`Flicker 8k` dataset from [here](https://forms.illinois.edu/sec/1713398) as the initial model train, test, validation samples. Fill in the survey, you'll get a link to dataset in your registered e-mail. The dataset is around `2GB`.    
During first training keras will download the `VGG16` model. It would be used to train the classification model to know the objects.    
Instead of getting the final layer of `VGG16` which contains the probable function; argmax of classification; you'll remove the output layer to get all probable densities. The `VGG16` model itself is 500 MB.

## Usage:

`1. Download the flicker dataset and place it in ../Flicker8k for this working directory.` 
