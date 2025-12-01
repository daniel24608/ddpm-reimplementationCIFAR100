

## Original Paper & Repo
https://arxiv.org/abs/2006.11239
https://github.com/hojonathanho/diffusion


## Training settings:
python train.py --dataset cifar10 --train-device cuda:0 --epochs 100 --chkpt-intv 10 --image-intv 10 --root "./datasets"

python train.py --dataset cifar100 --train-device cuda:0 --epochs 100 --chkpt-intv 10 --image-intv 10 --root "./datasets"



## Generate settings:
python generate.py --dataset cifar10 --chkpt-path ./chkpts/cifar10/cifar10_100.pt --save-dir ./images --device cuda:0 --total-size 50000

python generate.py --dataset cifar100 --chkpt-path ./chkpts/cifar100/cifar100_100.pt --save-dir ./images --device cuda:0 --total-size 50000


## Eval settings:
python eval.py --dataset cifar10 --root ./datasets --sample-folder ./images/eval/cifar10/cifar10_100 --device cuda:0

python eval.py --dataset cifar100 --root ./datasets --sample-folder ./images/eval/cifar10/cifar100_100 --device cuda:0




## Related repositories
- Original Repo: https://github.com/tqch/ddpm-torch
- Simple Web App empowered by Streamlit: [[tqch/diffusion-webapp]](https://github.com/tqch/diffusion-webapp)
- Classifier-Free Guidance: [[tqch/v-diffusion-torch]](https://github.com/tqch/v-diffusion-torch)




