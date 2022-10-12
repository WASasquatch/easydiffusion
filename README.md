# Stability.AI Easy Diffusion ![visitors](https://visitor-badge.glitch.me/badge?page_id=EasyDiffusion-github&left_color=blue&right_color=orange) 

Stability.AI Easy Diffusion is a Google Colab Notebook designed to be a relatively easy to use all-in-one suite for stable diffusion. It is being improved with features frequently. 

### Features
- Text to Image Stable Diffusion
- Image to Image Stable Diffusion
- Inpainting Stable Diffusion
- Enable or Disable NSFW Filtering (Gaussian Blurred Images)
- Cached Pipes - Cache pipes to disk for faster loading between pipe types.
- Optional Attention Slicing
- Define a HF Model not listed by selecting the `MODEL_ID` text and writing in your own model ID, or select from the drop down arrow list of predefined models.
- Stable Diffusion Concept support
- Use local, or remote init images or mask images. 
- Use a text file of init images, masks, or prompts to do batches.
- [Noodle Soup Prompts](https://github.com/WASasquatch/noodle-soup-prompts) support for prompts.
- Random word support in `[word1|word2|word3]` syntax, or multiple words in `[^#|word1|word2|word3] format, where `#` is a number determining how many random words from the list to use.
- Negative prompt support built into normal prompts, denote negative prompts at the end of your prompt with `--`. For example `Positive prompt here--Negative prompt here`
- Recursive Evolution - Feed your diffusion result into img2img for evolution. Can be used to create cool animations like below:<br>
&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://s4.gifyu.com/images/ezgif-2-6d22dcfde1_sm.gif">
- Image Upscaling (Easy Diffusion can be used as a image processor by enabling `SKIP_DIFFUSION_RUN`)
  - GOBIG - Slice a upscaled image up into small tiles to diffuse with img2img, and then compile the final upscaled result. Useful for adding diffusion details at higher resolutions where VRAM wouldn't allow.
  - IMG2IMG - Basic Image to Image upscaling, very VRAM intensive
  - GFPGAN - GFPGAN Face Enhancement
  - CodeFormer - CodeFormer Face Enhancement + Real-ESRGAN
  - Real-SRGAN - Real-ESRGAN Super Resolution
- Image Processing
  - Sharpening
  - Chromatic Aberration
  - Median Filter
  - Depth Output
  - Fake Depth of Field
  - Tileable Texture Output
- CLIP Interrogate
  - Interrogate diffusion results with various CLIP models
  - Interrogate batch images without diffusion (with `SKIP_DIFFUSION_RUN`)
  

Easy Diffusion is maintained by WASasquatch (WAS#0263)

## Stablity.AI Model Terms of Use

This model is open access and available to all, with a CreativeML OpenRAIL-M license further specifying rights and usage.

The CreativeML OpenRAIL License specifies:

1. You can't use the model to deliberately produce nor share illegal or harmful outputs or content

2. CompVis claims no rights on the outputs you generate, you are free to use them and are accountable for their use which must not go against the provisions set in the license

3. You may re-distribute the weights and use the model commercially and/or as a service. If you do, please be aware you have to include the same use restrictions as the ones in the license and share a copy of the CreativeML OpenRAIL-M to all your users (please read the license entirely and carefully)

Please read the full license here: https://huggingface.co/spaces/CompVis/stable-diffusion-license 
