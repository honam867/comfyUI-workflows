apt-get update && apt-get install aria2 -y

## Diffusion Models

cd /workspace/runpod-slim/ComfyUI/models/diffusion_models

aria2c -x 16 -s 16 -o "z_image_turbo_bf16.safetensors" "https://huggingface.co/Comfy-Org/z_image_turbo/resolve/main/split_files/diffusion_models/z_image_turbo_bf16.safetensors"

## Encoders

cd /workspace/runpod-slim/ComfyUI/models/text_encoders

aria2c -x 16 -s 16 -o "qwen_3_4b.safetensors" "https://huggingface.co/Comfy-Org/z_image_turbo/resolve/main/split_files/text_encoders/qwen_3_4b.safetensors"

# VAE

cd /workspace/runpod-slim/ComfyUI/models/vae

aria2c -x 16 -s 16 -o "ae.safetensors" "https://huggingface.co/Comfy-Org/z_image_turbo/resolve/main/split_files/vae/ae.safetensors"

# Upscale model

cd /workspace/runpod-slim/ComfyUI/models/upscale_models

aria2c -x 16 -s 16 -o "4x_NMKD-Superscale-SP_178000_G.pth" "https://huggingface.co/gemasai/4x_NMKD-Superscale-SP_178000_G/resolve/main/4x_NMKD-Superscale-SP_178000_G.pth"


## Lora:

cd /workspace/runpod-slim/ComfyUI/models/loras

wget --content-disposition -O smartphone_snapshot_v8.safetensors "https://civitai.com/api/download/models/2517015?token=814a0d5268df88f73b17873afc7ac17f"

## Controlnet

cd /workspace/runpod-slim/ComfyUI/models/model_patches

aria2c -x 16 -s 16 \
  -o "Z-Image-Turbo-Fun-Controlnet-Union-2.1-2601-8steps.safetensors" \
  "https://huggingface.co/alibaba-pai/Z-Image-Turbo-Fun-Controlnet-Union-2.1/resolve/main/Z-Image-Turbo-Fun-Controlnet-Union-2.1-2601-8steps.safetensors"

# Download

https://huggingface.co/Comfy-Org/z_image_turbo/blob/main/split_files/diffusion_models/z_image_turbo_bf16.safetensors
https://huggingface.co/Comfy-Org/z_image_turbo/blob/main/split_files/text_encoders/qwen_3_4b.safetensors
https://huggingface.co/Comfy-Org/z_image_turbo/blob/main/split_files/vae/ae.safetensors
