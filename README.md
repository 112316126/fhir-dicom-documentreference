# 心臟超音波 DICOM 與 FHIR DocumentReference 整合

## 專案介紹

本專案示範如何將心臟超音波 DICOM 影像與 HL7 FHIR DocumentReference 進行整合。

系統利用 FHIR DocumentReference 建立醫療影像的 Metadata，將 DICOM 檔案與 Metadata 分離管理，使醫療影像能以標準化方式進行索引、查詢及調閱。

本專案為前端示範系統，模擬 DICOM Repository 與 FHIR Server 的整合流程。

---

## 功能特色

- 上傳 DICOM 檔案
- 自動產生 FHIR DocumentReference Metadata
- 建立符合 FHIR R4 的 JSON
- 匯出 DocumentReference JSON
- 模擬 DICOM Repository 儲存流程
- 示範醫療影像 Metadata 管理

---

## 系統架構

```
使用者
    │
    ▼
DICOM Viewer
    │
    ▼
DICOM Repository
    │
    ▼
FHIR DocumentReference
    │
    ▼
FHIR Server
```

---

## 使用技術

- HTML5
- CSS3
- JavaScript
- HL7 FHIR R4
- DICOM

---

## 專案內容

本系統可建立下列 DocumentReference Metadata：

- Patient（病人資訊）
- Document Type（文件類型）
- Category（文件分類）
- Status（文件狀態）
- Author（建立者）
- Description（文件描述）
- DICOM URL
- Attachment Metadata

系統可輸出符合 FHIR R4 規範的 DocumentReference JSON。

---

## 未來擴充

- 串接真實 FHIR Server
- 串接 PACS / DICOM Server
- OAuth2 使用者驗證
- 病人查詢功能
- DICOM Viewer 整合
- 多模態醫療資料（PDF、ECG、Video）

---

## 授權

MIT License

---
---
# FHIR DICOM DocumentReference

## Project Overview

This project demonstrates how DICOM cardiac ultrasound images can be integrated with HL7 FHIR DocumentReference.

The application allows users to:

- Upload DICOM files
- Generate FHIR DocumentReference metadata
- Export DocumentReference JSON
- Simulate DICOM repository integration
- Demonstrate standardized medical image indexing

## Technologies

- HTML
- CSS
- JavaScript
- HL7 FHIR R4
- DICOM

## Features

- Generate DocumentReference metadata
- Support DICOM file selection
- Export metadata as JSON
- Simulate medical image repository integration

## Future Improvements

- Connect to a real FHIR Server
- PACS integration
- OAuth authentication
- Patient search
- DICOM Viewer integration
