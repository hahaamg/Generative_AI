## Introduction
本 RAG 資料庫內容取自於我的旅遊部落格的部分文章，將文章先匯出成 XML 檔案再轉檔至 Markdown 後再轉完 JSON，以 JSON 方式輸入再去切 Chunk。目前僅將部分文章作為資料庫內容，因此 RAG 能力有限，未來希望能夠更完善資料庫及編碼，讓其可以做延伸應用，像是對比文章資訊是否與網路資訊有誤、進行網站內容管理等等。

程式中有試圖讓模型的回應更好，嘗試包含：加大回應的 Token 數量、增加相關資料的片度數量，但效果還需優化。
## Prompt template
你是一位資深的知識專家助理，擅長用繁體中文從文件中找出重點並加以整合說明。
以下是知識庫中找到的資訊片段（可能來自不同文件）請你閱讀全部資訊後，再進行統整，不要只選擇部分資料作答：

{retrieved_chunks}

請根據上方資料，完整、有條理地回答使用者的問題。
1. 若資訊足夠，請詳細解釋並輔以舉例。
2. 若資訊不足，也請指出無法回答的原因。

使用者的提問如下：
{question}

## 實際使用
  <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week_8/img/TestCase_SreenShot1.png?raw=true" width="1000" style="margin-right: 10px;">
  <img src="https://github.com/hahaamg/Generative_AI/blob/main/Week_8/img/TestCase_SreenShot2.png?raw=true" width="1000" style="margin-right: 10px;">
