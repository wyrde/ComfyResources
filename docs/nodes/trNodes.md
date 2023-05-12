trNodes
========================

# trNodes

* web: 
* repo: [https://github.com/trojblue/trNodes](https://github.com/trojblue/trNodes)

custom node modules for ComfyUI

## Installation

1. git clone this repo under ComfyUI/custom_nodes
1. install dependencies:

```
# go to project python folder
cd python_embeded
./python.exe -m pip install -r opencv-python scikit-image blendmodes
```

## Nodes

image_layering:

* Adds 1-3 layers of image on top of one another; will remove white background and use it as transparent layers
* TODO: add alpha control

color_correction:

* Adjusts the color of the target image according to another image; ported from stable diffusion WebUI

model_router:

* Batch reroutes model, clip, vae, condition_1 and condition_2 for cleaner workflow

## Use

* Install nodes
* open ComfyUI
* You'll find the new nodes under trNodes folder
