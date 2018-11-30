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

## Factor-VAE 

## Relevance-Factor-VAE (aka Split-Factor-VAE)


loss_z:  0.278 (\sum_j ||z_j - z*_j|, note: zj \in [-1,+1])  <br />
loss_x: 15.478 (\sum_i CE(x_i; x*_i); note: dim(x) = 64*64 = 4096)

metric1 = 0.9950  <br />
metric2 = 0.9850
