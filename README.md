# Stable-diffusion-person
介绍由基于Stable-diffusion的Chilloutmix模型生成高清真实的人像的方法

主要是利用免费的Google Colab的在线环境，免去配置环境的麻烦。 由于是Google的服务，所以需要一点上网的技巧。

## 可以一键运行的Google Colab环境

* Chilloutmix模型：[Colab运行环境](https://colab.research.google.com/drive/1KiwBZ6CaXeuOlpRJMssQ04x2Q0XsGjom?usp=sharing)

* Korean Doll Likeness LoRA模型：[Colab运行环境](https://drive.google.com/file/d/1zgCN52pIbMXsVtVu-wLWrB694iUt2s1r/view?usp=sharing)、[Civitai效果图](https://civitai.com/models/6424/chilloutmix)

## 一些Prompts
```text
<lora:taiwanDollLikeness_v10:0.66>, best quality, ultra high res, photoshoot, (photorealistic:1.4), 1girl, singlet, sleeveless, (light brown hair:1), looking at viewer, smiling, cute, full body

Negative prompt: paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans

Size: 512x768, 
Seed: 4243885665, 
Steps: 24, 
Sampler: DPM++ SDE, 
CFG scale: 8, 
Model hash: 7234b76e42, 
Hires steps: 20, H
Hires upscale: 1.75, 
Hires upscaler: Latent (bicubic antialiased), 
Denoising strength: 0.45


<lora:taiwanDollLikeness_v10:0.66>, best quality, ultra high res, (photorealistic:1.4), 1girl, [loose and oversized black jacket,] [white|red] sports bra, (yoga pants:1), (light brown hair:1.2), looking at viewer, smiling, full body, streets, urban, makeup, wide angle
Negative prompt: paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans
Size: 512x768, 
Seed: [3, 537380690]
Steps: [28, 32, 50, 60]
Sampler: DPM++ SDE Karras, 
CFG scale: [7,8]
Model hash: 7234b76e42, 
Hires steps: 20, 
Hires upscale: 1.75, 
Hires upscaler: Latent (bicubic antialiased), 
Denoising strength: 0.5


<koreanDollLikeness_v10:0.66>, best quality, ultra high res, (photorealistic:1.4), 1woman, sleeveless white button shirt, black skirt, black choker, cute, (Kpop idol), (aegyo sal:1), (platinum blonde hair:1), ((puffy eyes)), looking at viewer, full body, facing front
Negative prompt: paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans, nsfw, nipples
Size: 512x768, 
Seed: 1315543661, 
Steps: 28, 
Sampler: DPM++ SDE Karras, 
CFG scale: 8, 
Model hash: a757fe8b3d, 
Hires steps: 20, 
Hires upscale: 1.75, 
Hires upscaler: Latent (bicubic antialiased), 
Denoising strength: 0.45
```

<!--
https://medium.com/@croath/%E4%BD%8E%E6%88%90%E6%9C%AC%E4%BD%93%E9%AA%8C%E7%94%9F%E6%88%90-ai-%E5%B0%8F%E5%A7%90%E5%A7%90%E7%85%A7%E7%89%87-85ffa7c13cd7
https://www.bilibili.com/video/BV12x4y1V71Q/
-->