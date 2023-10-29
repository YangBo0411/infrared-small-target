# EFLNet: Enhancing Feature Learning for Infrared Small Target Detection
## Prerequisite

Tested on Windows 10 , with Python 3.7, PyTorch 1.13, NVIDIA 3080.

The NUAA-SIRST dataset (https://github.com/YimianDai/sirst)

The NUDT-SIRST dataset (https://github.com/YeRen123455/Infrared-Small-Target-Detection)

The IRSTD-1k dataset (https://github.com/RuiZhang97/ISNet/tree/master)

The MDvsFA dataset (https://github.com/wanghuanphd/MDvsFA_cGAN)

The IRST640 dataset (https://github.com/jzchenriver/IRST640)

The bounding box annotation version of the current infrared small target public dataset: download from  BaiduYun Drive [https://pan.baidu.com/s/1kDQIg45_9wel6GVDBTkbdg](https://pan.baidu.com/s/1Gv1gMCdajtR8pR76Y4iQhg) with code IRST.

## Requirements
  pip install -r requirements.txt
 
  pip install -U openmim
  
  mim install mmengine
  
  mim install "mmcv>=2.0.0"

## Results 
### Quantitative Results
\begin{table*}[]
\caption{Comparisons with SOTA methods on NUAA-SIRST, NUDT-SIRST and IRSTD-1k in precision, recall and F1.\label{tab:table1}}
\centering
\renewcommand\arraystretch{1.5}
\begin{tabular}{|c|ccc|ccc|ccc|}
\hline
\multirow{2}{*}{Method} & \multicolumn{3}{c|}{NUAA-SIRST}                                 & \multicolumn{3}{c|}{NUDT-SIRST}                                 & \multicolumn{3}{c|}{IRSTD-1k}                                   \\ \cline{2-10} 
                        & \multicolumn{1}{c|}{$Precision$}   & \multicolumn{1}{c|}{$Recall$}   & $F1$    & \multicolumn{1}{c|}{$Precision$}   & \multicolumn{1}{c|}{$Recall$}   & $F1$    & \multicolumn{1}{c|}{$Precision$}   & \multicolumn{1}{c|}{$Recall$}   & $F1$    \\ \hline
MDvsFA[\textcolor{green}{9}]                  & \multicolumn{1}{c|}{0.845} & \multicolumn{1}{c|}{0.507} & 0.597 & \multicolumn{1}{c|}{0.608} & \multicolumn{1}{c|}{0.192} & 0.262 & \multicolumn{1}{c|}{0.55}  & \multicolumn{1}{c|}{0.483} & 0.475 \\ \hline
AGPCNet[\textcolor{green}{31}]                & \multicolumn{1}{c|}{0.39}  & \multicolumn{1}{c|}{0.81}  & 0.527 & \multicolumn{1}{c|}{0.368} & \multicolumn{1}{c|}{0.684} & 0.479 & \multicolumn{1}{c|}{0.415} & \multicolumn{1}{c|}{0.47}  & 0.441 \\ \hline
ACM[\textcolor{green}{10}]                     & \multicolumn{1}{c|}{0.765} & \multicolumn{1}{c|}{0.762} & 0.763 & \multicolumn{1}{c|}{0.732} & \multicolumn{1}{c|}{0.745} & 0.738 & \multicolumn{1}{c|}{0.679} & \multicolumn{1}{c|}{0.605} & 0.64  \\ \hline
ISNet[\textcolor{green}{18}]                  & \multicolumn{1}{c|}{0.82}  & \multicolumn{1}{c|}{0.847} & 0.834 & \multicolumn{1}{c|}{0.742} & \multicolumn{1}{c|}{0.834} & 0.785 & \multicolumn{1}{c|}{0.718} & \multicolumn{1}{c|}{0.741} & 0.729 \\ \hline
ACLNet[\textcolor{green}{17}]                  & \multicolumn{1}{c|}{0.848} & \multicolumn{1}{c|}{0.78}  & 0.813 & \multicolumn{1}{c|}{0.868} & \multicolumn{1}{c|}{0.772} & 0.817 & \multicolumn{1}{c|}{0.843} & \multicolumn{1}{c|}{0.656} & 0.738 \\ \hline
DNANet[\textcolor{green}{19}]               & \multicolumn{1}{c|}{0.847} & \multicolumn{1}{c|}{0.836} & 0.841 & \multicolumn{1}{c|}{0.914} & \multicolumn{1}{c|}{0.889} & 0.901 & \multicolumn{1}{c|}{0.768} & \multicolumn{1}{c|}{0.721} & 0.744 \\ \hline
Ours                    & \multicolumn{1}{c|}{\textbf{0.907}} & \multicolumn{1}{c|}{\textbf{0.867}} & \textbf{0.887} & \multicolumn{1}{c|}{\textbf{0.965}} & \multicolumn{1}{c|}{\textbf{0.924}} & \textbf{0.944} & \multicolumn{1}{c|}{\textbf{0.882}} & \multicolumn{1}{c|}{\textbf{0.807}} & \textbf{0.842} \\ \hline
\end{tabular}
\label{table1}
\end{table*}
![image](https://github.com/yang19950411/infrared-small-target/blob/main/Quantitative%20Results.png)

### Visual Results
![image](https://github.com/yang19950411/infrared-small-target/blob/main/Visual%20Results.png)

## Citation

