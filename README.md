# JugdementPredict
AI人民法槌-妨害名譽罪量刑系統
https://sanguine-robot-377702.uc.r.appspot.com/

目的
協助被起訴妨害名譽或是誹謗罪的一般大眾可以快速理解自己可能會被判多少罰金，以避免和解過程中被要求不合理的和解金。

網站架構說明
* 資料來源：爬蟲法學資料檢索系統民國89年至110年的妨害名譽罪的判決書。
* 資料清洗：使用Jieba自然語言處理程序，對判決書進行斷詞，提取罰款金額，並根據不同的情境提取其特徵值。
* 模型訓練：採用XGboost建立機械學習模型，最終預測準確度高於60%。
* Web應用框架：以Flask為開發框架。
* 部署平台：以GCP的App engine部署此服務
