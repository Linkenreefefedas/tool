# Notebook Utilities

此專案包含兩個獨立的 Python Notebook，分別提供數字序列生成與自動電子郵件發送功能。

## 目錄
1. [檔案介紹](#檔案介紹)
2. [環境需求](#環境需求)
3. [使用說明](#使用說明)
   - [Running Number Generator](#running-number-generator)
   - [Auto Email Sender](#auto-email-sender)
4. [範例結果](#範例結果)

---

## 檔案介紹
### 1. `running_number.ipynb`
**功能：**
- 生成一系列連續的數字，並根據指定格式進行處理與輸出。
- 適合用於標籤生成、序列號管理等情境。

**主要功能特性：**
- 設定起始與結束數字範圍。
- 支援自定義格式（例如，數字補零）。
- 可將輸出數據存成檔案。

---

### 2. `auto_email.ipynb`
**功能：**
- 自動發送電子郵件，支援批量處理。
- 適合行銷郵件、自動化通知等情境。

**主要功能特性：**
- 支援讀取外部檔案作為收件人清單。
- 可自定義郵件主旨、內文與附件。
- 使用 `smtplib` 實現與 SMTP 伺服器的連接。

---

## 環境需求
- Python 版本：3.8+
- 必要套件：
  - `smtplib`
  - `email`
  - 其他詳見 Notebook 中的 `requirements.txt` 或註解部分。

---

## 使用說明

### 1. **Running Number Generator**
1. 開啟 `running_number.ipynb`。
2. 在 Notebook 中找到配置部分，設定以下參數：
   - `start_number`: 起始數字。
   - `end_number`: 結束數字。
   - `format`: （選擇性）數字格式，例如前置零。
3. 執行所有代碼區塊。
4. 生成的序列將顯示在輸出區域，並可選擇存檔。

---

### 2. **Auto Email Sender**
1. 開啟 `auto_email.ipynb`。
2. 在 Notebook 中找到配置部分，設定以下參數：
   - `smtp_server`: SMTP 伺服器地址（例如，`smtp.gmail.com`）。
   - `email_address`: 發送者的電子郵件地址。
   - `password`: 發送者的郵件密碼或應用程式密鑰。
   - `recipients_file`: 收件人清單檔案的路徑。
   - `subject`: 郵件主旨。
   - `content`: 郵件內文。
   - （選擇性）附件檔案路徑。
3. 執行所有代碼區塊。
4. 程式將自動向所有收件人發送郵件。

---

## 範例結果
### Running Number Generator
**輸入：**
- 起始數字：1
- 結束數字：5
- 格式：`000`

**輸出：**
