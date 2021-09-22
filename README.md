# KaoKore Faces  
Blending FFHQ faces with KaoKore pre-modern Japanese art faces

## KaoKore Dataset  
<img src="https://github.com/laphisboy/stylegan2-pytorch/blob/master/images/kaokore.PNG" />  
source:  
https://github.com/rois-codh/kaokore    
https://arxiv.org/abs/2002.08595

# Created blend_and_project.py  
from projector.py  
referenced:  
https://github.com/justinpinkney/stylegan2/blob/master/blend_models.py  
https://github.com/XingruiWang/Animefy/blob/master/blend.py  

# Results  

Model blend: 
- model trained for 500,000 iteration on FFHQ  
- model further trained for additional 180,000 iteration on KaoKore  

## How model is blended  
<img src="https://github.com/laphisboy/stylegan2-pytorch/blob/master/images/method.PNG" />  

## Result for blend_and_project
<img src="https://github.com/laphisboy/stylegan2-pytorch/blob/master/images/ffhq1.PNG" />  
<img src="https://github.com/laphisboy/stylegan2-pytorch/blob/master/images/ffhq2.PNG" />  

## Result on my face
<img src="https://github.com/laphisboy/stylegan2-pytorch/blob/master/images/me.PNG" />   


# Future Fixes  
Latent space is found by projection on blended model,  
But it would have been better if projection was on FFHQ since the domains would match better.  
