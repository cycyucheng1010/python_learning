# Deep Residual Learning for Image Recognition
## Abstrct 
* 當深度逐漸增加，神經網路的訓練就會越來越困難。在這篇論文中，作者們提出了一個殘差學習 (residual Learning) 框架來使極深層的網路結構訓練變得更簡單。
## Introduction
* 當深度逐漸增加，準確度卻開始出現飽和，而且退化迅速。這樣的退化問題並非來自於 overfitting，而是因為深度增加連帶著使得 training error 增加所致。

![image](https://user-images.githubusercontent.com/62127656/133976001-1a5eb6e8-a71d-419d-be82-9bd358cfbaa8.png)

## 數學原理
* Residual: F(x) = H(x) - x
* 原本學習是這樣的。 x → H(x)
* 已經知道 F(x) = H(x) - x
* 所以學習也可以這樣寫：x → F(x) + x
* 因為H(x) = F(x) + x
* 白話文: 輸入→特徵 ，變成：輸入→ 輸入 + 殘差，若沒學到則殘差為0
![image](https://user-images.githubusercontent.com/62127656/135018371-50925c3a-8ebf-4fd6-9ba1-a1c9a5a4885d.png)

* 又因relu有負數則為0的特性，可配合殘差

![image](https://user-images.githubusercontent.com/62127656/134123823-05ae73d9-b15f-4318-ac40-0459729f0e8a.png)
![image](https://user-images.githubusercontent.com/62127656/134124009-54367385-1d5c-4880-9e9d-c9dd91f9dc45.png)
![image](https://user-images.githubusercontent.com/62127656/135017170-0c235b80-7a27-4625-b9bf-2f51a2c334a3.png)
![image](https://user-images.githubusercontent.com/62127656/135017303-4ffde896-727d-421d-a659-d1871e8fd87d.png)
![image](https://user-images.githubusercontent.com/62127656/135017641-baa5fb90-af60-44de-855f-c20bb0271320.png)
![image](https://user-images.githubusercontent.com/62127656/135018007-c2ac47b5-6e09-46c9-8639-a465624ce1e1.png)

## 參考資料
* [[文章]Deep Residual Learning for Image Recognition](https://allen108108.github.io/blog/2019/10/29/[%E8%AB%96%E6%96%87]%20Deep%20Residual%20Learning%20for%20Image%20Recognition/)
* [深度学习入门教学--Resnet残差网络介绍](https://www.youtube.com/watch?v=Bu9A_-M5OZk&t=421s)
* [Residual Leaning: 認識ResNet與他的冠名後繼者ResNeXt、ResNeSt](https://medium.com/%E8%BB%9F%E9%AB%94%E4%B9%8B%E5%BF%83/deep-learning-residual-leaning-%E8%AA%8D%E8%AD%98resnet%E8%88%87%E4%BB%96%E7%9A%84%E5%86%A0%E5%90%8D%E5%BE%8C%E7%B9%BC%E8%80%85resnext-resnest-6bedf9389ce)
* [ResNet学习笔记](https://zhuanlan.zhihu.com/p/27082562)
* [[論文]Deep Residual Learning for Image Recognition](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)
* [恆等函數](https://zh.wikipedia.org/zh-tw/%E6%81%86%E7%AD%89%E5%87%BD%E6%95%B8)
* 
