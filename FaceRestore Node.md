FaceRestore Node
========================
ComfyUI - FaceRestore Node
* civit: https://civitai.com/models/24690/
* repo:

FaceRestore node for ComfyUI. To install copy the facerestore directory from the zip to the custom_nodes directory in ComfyUI.

I bodged this together in an afternoon. You might need to pip install a package if it doesn't work at first.

You'll need codeformer-v0.1.0.pth or GFPGANv1.4.pth in your models/upscale_models directory. The node uses another model for face detection which it will download and put in models/facedetection




https://civitai.com/user/m99