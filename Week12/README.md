# 🎨 圖像生成應用設計：旅遊規劃教學四步驟插畫

本設計案例以「旅遊規劃教學」為主題，利用 Fooocus 產生四張具代表性的插畫圖像，模擬應用於旅遊文章、社群貼文與簡報封面等情境。

使用「anima_pencil-XL」模型，每一張圖像修改 **Prompt**，以呈現相同風格下的多樣表現 ，圖像皆屬於日系插畫風格

## 創作動機與轉向說明

原先規劃以 **Stable Diffusion** 生成旅遊部落格網站中所需的視覺素材，目標是為不同國家的城市設計專屬的網頁元素，例如城市導覽頁的橫幅（banner）、地標標誌（icon）、文化主題插圖等。初期實驗以「東京」為例，模型能夠穩定生成具備日系視覺語彙的畫面，如：晴空塔、鳥居、霓虹招牌與街景氛圍皆準確呈現。

然而，在嘗試輸入「首爾」或「釜山」等韓國城市時，發現模型生成結果不如預期，出現以下問題：

- 地標混亂或模糊（無法呈現南山塔、甘川洞等具象特徵）
- 風格錯亂，無法辨識為韓系設計語彙
- 無法生成穩定可重複的插畫素材（即便調整 prompt 結構亦然）

經分析推測，這可能與預訓練資料集中韓國城市相關視覺資源較少有關，也與模型對非主流地標的辨識能力有限有關。因此，我調整策略，轉向**設計較為通用、跨文化適用的網頁視覺素材**，不再強調「具體地點」，而是聚焦於：

- 旅遊流程（如：規劃、打包、出發、探索）
- 日系插畫風格的氛圍與風格控制
- 可重用於多個城市／主題的 UI 組件

這些內容後續透過編輯或是加入文字，可以成為實際發布的素材！


## 生成結果

| 圖片主題 | 圖像預覽 |
|----------|----------|
| **規劃行程**<br>_Planning the Trip_<br>Prompt: Japanese soft illustration of travel planning scene, map on table, open laptop showing destinations, sticky notes and notebook, pastel watercolor style, gentle shadows, cozy desk environment |  ![](https://raw.githubusercontent.com/hahaamg/Generative_AI/main/Week12/img/fooocus%20(3).png)|
| **打包行李**<br>_Packing for the Journey_<br>Prompt: Japanese style illustration of packing for a trip, suitcase on bed, clothes folded, camera, passport, travel list, warm pastel tones, watercolor hand-drawn style| ![](https://raw.githubusercontent.com/hahaamg/Generative_AI/main/Week12/img/fooocus%20(2).png) |
| **出發與移動**<br>_Travel in Progress_<br>Prompt: Japanese illustration of traveling in progress, airport or train station, traveler with suitcase, schedule board, looking out window, soft pastel watercolor texture, clean composition | ![](https://raw.githubusercontent.com/hahaamg/Generative_AI/main/Week12/img/fooocus%20(4).png)|
| **抵達探索**<br>_Arrive and Explore_<br>Prompt: Japanese illustration of exploring a new city, traveler walking through illustrated street, camera in hand, map, discovering cute shops and sights, soft warm colors, watercolor style | ![](https://raw.githubusercontent.com/hahaamg/Generative_AI/main/Week12/img/fooocus%20(1).png) |

