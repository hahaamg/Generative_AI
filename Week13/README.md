## 期末項目概述
期末預計建立一個現代化的 AI 驅動日記網站「MyMood Pic Diary」，使用者可以通過簡單的文字輸入和情緒選擇，自動生成相應的情緒場景圖。

### 核心功能

#### 主要特性
- **情緒記錄**: 直觀的天氣和心情選擇界面
- **智能日記**: 支持文字輸入和智能建議
- **AI生成**: 模擬 AI 圖片生成流程
- **響應式設計**: 完美適配電腦和移動設備

### 用戶流程
1. 選擇今日天氣（晴天/多雲/雨天/雪天）
2. 選擇今日心情（開心/難過/生氣/平靜/興奮/疲憊）
3. 輸入今日感恩
4. 輸入今日日記內容
5. 點擊生成按鈕，AI 創建專屬圖片
6. 下載或分享生成的圖片

### 前端與模型
- 前端預計利用 JS 開發
- 文字生成與圖片生成使用 Python 串 Groq（文字）API 及 Gemini（圖片）API

---
可能介面會改為 Gradio 設計
| 說明 | 預計呈現畫面 |
|----------|------|
| 網站整體介面，可以選取一些固定的選項，如：天氣、心情，下方可以輸入完整的日記內容 |![](https://github.com/hahaamg/Generative_AI/blob/main/Week13/img/MyMood%20Pic%20DiaryDemo%20(1).png?raw=true) 
|  選擇生成後的 Pop-up 畫面 |![](https://github.com/hahaamg/Generative_AI/blob/main/Week13/img/MyMood%20Pic%20DiaryDemo%20(2).png?raw=true) 
| 最終生成結果 | ![](https://github.com/hahaamg/Generative_AI/blob/main/Week13/img/MyMood%20Pic%20DiaryDemo%20(3).png?raw=true) | 
