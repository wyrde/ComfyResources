WASs ComfyUI Workspaces
========================
WAS's ComfyUI Workspaces (HR-Fix and more!)
* civit: https://civitai.com/models/20215/wass-comfyui-workspaces-hr-fix-and-more
* repo: 

These are worksapces to load into ComfyUI for various tasks such as HR-Fix with AI Model Upscaling

Note: WAS's Comprehensive Node Suite (WAS Node Suite) has a bloom filter now which works similar, except provides a high frequency pass to base the bloom off of. This is more accurate and used in screen-space bloom like in video games.

Requirements:

HR-Fix Bloom Workspace depends on Filters Suite V3, and NSP CLIPTextEncode nodes from here: https://civitai.com/models/20793/was-node-suites-comfyui

HR-Fix Usage:

* Extract "ComfyUI-HR-Fix_workspace.json" (or whatever the worksapce is called)
* Load workspace with the "Load" button in the right-hand menu and select "ComfyUI-HR-Fix_workspace.json"
* Select your desired diffusion model
* Select VAE model or use diffusion models vae
* Select your desired upscale model
* change prompt and sampling settings as seen fit.
    * (currently v1 set to 512x768 x4= 2048x3072, v2 has a resize so final size is 1024x1536)

https://civitai.com/user/WAS