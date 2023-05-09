ComfyUI CLIP BLIP Node
========================

ComfyUI CLIP BLIP Node

* web: https://civitai.com/models/42974/comfyui-clip-blip-node
* repo: 

CLIPTextEncode Node with BLIP
Dependencies

    Fairscale>=0.4.4 (NOT in ComfyUI)

    Transformers==4.26.1 (already in ComfyUI)

    Timm>=0.4.12 (already in ComfyUI)

    Gitpython (already in ComfyUI)

Local Installation

Inside ComfyUI_windows_portable\python_embeded, run:

    python.exe -m pip install fairscale

And, inside ComfyUI_windows_portable\ComfyUI\custom_nodes\, run:

    git clone https://github.com/paulo-coronado/comfy_clip_blip_node

Google Colab Installation

Add a cell anywhere, with the following code:

    !pip install fairscale
    !cd custom_nodes && git clone https://github.com/paulo-coronado/comfy_clip_blip_node

How to use

* Add the CLIPTextEncodeBLIP node;
* Connect the node with an image and select a value for min_length and max_length;
* Optional: if you want to embed the BLIP text in a prompt, use the keyword BLIP_TEXT (e.g. "a photo of BLIP_TEXT", medium shot, intricate details, highly detailed).

Acknowledgement
* The implementation of CLIPTextEncodeBLIP relies on resources from BLIP, ALBEF, Huggingface Transformers, and timm. We thank the original authors for their open-sourcing.

![hr-fix_00018_](../media/hr-fix_00018_.png)
![Screenshot_2](../media/Screenshot_2.png)
![312030](../media/312030.png)
![hamb](../media/hamb.png)
![312029](../media/312029.png)
![312032](../media/312032.png)

https://civitai.com/user/PauloCoronado
y Use the model without crediting the creator
n Sell images they generate
n Run on services that generate images for money
y Share merges using this model
n Sell this model or merges using this model
y Have different permissions when sharing merges
