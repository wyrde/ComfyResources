Multiple Subject Workflows
========================
Multiple Subject Workflows
* civit: https://civitai.com/models/21100/
* repo: 

This is a collection of custom workflows for ComfyUI

They can generate multiple subjects. Each subject has its own prompt.

They require some custom nodes to function properly, mostly to automate out or simplify some of the tediousness that comes with setting up these things. You can find the requirements listed in each download's description

There are three methods for multiple subjects included so far:
Latent Couple

Limits the areas affected by each prompt to just a portion of the image

Includes ControlNet and unCLIP (enabled by switching node connections)

From my testing, this generally does better than Noisy Latent Composition

Noisy Latent Composition

Generates each prompt on a separate image for a few steps (eg. 4/20) so that only rough outlines of major elements get created, then combines them together and does the remaining steps with Latent Couple
Character Interaction

This is an """attempt""" at generating 2 characters interacting with each other, while retaining a high degree of control over their looks, without using ControlNets. As you may expect, it's quite unreliable.

We do this by generating the first few steps (eg. 6/30) on a single prompt encompassing the whole image that describes what sort of interaction we want to achieve (+background and perspective, common features of both characters help too).

Then, for the remaining steps in the second KSampler, we add two more prompts, one for each character, limited to the area where we "expect" (guess) they'll appear, so mostly just the left half/right half of the image with some overlap.

I'm not gonna lie, the results and consistency aren't great. If you want to try it, some settings to fiddle around with would be at which step the KSampler should change, the amount of overlap between character prompts and prompt strengths. From my testing, the closest interaction I've been able to get out of this was a kiss, I've tried to go for a hug but with no luck.

The higher the step that you switch KSamplers at, the more consistently you'll get the desired interaction, but you'll lose out on the character prompts (I've been going between 20-35% of total steps). You may be able to offset this a bit by increasing character prompt strengths


https://civitai.com/user/Bocian