# Whisper + Gemini Meeting Transcription and Summarization

此專案結合 OpenAI 的 Whisper 模型與 Google Gemini API，實現以下功能：
1. 使用 Whisper 模型進行音檔轉錄，支援繁體中文。
2. 利用 Gemini API 生成會議摘要，輸出為簡潔的重點式摘要。

## 功能概述

- **音檔轉錄**：透過 Whisper 模型處理音頻，轉換為文字。
- **摘要生成**：將轉錄內容發送至 Gemini API，生成簡潔的會議摘要。
- **輸出結果**：轉錄文字及摘要結果分別保存為 `.txt` 文件。

---

## 環境需求

1. Google Colab 環境
2. 已安裝以下 Python 套件：
   - `whisper`
   - `requests`
   - `google-colab`

---

## 使用方法

### 1. 上傳音檔

請將欲轉錄的音檔（例如：`water.m4a`）上傳至 Colab 的 `/content` 路徑。

---

### 2. 更新程式碼中的 API Key

在程式碼中找到以下部分，替換成你的 Gemini API 密鑰：
```python
api_key = "YOUR_GEMINI_API_KEY"
