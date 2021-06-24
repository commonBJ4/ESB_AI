# Esun Bank Chinese Handwrite AI Competition
***將主辦方提供的六萬多張中文圖片透過深度學習模型訓練以達成識別分類***
## 動機
在搜尋有關AI相關資訊時，突然看到ESB的競賽訊息，因此想透過這個中文手寫辨識的競賽機會學習如何將Deep Learning與API 技術相結合，並透過部屬至雲端創造一個整合性服務。
## 設計理念
此次競賽我們使用到的技術有：**CNN+Flask+GCP+uWSGI+Nginx**

* Model的設計：  
  將已處理過的資料圖片結果(資料清洗及資料擴增)，透過CNN準確地辨別出圖片裡的中文字，最終將訓練過後的model與webservice結合回傳至client端。

* API的設計：  
  使用主辦方提供範例程式中的Flask框架(Flask是一個較為容易及快速上手的web service的套件)製作api再加上uwsgi及nginx的技術，避免service撐不住同時處理多個requests。
  
## 簡易步驟流程
由於這次主辦方提供了資料集，我們可以省去資料收集的過程。

將這次的競賽流程分了五個大方向：

