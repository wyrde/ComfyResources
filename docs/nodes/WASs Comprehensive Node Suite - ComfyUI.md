WASs Comprehensive Node Suite - ComfyUI
========================

# WAS's Comprehensive Node Suite - ComfyUI

* web: https://civitai.com/models/20793/
* repo: https://github.com/WASasquatch/was-node-suite-comfyui

WAS's Comprehensive Node Suite - ComfyUI - WAS#0263 https://github.com/WASasquatch/was-node-suite-comfyui

ComfyUI is an advanced node based UI utilizing Stable Diffusion. It allows you to create customized workflows such as image post processing, or conversions.

Latest Version Download

A node suite for ComfyUI with many new nodes, such as image processing, text processing, and more.
Share Workflows to the /workflows/ directory. Preferably embedded PNGs with workflows, but JSON is OK too. You can use this tool to add a workflow to a PNG file easily
Important Updates

    ASCII is deprecated. The new preferred method of text node output is TEXT. This is a change from ASCII so that it is more clear what data is being passed.

        The was_suit_config.json will automatically set use_legacy_ascii_text to true for a transition period. You can enable TEXT output by setting use_legacy_ascii_text to false

Current Nodes:

    BLIP Analyze Image: Get a text caption from a image, or interrogate the image with a question.

        Model will download automatically from default URL, but you can point the download to another location/caption model in was_suite_config

        Models will be stored in ComfyUI/models/blip/checkpoints/

    SAM Model Loader: Load a SAM Segmentation model

    SAM Parameters: Define your SAM parameters for segmentation of a image

    SAM Parameters Combine: Combine SAM parameters

    SAM Image Mask: SAM image masking

    Image Bounds: Bounds a image

    Inset Image Bounds: Inset a image bounds

    Bounded Image Blend: Blend bounds image

    Bounded Image Blend with Mask: Blend a bounds image by mask

    Bounded Image Crop: Crop a bounds image

    Bounded Image Crop with Mask: Crop a bounds image by mask

    CLIPTextEncode (NSP): Parse Noodle Soup Prompts

    Constant Number

    Dictionary to Console: Print a dictionary input to the console

    Image Analyze

        Black White Levels

        RGB Levels

            Depends on matplotlib, will attempt to install on first run

    Image Blank: Create a blank image in any color

    Image Blend by Mask: Blend two images by a mask

    Image Blend: Blend two images by opacity

    Image Blending Mode: Blend two images by various blending modes

    Image Bloom Filter: Apply a high-pass based bloom filter

    Image Canny Filter: Apply a canny filter to a image

    Image Chromatic Aberration: Apply chromatic aberration lens effect to a image like in sci-fi films, movie theaters, and video games

    Image Color Palette

        Generate a color palette based on the input image.

            Depends on scikit-learn, will attempt to install on first run.

        Supports color range of 8-256

        Utilizes font in ./res/ unless unavailable, then it will utilize internal better then nothing font.

    Image Dragan Photography Filter: Apply a Andrzej Dragan photography style to a image

    Image Edge Detection Filter: Detect edges in a image

    Image Film Grain: Apply film grain to a image

    Image Filter Adjustments: Apply various image adjustments to a image

    Image Flip: Flip a image horizontal, or vertical

    Image Gradient Map: Apply a gradient map to a image

    Image Generate Gradient: Generate a gradient map with desired stops and colors

    Image High Pass Filter: Apply a high frequency pass to the image returning the details

    Image History Loader: Load images from history based on the Load Image Batch node. Can define max history in config file. (requires restart to show last sessions files at this time)

    Image Levels Adjustment: Adjust the levels of a image

    Image Load: Load a image from any path on the system, or a url starting with http

    Image Median Filter: Apply a median filter to a image, such as to smooth out details in surfaces

    Image Mix RGB Channels: Mix together RGB channels into a single iamge

    Image Monitor Effects Filter: Apply various monitor effects to a image

        Digital Distortion

            A digital breakup distortion effect

        Signal Distortion

            A analog signal distortion effect on vertical bands like a CRT monitor

        TV Distortion

            A TV scanline and bleed distortion effect

    Image Nova Filter: A image that uses a sinus frequency to break apart a image into RGB frequencies

    Image Perlin Noise Filter

        Create perlin noise with pythonperlin module. Trust me, better then my implementations that took minutes...

    Image Remove Background (Alpha): Remove the background from a image by threshold and tolerance.

    Image Remove Color: Remove a color from a image and replace it with another

    Image Resize

    Image Rotate: Rotate an image

    Image Save: A save image node with format support and path support. (Bug: Doesn't display image

    Image Seamless Texture: Create a seamless texture out of a image with optional tiling

    Image Select Channel: Select a single channel of an RGB image

    Image Select Color: Return the select image only on a black canvas

    Image Shadows and Highlights: Adjust the shadows and highlights of an image

    Image Size to Number: Get the width and height of an input image to use with Number nodes.

    Image Stitch: Stitch images together on different sides with optional feathering blending between them.

    Image Style Filter: Style a image with Pilgram instragram-like filters

        Depends on pilgram module

    Image Threshold: Return the desired threshold range of a image

    Image Transpose

    Image fDOF Filter: Apply a fake depth of field effect to an image

    Image to Latent Mask: Convert a image into a latent mask

    Image Voronoi Noise Filter

        A custom implementation of the worley voronoi noise diagram

    Input Switch (Disable until * wildcard fix)

    KSampler (WAS): A sampler that accepts a seed as a node inpu

    Load Text File

        Now supports outputting a dictionary named after the file, or custom input.

        The dictionary contains a list of all lines in the file.

    Load Batch Images

        Increment images in a folder, or fetch a single image out of a batch.

        Will reset it's place if the path, or pattern is changed.

        pattern is a glob that allows you to do things like **/* to get all files in the directory and subdirectory or things like *.jpg to select only JPEG images in the directory specified.

    Latent Noise Injection: Inject latent noise into a latent image

    Latent Size to Number: Latent sizes in tensor width/height

    Latent Upscale by Factor: Upscale a latent image by a facto

    MiDaS Depth Approximation: Produce a depth approximation of a single image input

    MiDaS Mask Image: Mask a input image using MiDaS with a desired color

    Number Operation

    Number to Seed

    Number to Float

    Number to Int

    Number to String

    Number to Text

    Random Number

    Save Text File: Save a text string to a file

    Seed: Return a seed

    Tensor Batch to Image: Select a single image out of a latent batch for post processing with filters

    Text Add Tokens: Add custom tokens to parse in filenames or other text.

    Text Add Token by Input: Add custom token by inputs representing single single line name and value of the token

    Text Concatenate: Merge two strings

    Text Dictionary Update: Merge two dictionaries

    Text File History: Show previously opened text files (requires restart to show last sessions files at this time)

    Text Find and Replace: Find and replace a substring in a string

    Text Find and Replace by Dictionary: Replace substrings in a ASCII text input with a dictionary.

        The dictionary keys are used as the key to replace, and the list of lines it contains chosen at random based on the seed.

    Text Multiline: Write a multiline text string

    Text Parse A1111 Embeddings: Convert embeddings filenames in your prompts to embedding:[filename]] format based on your /ComfyUI/models/embeddings/ files.

    Text Parse Noodle Soup Prompts: Parse NSP in a text input

    Text Parse Tokens: Parse custom tokens in text.

    Text Random Line: Select a random line from a text input string

    Text String: Write a single line text string value

    Text to Conditioning: Convert a text string to conditioning.


Text Tokens

Text tokens can be used in the Save Text File and Save Image nodes. You can also add your own custom tokens with the Text Add Tokens node.

The token name can be anything excluding the : character to define your token. It can also be simple Regular Expressions.
Built-in Tokens

    [time]

        The current system microtime

    [time(format_code)]

        The current system time in human readable format. Utilizing datetime formatting

        Example: [hostname]_[time]__[time(%Y-%m-%d__%I-%M%p)] would output: SKYNET-MASTER_1680897261__2023-04-07__07-54PM

    [hostname]

        The hostname of the system executing ComfyUI

    [user]

        The user that is executing ComfyUI

Other Features
Import AUTOMATIC1111 WebUI Styles

When using the latest builds of WAS Node Suite a was_suite_config.json file will be generated (if it doesn't exist). In this file you can setup a A1111 styles import.

    Run ComfyUI to generate the new /custom-nodes/was-node-suite-comfyui/was_Suite_config.json file.

    Open the was_suite_config.json file with a text editor.

    Replace the webui_styles value from None to the path of your A1111 styles file called styles.csv. Be sure to use double backslashes for Windows paths.

        Example C:\\python\\stable-diffusion-webui\\styles.csv

    Restart ComfyUI

    Select a style with the Prompt Styles Node.

        The first ASCII output is your positive prompt, and the second ASCII output is your negative prompt.

You can set webui_styles_persistent_update to true to update the WAS Node Suite styles from WebUI every start of ComfyUI
Recommended Installation:

If you're running on Linux, or non-admin account on windows you'll want to ensure /ComfyUI/custom_nodes, was-node-suite-comfyui, and WAS_Node_Suite.py has write permissions.

    Navigate to your /ComfyUI/custom_nodes/ folder

    git clone https://github.com/WASasquatch/was-node-suite-comfyui/

    Start ComfyUI

        WAS Suite should uninstall legacy nodes automatically for you.

        Tools will be located in the WAS Suite menu.

Alternate Installation:

If you're running on Linux, or non-admin account on windows you'll want to ensure /ComfyUI/custom_nodes, and WAS_Node_Suite.py has write permissions.

    Download WAS_Node_Suite.py

    Move the file to your /ComfyUI/custom_nodes/ folder

    Start, or Restart ComfyUI

        WAS Suite should uninstall legacy nodes automatically for you.

        Tools will be located in the WAS Suite menu.

Installing on Colab

Create a new cell and add the following code, then run the cell. You may need to edit the path to your custom_nodes folder.

    !git clone https://github.com/WASasquatch/was-node-suite-comfyui /content/ComfyUI/custom_nodes/was-node-suite-comfyui

    Restart Colab Runtime (don't disconnect)

        Tools will be located in the WAS Suite menu.

Dependencies:

WAS Node Suite is designed to download dependencies on it's own as needed, but what it depends on can be installed manually before use to prevent any script issues. The dependencies which are not required by ComfyUI are as follows:

    BLIP

        Requires transformers==4.26.1

            You can try to manually install from your /python_embeds/ folder run .\python.exe -m pip install --user --upgrade --force-reinstall transformers==4.26.1

    opencv

    scipy

    pilgram

    timm (for MiDaS and BLIP)

        MiDaS Models (they will download automatically upon use and be stored in /ComfyUI/models/midas/checkpoints/, additional files may be installed by PyTorch Hub)

    img2texture (for Image Seamless Texture node)

    pythonperlin

        Used for the perlin noise. I tried writing three different perlin noise functions but I couldn't get things as fast as this library, even with numpy, and that was really hard to figure out. Haha. I'm just terrible with math. Feel free to PR a in-house version so long as it doesn't take longer than a few seconds. Fastest I got was nearly a minute... Lol

    PythonGit

        For downloading repos (such as BLIP)

Github Repository: https://github.com/WASasquatch/was-node-suite-comfyui

https://civitai.com/user/WAS