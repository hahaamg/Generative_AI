## 吉卜力風格圖像生成器
模型：<a href="https://huggingface.co/nitrosocke/Ghibli-Diffusion">nitrosocke/Ghibli-Diffusion</a>

🧨 Diffusers
```python
from diffusers import StableDiffusionPipeline
import torch

model_name = "nitrosocke/Ghibli-Diffusion"
pipe = StableDiffusionPipeline.from_pretrained(
    model_name,
    torch_dtype=torch.float16,
).to("cuda")
```
> enhancement prompt："masterpiece, ultra high quality, intricate skin details, cinematic lighting"

> negative prompt: "soft blurry, bad anatomy, blurry, disfigured, poorly drawn hands, extra fingers, mutated hands, low quality, worst quality"
<h2>生成結果</h2>
<table>
  <tr>
    <td>img
    </td>
    <td>prompt
    </td>
  </tr>
  
  <tr>
    <td>
      <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week11/img/Ghibli-Diffusion%20(1).webp?raw=true" width="300">
      <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week11/img/Ghibli-Diffusion%20(8).webp?raw=true" width="300">
    </td>
    <td style="padding-left: 15px;">
     ghibli style magical garden with oversized flowers and butterflies
    </td>
  </tr>
   <tr>
    <td>
      <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week11/img/Ghibli-Diffusion%20(7).webp?raw=true" width="300">
    </td>
    <td style="padding-left: 15px;">
     ghibli style mystical forest with glowing mushrooms at twilight
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week11/img/Ghibli-Diffusion%20(6).webp?raw=true" width="300">
    </td>
    <td style="padding-left: 15px;">
     ghibli style old European town with cobblestone streets and lanterns at dusk
    </td>
  </tr>
  <tr>
    <td>
       <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week11/img/Ghibli-Diffusion%20(4).webp?raw=true" width="300">
    </td>
    <td style="padding-left: 15px;">
      ghibli style beautiful Caribbean beach tropical (sunset) 
    </td>
  </tr>
  <tr>
    <td>
       <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week11/img/Ghibli-Diffusion%20(2).webp?raw=true" width="300">
       <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week11/img/Ghibli-Diffusion%20(3).webp?raw=true" width="300">
    </td>
    <td style="padding-left: 15px;">
      ghibli style ice field white mountains ((northern lights)) starry sky low horizon
    </td>
  </tr>
</table>
