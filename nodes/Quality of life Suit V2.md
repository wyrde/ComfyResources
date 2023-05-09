Quality of life Suit V2
========================
# ComfyUI "Quality of life Suit:V2" (auto Update,Chat GPT , DallE-2 ,Math, ... and more )

* web: https://civitai.com/models/21996
* repo: https://github.com/omar92

If you like my work Kindly like,rate and comment XD

These nodes are for : ComfyUI
ComfyUI:

ComfyUI is an advanced node based UI utilizing Stable Diffusion. It allows you to create customized workflows such as image post-processing, or conversions.

Auto Update:

-when you run comfyUI, the suit will generate a config file

The file looks like this :
{

"autoUpdate": true,

"branch": "main",

"openAI_API_Key": "sk-#################################"

}

this file is used to control Auto update, and to manage any other settings the tool requires

File Description:
"autoUpdate": can be (true) or (false),
"branch": default is ("main")

other options for branch:

    "v2.1.X": means it will only update bug fixes for v2 version.

    "main" means it will always be on latest stable build, this may add new nodes suddenly (also usually it assume you update comfy)

    "develop": it will contain latest stuff I'm working on now, but may contain bugs

"openAI_API_Key": if you want to use the ChatGPT or Dall-E2 features, you need to add your open-AI API key, you can get it from (Account API Keys - OpenAI API)
How to use

    you must update comfyUI first before using this version

As this version relies heavily on the new feature of comfyUI : the ability to switch inputs to be widgets and widgets to be inputs

    Download the zip file.

    Extract to ..\ComfyUI\custom_nodes : like this image :

    restart comfy if it was running (reload web, not enough)

    you will find my nodes under new group O/…

    You can check the workflow folder to find great examples of how to use the tool

Kindly be notified that you can load the images in the downloaded ZIP/workflows in comfyUI to load the workflow that was used to generate it

Current Nodes:

//7/4/2023 -----------------------------------------------------------------

    selectLatentFromBatchNode
    if you generate multiple images, it allows you to pick which to use
    for example, if you generate 4 images, it allows you to select 1 of them to do further processing on it

    or you can use it to process them sequentially

    NSP
    this node allow you to select random value from SoupPrompts file

    equations
    - this node allow you to perform math equations on the input
    - there are two variants
    - 1 input (X)
    - 2 inputs (X,Y)
    (you can convert the x and y to inputs by right click on them, so you can use values from another node)

    if you like this node tell me i can enhance it so you can select inputs number

// 22/3/2023 -----------------------------------------------------------------

OpenAI Nodes

OpenAI ChatGPT and DALLE-2 API as nodes, so you can use them to enhance your workflow
ChatGPT-Advanced

    Load_openAI
    to initialize openAI for next nodes

Advanced ChatGPT nodes

    chat_message :
    create a message to send it to chatGPT

    combine_chat_messages:
    used to group messages together before sending them to chatGPT

    Chat_Completion:
    the magic node this node will send the messages to ChatGPT and receive response from it , the response will be the output string

    debug_Completion:
    this to help you check the whole response

in this workflow, I used ChatGPT to create the prompt,

    at start, I send 2 messages to ChatGPT

    first message is to tell ChatGPT how to behave and what is the prompt format that I need from him

    in the second message I send what I want in this case young girl dancing (I added young, so her clothes become decent XD don't misunderstand me please )

    after that I feed the messages to the completion node “it is called like that in their API sorry”

    and congrats, you have a nice input for your image

DallE-2 Image nodes

    create_image:
    used to create and image using DALLE-2 for now only 1 image each time, will update it in next patch to allow multiple images

    variation_image:
    this node will generate variations similar to the image you send to it

this is a full workflow where

1- use ChatGPT to generate a prompt

2- send that prompt to DALLE-2

3- give the generated image to Stable Diffusion to paint over it

4- use DALLE-2 to create variations from the output

ChatGPT-simple

This node harnesses the power of chatGPT, an advanced language model that can generate detailed image descriptions from a small input.

    You need to have OpenAI API key , which you can find at https://beta.openai.com/docs/developer-apis/overview

    Once you have your API key, add it to the api_key.txt file

I have made it a separate file, so that the API key doesn't get embedded in the generated images.

<you can load this image in comfyUI to load the workflow>

String Suit

add multiple nodes to support string manipulation also a tool to generate image from text

    String:
    node that can hold string (text)

    Debug String
    this node will write the string on the console

    Concat string
    this node is used to combine two strings together

    Trim string
    this is used to remove any extra spaces at the start or the end of a string

    Replace string & replace string advanced
    used to replace part of the text by another part

    >>>> String2image <<<<
    this node will generate an images based on a text, which can be used with controlNet to add text to the image.
    — the tool support fonts “add the font you want in fonts folder”
    “If you load the example image in comfyUI the workflow that generated it will be loaded”

    >>>>CLIPStringEncode <<<
    The normal ClipTextEncode node but this one receive the text from the string node, so you don't have to retype your prompt twice anymore

in this example I used depth filter but if you are using WAS nodes you can convert the text to canny using WAS canny filter it will give much better results with the canny controlNet

Other tools

    LatentUpscaleMultiply:
    it is a variant from the original LatentUpscale tool but instead of using width and height you use a multiply number
    for example, if the original images dimensions are (512,512) and the mul values were (2,2) the result image will be (1024,1024)
    also you can use it to downscale if needed by using fractions ex:(512,512) mul (.5,.5) → (256,256)
    Node Path: O/Latent/LatentUpscaleMultiply


there are also many brilliant nodes in this package
WAS's Comprehensive Node Suite - ComfyUI | Stable Diffusion Other | Civitai

thanks for reading my message, I hope that my tools will help you.

Discord: Omar92#3374

Githup: omar92 (omar abdelzaher sleam) (github.com)

https://civitai.com/user/omar92
