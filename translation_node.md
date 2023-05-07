translation_node
========================
comfyui comfy_translation_node
* civit: https://civitai.com/models/42647/comfyui-comfytranslationnode
* repo: https://github.com/laojingwei/comfy_translation_node

comfy_translation_node

Updated --2023 04 24

There is no change in the update function, only a small change has been made to adjust the grouping of nodes and put them into xww-tran. If you have downloaded them before, you do not need to update them. If you want to update them, if you use openIE.txt, please first backup openIE.txt and then update it. If you don't overwrite comfy_translation_node directly, you'll be fine

Gratitude model：https://civitai.com/models/10415/3-guofeng3

For more details, please visit：https://github.com/laojingwei/comfy_translation_node

Description

    can be used on ComfyUI interface node for translation, chinese-english translation, translation youdao and Google API support, a variety of options for your choice;

    CN2EN: Support: translation api switch, whether to open translation, Chinese-English switch, embeddings selection, embeddings weight adjustment;

    Tweak Keywords CN2EN: You can tweak the translated content, making it more flexible to tweak your keywords

Download

git clone git clone https://github.com/laojingwei/comfy_translation_node.git

ZIP download

Position installation and operation before use

    Place the downloaded folder comfy_translation_node under ComfyUI\custom_nodes

    If you want to start ComfyUI is used when you want the browser (just want to use the default browser can skip this step), you can edit openIE. TXT (path: PATH field in ComfyUI\custom_nodes\comfy_translation_node\openIE.txt), add the corresponding browser.exe execution file path to it, for example: PATH="C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe", other fields (*PATHOLD, SAVE*) never move, no matter what value they are do not change! If the ComfyUI code update fails, then you need to reset the other two fields to *PATHOLD=""* and *SAVE="FALSE"*

    Go back to the ComfyUI update folder ComfyUI_windows_portable\update and execute the three files in order. Because this plugin requires the latest code ComfyUI, not update can't use, if you have is the latest (2023-04-15) have updated after you can skip this step

    Go to the root directory and double-click run_nvidia_gpu.bat (or run_cpu.bat) to start ComfyUI. Note that if you did step 2 above, you will need to close the ComfyUI launcher and start again, because the first startup only initialized the browser path, which cannot be read. You will need to start again to open the browser you want. In the future, as long as you do not update the ComfyUI code, you will be able to open your browser every time. If you have an update later, you need to update the code twice before the service takes effect

Instructions for use

    Node addition method: You can find utils by double-clicking into search and output related words or right-click to find utils and click in to search. Both of these nodes can be directly connected to the Text of CLIP Text Encode. CLIP Text Encode accepts text entry, and Text entry can be right-click on CLIP Text Encode. Find the Convert text to input, select it and the text entry will appear on the left side. (This is very important because many nodes can open the text entry in this way.)

    CLIP Text Encode CN2EN

Text input field: Enter keywords

"language": 'AUTO' will not be translated, the original text will be output, 'CN' will be translated into Chinese (note that due to the translation api, please ensure that it is pure English before being translated into Chinese), 'EN' will be translated into English (Chinese and English can be mixed)

"transAPI": 'YOUDAO' uses Youdao api to translate,'GOOGLE' uses Google api to translate (Google call time is slow, generally about 2 seconds, sometimes will call failure, it is recommended to use Youdao translation, speed is very fast, but different translation api translated content is a little different, Which one you choose depends on your preference)

"log": 'CLOSE' does not print logs on the console,'OPEN' prints logs on the console

"embeddings": 'none' is not used. Other: Select the model you want (if there is no model in the embeddingsStrength folder, embeddings and EmbeddingsStrength are not displayed)

"embeddingsStrength": it sets the weight,

Tweak Keywords CN2EN

    Display the input content with CLIP Text Encode CN2EN to display the translated content; Due to the limitations of the translation api, there may be some problems with the translated format, you can correct it here if necessary; If you don't think you want to translate certain words, you can edit specific words, which can make your keywords more perfect and produce better pictures If the tweak_keywords_CN2EN node cannot view content after the ComfyUI code is updated, check whether the folder tweak_keywords_CN2EN exists in the ComfyUI\web\extensions path first, If yes, you can decompress tweak_keywords_CN2EN.zip (path: ComfyUI\custom_nodes\comfy_translation_node\ tweak_Keywords_cn2en.zip). Manually add it to ComfyUI\web\extensions (it is not usually overwritten, I give you a zip pack just in case)
    

https://civitai.com/user/xww911
This model permits users to:

y Use the model without crediting the creator
n Sell images they generate
n Run on services that generate images for money
y Share merges using this model
n Sell this model or merges using this model
y Have different permissions when sharing merges

