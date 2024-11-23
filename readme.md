# FLUX DEV: FILL (INPAINT / OUTPAINT), REDUX, CANNY, DEPTH

## מבנה תיקיות ודוגמאות זרימה
```
FLUX FIL (INPAINING-OUTPAINING) +REDUX +CANNY +DEPTH/
├── flux_fill_controlnet_example_workflow.json
├── flux_fill_canny_example_workflow.json
├── flux_fill_redux_example_workflow.json
├── flux_fill_outpaint_example_workflow.json
├── flux_fill_inpaint_example_workflow.json
├── flux_fill_inpaint_example_workflow-crop&stitch.json
├── flux_fill_depth_example_workflow.json
├── workflow screenshot/
├── png original workflow/
├── input picture/
└── readme.md
```

## מודלים בסיסיים

### FLUX1-DEV
- **flux1-dev.safetensors**
- **לינק להורדה**:  
https://huggingface.co/black-forest-labs/FLUX.1-dev/blob/main/flux1-dev.safetensors
- **לשמור בתיקיית**:  
`ComfyUI_windows_portable\ComfyUI\models\unet`

### FLUX.1-schnell
- **flux1-schnell.safetensors**
- **לינק להורדה**:  
https://huggingface.co/black-forest-labs/FLUX.1-schnell/blob/main/flux1-schnell.safetensors
- **לשמור בתיקיית**:  
`ComfyUI_windows_portable\ComfyUI\models\unet`

### VAE Model
- **ae.safetensors**
- **לינק להורדה**:  
https://huggingface.co/black-forest-labs/FLUX.1-dev/blob/main/ae.safetensors
- **לשמור בתיקיית**:  
`ComfyUI_windows_portable\ComfyUI\models\vae`

## Fill (Inpainting/ Outpainting) model
- **flux1-fill-dev.safetensors**
- **לינק להורדה**:  
https://huggingface.co/black-forest-labs/FLUX.1-Fill-dev/blob/main/flux1-fill-dev.safetensors
- **לשמור בתיקיית**:  
`ComfyUI_windows_portable\ComfyUI\models\diffusion_models`

## Redux

### Model Files
1. **flux1-redux-dev.safetensors**
   - **לינק להורדה**:  
   https://huggingface.co/black-forest-labs/FLUX.1-Redux-dev/blob/main/flux1-redux-dev.safetensors
   - **לשמור בתיקיית**:  
   `ComfyUI_windows_portable\ComfyUI\models\style_models`

2. **sigclip_vision_patch14_384.safetensors**
   - **לינק להורדה**:  
   https://huggingface.co/Comfy-Org/sigclip_vision_384/blob/main/sigclip_vision_patch14_384.safetensors
   - **לשמור בתיקיית**:  
   `ComfyUI_windows_portable\ComfyUI\models\clip_vision`

## Canny and Depth

### Models
1. **flux1-canny-dev.safetensors**
   - **לינק להורדה**:  
   https://huggingface.co/black-forest-labs/FLUX.1-Canny-dev
   - **לשמור בתיקיית**:  
   `ComfyUI_windows_portable\ComfyUI\models\diffusion_models`

2. **flux1-depth-dev.safetensors**
   - **לינק להורדה**:  
   https://huggingface.co/black-forest-labs/FLUX.1-Depth-dev
   - **לשמור בתיקיית**:  
   `ComfyUI_windows_portable\ComfyUI\models\diffusion_models`

### LoRA Files
- **flux1-canny-dev-lora.safetensors**
- **flux1-depth-dev-lora.safetensors**
- **לינק להורדה**:
  - https://huggingface.co/black-forest-labs/FLUX.1-Canny-dev-lora
  - https://huggingface.co/black-forest-labs/FLUX.1-Depth-dev-lora
- **לשמור בתיקיית**:  
`ComfyUI_windows_portable\ComfyUI\models\loras`

## Community Flux Controlnets
XLab, InstantX ו-Shakker הוציאו מודלי CONTROLNET המותאמים ל-FLUX

### InstantX Canny Model
- **flux1-dev-fp8.safetensors**
- **לינק להורדה**:  
https://huggingface.co/lllyasviel/flux1_dev/blob/main/flux1-dev-fp8.safetensors
- **לשמור בתיקיית**:  
`ComfyUI_windows_portable\ComfyUI\models\checkpoints`

### Additional Controlnet Files

1. **InstantX Canny**
   - **לינק להורדה**:  
   https://huggingface.co/InstantX/FLUX.1-dev-Controlnet-Canny/blob/main/diffusion_pytorch_model.safetensors
   - **לשנות שם ל**: `instantx_flux_canny.safetensors`
   - **לשמור בתיקיית**:  
   `ComfyUI_windows_portable\ComfyUI\models\controlnet`

2. **Depth Controlnet**
   - **לינק להורדה**:  
   https://huggingface.co/Shakker-Labs/FLUX.1-dev-ControlNet-Depth/blob/main/diffusion_pytorch_model.safetensors
   - **לשנות שם ל**: `Shakker-Labs/FLUX.1-dev-ControlNet-Depth.safetensors`
   - **לשמור בתיקיית**:  
   `ComfyUI_windows_portable\ComfyUI\models\controlnet`

3. **Union Controlnet**
   - **לינק להורדה**:  
   https://huggingface.co/Shakker-Labs/FLUX.1-dev-ControlNet-Union-Pro/blob/main/diffusion_pytorch_model.safetensors
   - **לשנות שם ל**: `FLUX.1-dev-ControlNet-Union-Pro.safetensors`
   - **לשמור בתיקיית**:  
   `ComfyUI_windows_portable\ComfyUI\models\controlnet`

### XLAB Controls
קונטרולים נוספים של XLAB ניתן להוריד מכאן:  
https://huggingface.co/XLabs-AI/flux-controlnet-collections/tree/main

## קישורים שימושיים
- **דף ראשי של FLUX1**:  
https://huggingface.co/black-forest-labs

## בונוס
חלק מקבצי הזרימה כוללים **ComfyUI-Inpaint-CropAndStitch** אשר נותן מיקוד כאשר משתמשים במסכה ותפקידו להתמקד רק באזור ולא לשנות פרטים אחרים בתמונת המקור.

- **לינק להתקנה**:  
https://github.com/lquesada/ComfyUI-Inpaint-CropAndStitch  
או דרך המנג'ר
