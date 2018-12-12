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

![recon](https://user-images.githubusercontent.com/44901665/49410620-84e82800-f733-11e8-8b48-157473051c53.png)<br />
![kl](https://user-images.githubusercontent.com/44901665/49410621-887baf00-f733-11e8-8ed5-55e88b2dcdca.png)<br />
![metrics](https://user-images.githubusercontent.com/44901665/49410623-89acdc00-f733-11e8-9d36-78c44d6fd75b.png)<br />
![rvs](https://user-images.githubusercontent.com/44901665/49410631-903b5380-f733-11e8-8656-eb7d6926b0be.png)<br />
![rvh](https://user-images.githubusercontent.com/44901665/49410632-92051700-f733-11e8-86df-c004ed3c0b26.png)<br />

#### Vector "r" over time (during training)
![anim_rvec](https://user-images.githubusercontent.com/44901665/49452196-b3efaf80-f7ae-11e8-9339-e0ec8713cd35.gif)

#### KL for individual dims
![rfvae_learn_kl_inds](https://user-images.githubusercontent.com/44901665/49410666-ba8d1100-f733-11e8-882b-c3597a4ba55b.png)


### (RF-VAE No-Cheat) Latent traversal

  4 examples and each is:
  [ x | z1 | z2 | z3 | ... | z10 ]
  

![fixed1](https://user-images.githubusercontent.com/44901665/49454958-447cbe80-f7b4-11e8-9bfc-18cb9c500ec3.gif)<br />
![fixed2](https://user-images.githubusercontent.com/44901665/49454992-56f6f800-f7b4-11e8-8af0-3b7c06258f41.gif)<br />
![fixed3](https://user-images.githubusercontent.com/44901665/49455000-5a8a7f00-f7b4-11e8-959e-ba24be400b5e.gif)<br />
![random_img0](https://user-images.githubusercontent.com/44901665/49455007-5e1e0600-f7b4-11e8-8dbd-20c8d5a7b186.gif)<br />


## 5. BF-VAE 

### (BF-VAE) Losses and Metrics

![recon](https://user-images.githubusercontent.com/44901665/49827433-4b2ca800-fd57-11e8-9ec9-fda433e86678.png)<br />
![kl](https://user-images.githubusercontent.com/44901665/49827438-4e279880-fd57-11e8-8cdf-83d1af67e5e7.png)<br />
![metrics](https://user-images.githubusercontent.com/44901665/49827440-5089f280-fd57-11e8-96d8-3ac19c70e487.png)<br />
![pv_reg](https://user-images.githubusercontent.com/44901665/49827444-51bb1f80-fd57-11e8-9f64-7b157deb9560.png)<br />

#### Prior Variances "pv" over time (during training)
![anim_pv](https://user-images.githubusercontent.com/44901665/49900541-d9bf2900-fe2c-11e8-992c-b132cf3903be.gif)

#### KL for individual dims
![bfvae_kl_inds](https://user-images.githubusercontent.com/44901665/49899250-2e60a500-fe29-11e8-93e2-3234914da38a.png)

### (BF-VAE) Latent traversal

  4 examples and each is:
  [ x | z1 | z2 | z3 | ... | z10 ]
  
![fixed1](https://user-images.githubusercontent.com/44901665/49827492-6f888480-fd57-11e8-8b20-d8ebe3b9038d.gif)<br />
![fixed2](https://user-images.githubusercontent.com/44901665/49827499-731c0b80-fd57-11e8-9288-ced6a0765103.gif)<br />
![fixed3](https://user-images.githubusercontent.com/44901665/49827504-76af9280-fd57-11e8-9da5-ef5e0507d5f3.gif)<br />
![random_img](https://user-images.githubusercontent.com/44901665/49827510-79aa8300-fd57-11e8-8537-9171871de882.gif)<br />
