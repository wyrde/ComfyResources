assemble_tags_node
========================

# comfyui comfy_assemble_tags_node

* web: https://civitai.com/models/49851/comfyui-comfyassembletagsnode
* repo: https://github.com/laojingwei/comfy_assemble_tags_node

comfy_assemble_tags_node

2023 04-26 Troubleshooting Instructions:

I am very sorry that I overwrote the code of search path display and selected path display when I packaged yesterday. I just found out today that I have uploaded the code to github and civitail again. If you have downloaded it before and want to use the function of path display, Please download the latest code to overwrite this file ComfyUI\custom_nodes\comfy_assemble_tags_node, then go to ComfyUI\web\extensions\select_tags and delete select_tags folder. If you have modified or added your content to tags.xlsx in this folder, please back up and restart ComfyUI

---

It took me over a week to write. Please give me a star if you like, or give me a star on github

gitHub: https://github.com/laojingwei/comfy_assemble_tags_node

Gratitude model：https://civitai.com/models/10415/3-guofeng3

description

comfy_assemble_tags_node is a keyword selection and assembly modification plugin that can help you quickly generate various ai keywords.

It has the following characteristics:

1. It covers most of the keywords used in ai, and makes a lot of classifications, including some common presuppositions, etc.

2. Keywords are marked in Chinese, which is convenient for users who do not speak English to choose.

3, provides the search function, can quickly locate the approximate location of keywords, search the current page can also be global search, save time and energy.

4, with the function of choosing memory, you can see the keywords you selected last time and the path on the home page, convenient modification and adjustment.

5, can be customized to increase keywords, to meet different needs and preferences.

6, you can view the current generated random seeds, easy to copy and share.

7, can split the assembly of keywords, if the keywords are more recommended to use the assembly node, can let you want to modify the follow-up keyword can be faster to locate the keyword position to modify.

Download method

git

git clone https://github.com/laojingwei/comfy_assemble_tags_node.git

zip

ZIP

Installation mode

1. Put the downloaded plug-in folder into this folder ComfyUI_windows_portable\ComfyUI\custom_nodes 2. Restart comfyui software and open the UI interface

Node introduction

Show Seed Displays random seeds that are currently generated

Select Tags Tags Used to select keywords

Assemble Tags (more keywords and often modify is recommended)

Show Tags You can check the keywords selected by the previous nodes, which can be adjusted in more detail here (if the process does not monitor the change after adjusting the keywords, you can disconnect the chain connected with the front and click to generate)

Usage method

1. Double-click the left button to search Select Tags, Assemble Tags, Show Tags and Show Seed to add nodes

2. Right-click Add Node-&gt. xww-&gt; tags-&gt; ... Select the node you want to add

Select Tags:

1. You can enter the corresponding tab to find the keywords you need, or you can use search to search. If \** is added in front of the search, it means to check the contents of all tabs, and the corresponding path will be displayed on the found value. If you do not add \** Indicates that only the content of the current tab is searched, regardless of the global or the current tab, as long as the corresponding value is found, the text in the search box will be converted to green, and it will be white if it cannot be found, and the upper right corner of the corresponding keyword option will be displayed An arrow animation will appear to tell you what you are searching for. 2. Click OK to display the English in reverse. The content in the reverse display here cannot be changed just to show you what you have selected. 3. You can tag the content in it by yourself. Modify or add in the xlsx table 4. The input box on the right side of the option is weight input 5. For more detailed operations, please see the screenshot below

Assemble Tags:

1, can be used with Select Tags, can also be used alone, when used with Select Tags, please right-click in the bottom to find which option you want to change to take the input content, then you can Select Tags connected to the option 2, the options are preset, available without

Show Tags:

1. Keywords can be fine-tuned with Select Tags or Assemble Tags, or can be used alone

Show Seed:

1. It can be connected to VAE Decode, there are as many KSampler seeds as there are in the process, and you can copy corresponding seeds for use. When we generate images, we think the generated images are pretty good. If we wanted to modify the seeds a little bit, we couldn't get the generated seeds, because the seeds shown in KSampler will generate the next seeds immediately after the call. In this case, you can use this node to solve your needs

https://civitai.com/user/xww911
This model permits users to:

y Use the model without crediting the creator
n Sell images they generate
n Run on services that generate images for money
y Share merges using this model
n Sell this model or merges using this model
y Have different permissions when sharing merges

