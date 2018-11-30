# Results on dSprites with "Oval" shape only

## 0. Setup (brief)
- Collect only "oval" shape images (remove "square" and "heart")
- So, there are 4 factors (rot, scale, x-pos, y-pos)


## 1. Vanilla-VAE (beta = 1.0)

### (Vanilla-VAE) Losses and Metrics

![recon](https://user-images.githubusercontent.com/44901665/49293764-111df500-f47f-11e8-9c60-1b96d3433057.png)<br />
![kl](https://user-images.githubusercontent.com/44901665/49293768-1418e580-f47f-11e8-940f-9828ef088f8a.png)<br />
![metrics](https://user-images.githubusercontent.com/44901665/49293771-15e2a900-f47f-11e8-8c66-3ab1b54a2fd4.png)<br />

### (Vanilla-VAE) Latent traversal

  4 examples and each is:
  [ x | z1 | z2 | z3 | ... | z10 ]

![fixed1](https://user-images.githubusercontent.com/44901665/49293799-2004a780-f47f-11e8-85ac-459ddb62941a.gif)<br />
![fixed2](https://user-images.githubusercontent.com/44901665/49293817-2d219680-f47f-11e8-89ab-b32593ae4857.gif)<br />
![fixed3](https://user-images.githubusercontent.com/44901665/49293821-301c8700-f47f-11e8-8b3a-7c01c93510fa.gif)<br />
![random_img](https://user-images.githubusercontent.com/44901665/49293823-327ee100-f47f-11e8-9665-bc4babbf4be3.gif)<br />

## 2. Factor-VAE 



## 3. (Our) Relevance-VAE (aka "split model")

### (Relevance-VAE) Losses and Metrics

![recon](https://user-images.githubusercontent.com/44901665/49294133-16c80a80-f480-11e8-89c3-0cb387010d0c.png)<br />
![kl](https://user-images.githubusercontent.com/44901665/49294137-1760a100-f480-11e8-83e6-5dd8bf9af33e.png)<br />
![metrics](https://user-images.githubusercontent.com/44901665/49294138-192a6480-f480-11e8-8602-f33ccf5aa476.png)<br />


### (Relevance-VAE) Latent traversal

  4 examples and each is:
  [ x | z1 | z2 | z3 | ... | z10 ]

![fixed1](https://user-images.githubusercontent.com/44901665/49294150-25162680-f480-11e8-99ad-b4b1be79b005.gif)<br />
![fixed2](https://user-images.githubusercontent.com/44901665/49294153-27788080-f480-11e8-9bc9-2a072e88a772.gif)<br />
![fixed3](https://user-images.githubusercontent.com/44901665/49294163-29dada80-f480-11e8-845f-796abc588f32.gif)<br />
![random_img](https://user-images.githubusercontent.com/44901665/49294165-2ba49e00-f480-11e8-8c1c-6583e7033e32.gif)<br />

