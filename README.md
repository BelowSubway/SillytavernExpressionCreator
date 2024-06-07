# Silly Tavern Expression Creation Workflows
ComfyUI workflows to create expressions for Silly Tavern characters.

![2024-06-07 22_27_39](https://github.com/BelowSubway/SillytavernExpressionCreator/assets/172079054/83c22dda-785d-4e36-aba2-041941af4bc3)

## How to use

These are workflows for [ComfyUI](https://github.com/comfyanonymous/ComfyUI). Install and configue ComfyUI as desribed on their page.

After that configure the single fields in the setup group

![grafik](https://github.com/BelowSubway/SillytavernExpressionCreator/assets/172079054/5f8d2687-8482-42d8-9948-cb8b0f161762)

* Character Name: A folder with the character name will be created in the output folder of ComfyUI. It will contain all the necessary images and can be copied to your Silly Tavern characters folder
* Genercal description: The positve prompt that will be used for all expressions.
* Negative Prompt: The negative prompt that will be used for all expressions.
* Load Checkpoint: Checkpoint to use
* Empty Latent Image: Resolution of the images
* Steps & CFG: Settings for the sampler
* (Only Default Expression Creator) UltralyticsDetectorProvider: Model for the face detection, used by the Face Detailer
* (Only ReActor Expression Creator) Load Image: Face that will be used to replace the face in the generated image

Run the workflow and it will automatically create all the different expressions. After all expressions were created you can adjust the specific positive prompt on each single expression. All KSamplers are set to fixed seeds, so only changed expressions will be re-created.
