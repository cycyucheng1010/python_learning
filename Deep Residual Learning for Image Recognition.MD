# 論文 Deep Residual Learning for Image Recognition
## Abstrct 
* 當深度逐漸增加，神經網路的訓練就會越來越困難。在這篇論文中，作者們提出了一個殘差學習 (residual Learning) 框架來使極深層的網路結構訓練變得更簡單。
* ResNet在2015年被提出，在ImageNet比賽classification任務上獲得第一名，因為它「簡單與實用」。
## Introduction
* 當深度逐漸增加，準確度卻開始出現飽和，而且退化迅速。這樣的退化問題並非來自於 overfitting，而是因為深度增加連帶著使得 training error 增加所致。
<br>
![image](https://user-images.githubusercontent.com/62127656/133976001-1a5eb6e8-a71d-419d-be82-9bd358cfbaa8.png)
<br>
* 期望F(x)→x，既然無法則讓F(x)-x趨近於0，F(x)=x
<br>
![image](https://user-images.githubusercontent.com/62127656/134841180-848ac7bf-e5f7-42ac-a2d2-f44fbb93fe2a.png)
![image](https://user-images.githubusercontent.com/62127656/134841151-c1ef2ec0-42e1-46fe-99d9-d81cdda1309c.png)
![image](https://user-images.githubusercontent.com/62127656/134841145-0e381bb6-545e-4d5b-9a4b-814b424d8576.png)
<br>
* 目前ResNet 的 層數以及捲積
<br>
![image](https://user-images.githubusercontent.com/62127656/134841002-85367e1f-4ac5-4edd-a4a5-fe58a1dc7f9e.png)
![image](https://user-images.githubusercontent.com/62127656/134841467-6c1a3bbc-d376-496c-849c-0b30af5b73ca.png)
<br>
* 深度残差網路可以很容易的從急劇增加的深度中获得精準度
<br>
![image](https://user-images.githubusercontent.com/62127656/134842430-7b38fb6b-5ccd-4ec2-9578-cccfe5ddfb4f.png)





## 參考資料
* [Deep Residual Learning for Image Recognition (allen108108筆記)](https://allen108108.github.io/blog/2019/10/29/[%E8%AB%96%E6%96%87]%20Deep%20Residual%20Learning%20for%20Image%20Recognition/)
* [經典神經網路學習（四）——ResNet](https://www.itread01.com/content/1545500646.html)
* [Deep Residual Learning for Image Recognition (論文)](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)
* [恆等函數](https://zh.wikipedia.org/wiki/%E6%81%86%E7%AD%89%E5%87%BD%E6%95%B8)
* [ResNet学习笔记](https://zhuanlan.zhihu.com/p/27082562)
