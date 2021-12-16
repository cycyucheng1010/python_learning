# 計算深度學習評價指標Precision、Recall、F1
* 對深度學習的結果進行評價是深度學習的重要一環，一般常用的評價方法有：準確率（Accuracy），精確率（Precision），召回率（Recall），畫素精度（PA），平均精度（AP），交併比（IoU）等方法。
## 什麼是TP、TN、FP、FN
1. TP（True positives）:正樣本被正確識別為正樣本。
2. TN（True negatives）:負樣本被正確識別為負樣本。
3. FP（False positives）:假的正樣本，即負樣本被錯誤識別為正樣本。
4. FN（False negatives）:假的負樣本，即正樣本被錯誤識別為負樣本。
## Recall
* Recall是測試集中所有正樣本樣例中，被正確識別為正樣本的比例。
* Recall=TP/(TP+FN)
## Precision
* Precision就是在識別出來的正樣本中，True positives所佔的比率。
* Precision=TP/(TP+FP)
## F1
* F1 score為精確率與召回率的調和均值，是用來衡量二分類模型精確度的一種指標。
* F1=2*(Precision*Recall)/(Precision+Recall)
