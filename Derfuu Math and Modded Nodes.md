Derfuu Math and Modded Nodes
========================
ComfyUI Derfuu Math and Modded Nodes
* web: https://civitai.com/models/21558/
* repo: https://github.com/Derfuu/Derfuu_ComfyUI_ModdedNodes#nodes-descriptions

ComfyUI: https://github.com/comfyanonymous/ComfyUI

Github repo + nodes description: https://github.com/Derfuu/Derfuu_ComfyUI_ModdedNodes#nodes-descriptions

Leave suggestions and errors if you meet them

What's new in 0.5.0:

    CombiningArea scaler

    More user-friendly ui names

    ALL nodes description moved to https://github.com/Derfuu/Derfuu_ComfyUI_ModdedNodes#nodes-descriptions

    Tuples and so on moved to their own directory in UI

Simple* introduction:

    Automate calculation depending on image sizes or something you want

    easier(or not) editing multiple values of various nodes

    Math

    Modded scalers

Installing: unzip files in ComfyUI/custom_nodes folder

Should look like this:

For example (v0.5.0) there is an example how scaled ConditioningArea can improve image after scaled latent combining:

Only LatentCombine:

Combining preview:

LatentCombine with scaled ConditioningArea (640*360 to 1360*768):

Example of workflow i made for this located in: /Derfuu_ComfyUI_ModdedNodes/workflow_examples/

model: hPANTYHOSENEKO (sorry, couldn't find link)

negative promp: embedding:verybadimagenegative6400

TROUBLESHOOTING:

If there are troubles with different sizes, aside from *64, this may solve problem: found on GitHUB

This code is at the end of this file: /ComfyUI/comfy/ldm/modules/diffusionmodules/openaimodules.py

NOTES#2:

Debug nodes counts as OUTPUT nodes and can be used withowt image preview or save nodes to get results

P.S.:

All fixes wou can find or post on github, i look there too

If you catch error like: Calculated padded input size per channel: (2 x 82). Kernel size: (3 x 3). Kernel size can't be greater than actual input size. This MAY be because of too high or low offset you give to node
    
https://civitai.com/user/Derfuu
This model permits users to:
y Use the model without crediting the creator
y Sell images they generate
y Run on services that generate images for money
y Share merges using this model
n Sell this model or merges using this model
y Have different permissions when sharing merges