README
========================

# README for ComfyUI Resources

* web: [https://wyrde.github.io/ComfyResources/](https://wyrde.github.io/ComfyResources/) (this page)
* web1: 
* repo: [https://github.com/wyrde/ComfyResources](https://github.com/wyrde/ComfyResources)

## Node List

* Click `Nodes` above or [click here](./nodes/index.md) for the wiki.
* Click [here](https://github.com/wyrde/ComfyResources/tree/main/docs/nodes) for the repo.

## Purpose

* This is a simple copy of the ComfyUI resources pages on [Civitai.com](https://civitai.com/tag/comfyui)
* It is meant to be an quick source of links and is not comprehensive or complete. Only the top page of each listing is here.
* If you are the owner of a resource and want it removed, do a local fork removing it on github and a PR. (This is the easiest way to authenticate ownership.)
* Links to resources and sources other than those hosted by civit are okay! 
* If you're the owner of a resource and want to improve the listing, add links, or even an archive, open PRs with the changes. Though in most cases I'd much rather a link to github, huggingfaces, or other repo be provided rather than releases. If you desire images/archives included in a listing, please create a subdirectory and place everything in there to keep the main area tidy.
  * example:

```
    nodename\
             readme.md
             node.py
             node.zip
             node.png
```

* If you know of a resource missing from here, ask the author to open a PR adding it (or permission to do so)! That'd be awesome. (:

##  md fille format
This page can be used as a template.

```
filename
========================

# full project name

* web: URL for project website (usually civitai)
* web1: alternate URL. For each additional, add a number
* repo: git-or other cvs system-enabled repository

main body: the rest is project text with no standard format
```

* The file name is also a short name for the project. In most caes, "Comfy" or "ComfyUI" can be left off since, logically, that's what all the files in this repo are for.
* The blank lines are important for formatting
* The `*` are for generating a list
* websites are places the nodes/files can be downloaded
* social media and other links should go in the main body


## Special Mention

* ltdrdata's [Comfy Manager](https://github.com/ltdrdata/ComfyUI-Manager)
  * help organize and install various custom nodes


happy nodes,

--wyn
