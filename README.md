# Results on dSprites with "Oval" shape only

## 0. Setup (brief)
- Collect only "oval" shape images (remove "square" and "heart")
- So there are 4 factors (rot, scale, x-pos, y-pos)


## 1. Vanilla-VAE (beta = 1.0)

### (Vanilla-VAE) Losses and Metrics

![recon](https://user-images.githubusercontent.com/44901665/49293764-111df500-f47f-11e8-9c60-1b96d3433057.png)<br />
![kl](https://user-images.githubusercontent.com/44901665/49293768-1418e580-f47f-11e8-940f-9828ef088f8a.png)<br />
![metrics](https://user-images.githubusercontent.com/44901665/49293771-15e2a900-f47f-11e8-8c66-3ab1b54a2fd4.png)<br />

#### KL for individual dims
![vanilla_vae_kl_inds](https://user-images.githubusercontent.com/44901665/49304200-9f06d980-f499-11e8-8ddc-6dae67a4bc65.png)

### (Vanilla-VAE) Latent traversal

  4 examples and each is:
  [ x | z1 | z2 | z3 | ... | z10 ]

![fixed1](https://user-images.githubusercontent.com/44901665/49293799-2004a780-f47f-11e8-85ac-459ddb62941a.gif)<br />
![fixed2](https://user-images.githubusercontent.com/44901665/49293817-2d219680-f47f-11e8-89ab-b32593ae4857.gif)<br />
![fixed3](https://user-images.githubusercontent.com/44901665/49293821-301c8700-f47f-11e8-8b3a-7c01c93510fa.gif)<br />
![random_img](https://user-images.githubusercontent.com/44901665/49293823-327ee100-f47f-11e8-9665-bc4babbf4be3.gif)<br />



## 2. Factor-VAE 

### (Factor-VAE) Losses and Metrics

![recon](https://user-images.githubusercontent.com/44901665/49294464-08c6b980-f481-11e8-8f80-1a11268ea13c.png)<br />
![kl](https://user-images.githubusercontent.com/44901665/49294468-09f7e680-f481-11e8-8cc8-c15de7bcccee.png)<br />
![metrics](https://user-images.githubusercontent.com/44901665/49294470-0b291380-f481-11e8-9a1a-c96ac8979b85.png)<br />

#### KL for individual dims
![factor_vae_kl_inds](https://user-images.githubusercontent.com/44901665/49304139-767edf80-f499-11e8-9e21-7cf87a459837.png)

### (Factor-VAE) Latent traversal

  4 examples and each is:
  [ x | z1 | z2 | z3 | ... | z10 ]
  
![fixed1](https://user-images.githubusercontent.com/44901665/49294480-10865e00-f481-11e8-9c59-5ea2c075ae77.gif)
![fixed2](https://user-images.githubusercontent.com/44901665/49294484-12e8b800-f481-11e8-94b6-436704389c52.gif)
![fixed3](https://user-images.githubusercontent.com/44901665/49294490-154b1200-f481-11e8-842b-17ebffd011e2.gif)
![random_img](https://user-images.githubusercontent.com/44901665/49294497-17ad6c00-f481-11e8-9f61-bcab054b6c62.gif)




## 3. RF-VAE Cheat <!--(Our) Relevance-VAE (aka "split model") -->

### (RF-VAE Cheat) Losses and Metrics

![recon](https://user-images.githubusercontent.com/44901665/49294133-16c80a80-f480-11e8-89c3-0cb387010d0c.png)<br />
![kl](https://user-images.githubusercontent.com/44901665/49294137-1760a100-f480-11e8-83e6-5dd8bf9af33e.png)<br />
![metrics](https://user-images.githubusercontent.com/44901665/49294138-192a6480-f480-11e8-8602-f33ccf5aa476.png)<br />

#### KL for individual dims
![relevance_vae_kl_inds](https://user-images.githubusercontent.com/44901665/49304005-34559e00-f499-11e8-9bc0-1fe3332f940f.png)

### (RF-VAE Cheat) Latent traversal

  4 examples and each is:
  [ x | z1 | z2 | z3 | ... | z10 ]

![fixed1](https://user-images.githubusercontent.com/44901665/49294150-25162680-f480-11e8-99ad-b4b1be79b005.gif)<br />
![fixed2](https://user-images.githubusercontent.com/44901665/49294153-27788080-f480-11e8-9bc9-2a072e88a772.gif)<br />
![fixed3](https://user-images.githubusercontent.com/44901665/49294163-29dada80-f480-11e8-845f-796abc588f32.gif)<br />
![random_img](https://user-images.githubusercontent.com/44901665/49294165-2ba49e00-f480-11e8-8c1c-6583e7033e32.gif)<br />

<!-- ** when z_j goes from -6 to +6 (instead of [-3,+3]):
![fixed1](https://user-images.githubusercontent.com/44901665/49304496-7e8b4f00-f49a-11e8-859a-e909aaffc830.gif)
![fixed2](https://user-images.githubusercontent.com/44901665/49304498-82b76c80-f49a-11e8-95d0-f5c94d9bc8b3.gif)
![fixed3](https://user-images.githubusercontent.com/44901665/49304500-85b25d00-f49a-11e8-8cc3-bb99a5ff0857.gif)
![random_img](https://user-images.githubusercontent.com/44901665/49304503-88ad4d80-f49a-11e8-91af-776bfaafdcf4.gif)
-->


## 4. RF-VAE No-Cheat 

### (RF-VAE No-Cheat) Losses and Metrics

![recon](https://user-images.githubusercontent.com/44901665/49294133-16c80a80-f480-11e8-89c3-0cb387010d0c.png)<br />
![kl](https://user-images.githubusercontent.com/44901665/49294137-1760a100-f480-11e8-83e6-5dd8bf9af33e.png)<br />
![metrics](https://user-images.githubusercontent.com/44901665/49294138-192a6480-f480-11e8-8602-f33ccf5aa476.png)<br />

#### KL for individual dims
![relevance_vae_kl_inds](https://user-images.githubusercontent.com/44901665/49304005-34559e00-f499-11e8-9bc0-1fe3332f940f.png)

### (RF-VAE No-Cheat) Latent traversal

  4 examples and each is:
  [ x | z1 | z2 | z3 | ... | z10 ]

![fixed1](https://user-images.githubusercontent.com/44901665/49294150-25162680-f480-11e8-99ad-b4b1be79b005.gif)<br />
![fixed2](https://user-images.githubusercontent.com/44901665/49294153-27788080-f480-11e8-9bc9-2a072e88a772.gif)<br />
![fixed3](https://user-images.githubusercontent.com/44901665/49294163-29dada80-f480-11e8-845f-796abc588f32.gif)<br />
![random_img](https://user-images.githubusercontent.com/44901665/49294165-2ba49e00-f480-11e8-8c1c-6583e7033e32.gif)<br />

