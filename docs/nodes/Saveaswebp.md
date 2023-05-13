Saveaswebp
========================

# ComfyUI-Saveaswebp

* web: 
* repo: https://github.com/Kaharos94/ComfyUI-Saveaswebp


Save a picture as Webp file in Comfy + Workflow loading

## Description:

This adds a custom node to save a picture as a Webp File and also adds a script to Comfy to drag and drop generated webpfiles into the UI to load the workflow.

I've added a compression slider and a lossy/lossless option. The compression slider is a bit misleading.

In lossless mode, it only affects the "effort" taken to compress where 100 is the smallest possible size and 1 is the biggest possible size, it's a tradeoff for saving speed.

In lossy mode, that's the other way around, where 100 is the biggest possible size with the least compression and 1 is the smallest possible size with maximum compression.

On default it's set to lossy with a compression of 80, below are examples for that.
