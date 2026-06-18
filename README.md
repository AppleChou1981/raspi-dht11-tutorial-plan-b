【中文詳細說明】

本專案為物聯網進階實作之「方案 B（本地中繼發送方案）」。系統以樹莓派 3 為核心，透過 Python 定時讀取 DHT11 溫溼度感測器數據。為了確保高隱私度與企業級安全驗證，本方案放棄使用 GAS 網頁部署，改採 Google Cloud Platform (GCP) 的服務帳戶（Service Account）下載 JSON 金鑰憑證，直接呼叫 Google Sheets API V4 將數據精準寫入雲端試算表；同時直接調用 LINE Messaging API 執行 Push Message，將即時環境狀態推播至使用者手機。

【English Detailed Description】

This project demonstrates "Plan B (Local Relay Solution)" for an advanced IoT implementation. Powered by Raspberry Pi 3, the system uses Python to periodically read temperature and humidity data from a DHT11 sensor. To ensure high privacy and enterprise-grade security authentication, this approach bypasses GAS web apps. Instead, it utilizes a Google Cloud Platform (GCP) Service Account with a downloaded JSON credential key to directly write data into Google Sheets via the API V4, while simultaneously calling the LINE Messaging API to push real-time environmental alerts to the user's mobile device.
