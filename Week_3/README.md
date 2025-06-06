## 主題一：GAN模型實際操作生成圖片
### 模型介紹：
* 網站名稱：This XXX Does Not Exist
* 網站連結：https://www.thisautomobiledoesnotexist.com/
* 網站描述：​利用生成對抗網絡（GAN），自動生成不存在的汽車圖片。每次刷新頁面，都會看到一輛全新的、由 AI 創造的虛構汽車。
* 技術背景：StyleGAN2

### 生成結果
從以下上傳的樣張中可以觀察到，「This Automobile Does Not Exist」確實能夠生成虛構的汽車圖片，但整體品質仍有許多可改進之處。儘管圖片中能夠辨識出汽車的存在，但在細節方面仍存在許多不自然的現象，例如：
* 結構錯誤：車頭與車尾有時會重複出現，導致一輛車可能擁有兩個車頭或不合理的外形結構。
* 細節缺失：車輛的關鍵部件（如車門、進氣壩、車燈）有時缺失或形狀異常，使得整體車輛顯得不完整。
* 車牌問題：車牌的處理較為粗糙，號碼模糊不清，且有時出現無意義的亂碼，使其無法仿真真實車牌。
* 設計較為過時：生成的汽車多呈現較舊的設計風格，可能與訓練數據集中較多的舊款車型有關，使其難以生成較為現代化的車款。
* 背景變形與融合問題：背景經常呈現失真或模糊狀態，部分情境下甚至會與車輛融合，使得汽車與環境之間的界線不明確。

<div style="display: flex; justify-content: center;">
  <img src="img/thisautomobiledoesnotexist(1).png" alt="圖片 1" width="300" style="margin-right: 10px;">
  <img src="img/thisautomobiledoesnotexist(2).png" alt="圖片 2" width="300">
</div>

<div style="display: flex; justify-content: center;">
  <img src="img/thisautomobiledoesnotexist(3).png" alt="圖片 3" width="300" style="margin-right: 10px;">
  <img src="img/thisautomobiledoesnotexist(4).png" alt="圖片 4" width="300">
</div>

### 目前 GAN 較少人使用的原因
* 在生成圖片方面，GAN 似乎難以處理「文本到圖片」的生成，像是目前較常使用的 Diffusion 模型都可以根據文字描述來生成圖片
* 經過平常使用 Diffusion 模型與這次使用 GAN 模型，可以明顯發現 Diffusion 模型所生成的圖片品質與細節的控制較好

