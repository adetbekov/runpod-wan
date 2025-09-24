## Downloading loras:

note: if civitai requires token, set it like so:
```bash
token=YOUR_TOKEN
```
LORAs:
```bash
# WAN22 lightx2v high for I2V
aria2c -x16 -s16 -d /workspace/models/loras -o Wan2.2-Lightning_I2V-A14B-4steps-lora_HIGH_fp16.safetensors --continue=true https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/Wan22-Lightning/Wan2.2-Lightning_I2V-A14B-4steps-lora_HIGH_fp16.safetensors
# WAN22 lightx2v low for I2V
aria2c -x16 -s16 -d /workspace/models/loras -o Wan2.2-Lightning_I2V-A14B-4steps-lora_LOW_fp16.safetensors --continue=true https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/Wan22-Lightning/Wan2.2-Lightning_I2V-A14B-4steps-lora_LOW_fp16.safetensors

# WAN22 lightx2v high for T2V
aria2c -x16 -s16 -d /workspace/models/loras -o Wan2.2-Lightning_T2V-v1.1-A14B-4steps-lora_HIGH_fp16.safetensors --continue=true https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/Wan22-Lightning/Wan2.2-Lightning_T2V-v1.1-A14B-4steps-lora_HIGH_fp16.safetensors
# WAN22 lightx2v low for T2V
aria2c -x16 -s16 -d /workspace/models/loras -o Wan2.2-Lightning_T2V-v1.1-A14B-4steps-lora_LOW_fp16.safetensors --continue=true https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/Wan22-Lightning/Wan2.2-Lightning_T2V-v1.1-A14B-4steps-lora_LOW_fp16.safetensors

# phut hon dance
aria2c -x16 -s16 -d /workspace/models/loras -o dbc.safetensors --continue=true "https://civitai.com/api/download/models/1542806?type=Model&format=SafeTensor&token=${token}"
# trigger words: 
# dabaichui
# making dabaichui motion
# example:  dabaichui，the person holds their head with both hands and twists their waist and hips left and right ，making dabaichui motion

# Hulk transformation:
aria2c -x16 -s16 -d /workspace/models/loras -o Hulk_epoch35.safetensors --continue=true "https://civitai.com/api/download/models/1588339?type=Model&format=SafeTensor&token=${token}"
# trigger words: 
# h01k green hulk transformation
# examples:
# The video shows a person looking forward. Slowly, the h01k green hulk transformation begins. Their muscles start to swell, veins bulge beneath their skin, and their face tightens with strain. Their skin gradually shifts to green as their body continues to grow. Their clothes begin to tear apart under the pressure. The transformation completes as the Hulk emerges, standing tall and roaring.
# The video shows an Asian man looking forward. Slowly, the h01k green hulk transformation begins. His muscles start to swell, veins bulge beneath his skin, and his face tightens with strain. His skin gradually shifts to green as his body continues to grow. His clothes begin to tear apart under the pressure. The transformation completes as the Hulk emerges, standing tall and roaring.
# The video shows an elderly man looking forward. Slowly, the h01k green hulk transformation begins. His muscles start to swell, veins bulge beneath his skin, and his face tightens with strain. His skin gradually shifts to green as his body continues to grow. His clothes begin to tear apart under the pressure. The transformation completes as the Hulk emerges, standing tall and roaring

# WAN missionary
aria2c -x16 -s16 -d /workspace/models/loras -o wan2.2_i2v_highnoise_pov_missionary_v1.0.safetensors --continue=true "https://civitai.com/api/download/models/2098405?type=Model&format=SafeTensor&token=${token}"
aria2c -x16 -s16 -d /workspace/models/loras -o wan2.2_i2v_lownoise_pov_missionary_v1.0.safetensors --continue=true "https://civitai.com/api/download/models/2098396?type=Model&format=SafeTensor&token=${token}"
# Important parts of the prompt:
# with her legs spread having sex with a man
# ...
# A man is thrusting his penis back and forth inside her vagina at the bottom of the screen
# {Movement is fast with bouncing breasts|Movement is slow}
# Her breasts are {small|medium sized|large}

# WAN 2.2 sigma face
aria2c -x16 -s16 -d /workspace/models/loras -o wan2_2_14b_i2v_sigma_000002100_high_noise.safetensors --continue=true "https://civitai.com/api/download/models/2147746?type=Model&format=SafeTensor&token=${token}"
# trigger words:
# ... doing sigma face expression

# WAN i2v orgasm
aria2c -x16 -s16 -d /workspace/models/loras -o wan2.2_i2v_orgasm_high_14b.safetensors --continue=true "https://civitai.com/api/download/models/2178013?type=Model&format=SafeTensor&token=${token}"

aria2c -x16 -s16 -d /workspace/models/loras -o wan2.2_i2v_orgasm_low_14b.safetensors --continue=true "https://civitai.com/api/download/models/2178018?type=Model&format=SafeTensor&token=${token}"
# trigger words:
# She is having an orgasm. Her body shudders and shivers as a profound, guttural moan of sexual pleasure escapes her lips, her face a portrait of sublime ecstasy as she reaches the peak of her orgasm.

# WAN 2.2 Oral Insertion
aria2c -x16 -s16 -d /workspace/models/loras -o wan2.2-i2v-oral-insertion-v1.0.zip --continue=true "https://civitai.com/api/download/models/2121297?type=Model&format=Diffusers&token=${token}"
# unzipped:
# wan2.2-i2v-high-oral-insertion-v1.0.safetensors
# wan2.2-i2v-low-oral-insertion-v1.0.safetensors
# trigger words:
# A man appears and she sucks his penis
```