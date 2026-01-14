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
# Download

https://huggingface.co/Comfy-Org/z_image_turbo/blob/main/split_files/diffusion_models/z_image_turbo_bf16.safetensors
https://huggingface.co/Comfy-Org/z_image_turbo/blob/main/split_files/text_encoders/qwen_3_4b.safetensors
https://huggingface.co/Comfy-Org/z_image_turbo/blob/main/split_files/vae/ae.safetensors
