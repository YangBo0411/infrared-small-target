# EFLNet: Enhancing Feature Learning for Infrared Small Target Detection
## Prerequisite

Tested on Windows 10 , with Python 3.7, PyTorch 1.13, NVIDIA 3080.

The NUAA-SIRST dataset (https://github.com/YimianDai/sirst)

The NUDT-SIRST dataset (https://github.com/YeRen123455/Infrared-Small-Target-Detection)

The IRSTD-1k dataset (https://github.com/RuiZhang97/ISNet/tree/master)

The MDvsFA dataset (https://github.com/wanghuanphd/MDvsFA_cGAN)

The IRST640 dataset (https://github.com/jzchenriver/IRST640)

The bounding box annotation version of the current infrared small target public dataset: download from [BaiduYun Drive](https://pan.baidu.com/s/1Gv1gMCdajtR8pR76Y4iQhg) with code IRST.

## Requirements
  pip install -r requirements.txt
 
  pip install -U openmim
  
  mim install mmengine
  
  mim install "mmcv>=2.0.0"

## Results 
### Quantitative Results
|     Method     |     NUAA-SIRST    |              |              |     NUDT-SIRST    |              |              |     IRSTD-1k    |              |              |
|----------------|-------------------|--------------|--------------|-------------------|--------------|--------------|-----------------|--------------|--------------|
|                |     Pre           |     Rec      |     F1       |     Pre           |     Rec      |     F1       |     Pre         |     Rec      |     F1       |
|     MDvsFA     |     0.845         |     0.507    |     0.597    |     0.608         |     0.192    |     0.262    |     0.55        |     0.483    |     0.475    |
|     AGPCNet    |     0.39          |     0.81     |     0.527    |     0.368         |     0.684    |     0.479    |     0.415       |     0.47     |     0.441    |
|     ACM        |     0.765         |     0.762    |     0.763    |     0.732         |     0.745    |     0.738    |     0.679       |     0.605    |     0.64     |
|     ISNet      |     0.82          |     0.847    |     0.834    |     0.742         |     0.834    |     0.785    |     0.718       |     0.741    |     0.729    |
|     ACLNet     |     0.848         |     0.78     |     0.813    |     0.868         |     0.772    |     0.817    |     0.843       |     0.656    |     0.738    |
|     DNANet     |     0.847         |     0.836    |     0.841    |     0.914         |     0.889    |     0.901    |     0.768       |     0.721    |     0.744    |
|     ours       |     0.907         |     0.867    |     0.887    |     0.965         |     0.924    |     0.944    |     0.882       |     0.807    |     0.842    |
| Download       |            [weight](https://github.com/yang19950411/infrared-small-target/raw/main/runs/train/IRSTD.pt)       |              |              |                   |              |              |                 |              |              |

### Visual Results

![image](https://github.com/yang19950411/infrared-small-target/blob/main/Visual%20Results.png)

## Citation

