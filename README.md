# geteduroam_tw
因為臺灣沒有官方的 geteduroam 能用，所以我手搓了一些大學的設定檔[1]。<br>
製作這些設定檔時，參考了 `Srednja šola Jesenice` 以及 `eVA(UK) - eduroam Visitor Access UK` 的設定檔格式，在此註明。<br>
目前僅支援認證方式為 PEAP-MSCHAPv2 / TTLS-PAP 的學校，不支援 PEAP-GTC。<br>
設定應用程式請至 https://www.geteduroam.app/ 下載。<br>
近期會更新更多學校的設定檔，如果有立即性需求，請參考我們的自動化生成工具 [GitHub](https://github.com/eduroamtw/eduroam_profile_generater_colab) [Colab](https://colab.research.google.com/github/eduroamtw/eduroam_profile_generater_colab/blob/main/eduroam_profile_generater_colab.ipynb)
<!--嚴格來說不只這幾個，但有 GTC 的基本上不支援-->

# 免責聲明
以下設定檔皆為第三方製作，與各校方管理單位無關，且本方不對設定檔有效性做任何擔保。<br>
其次，由於我無法取得各校的測試帳號，以下設定檔資訊大多以實際測試、認證過程 log、學校官方文件推敲組合，可能與實際情況有出入。<br>
如果內容有誤 (如認證方式、根憑證資訊、Domain、Realm 等)，歡迎直接開 Issue 或 Pull requests 修正，畢竟我不可能整天監測學校根憑證有沒有換。<br>
如果有需要不在名單上的學校，也歡迎開 Issue 或 Pull requests。<br>
設定檔內已包含：<br>
- Server CA 根憑證[2]
- 啟用匿名身分
- EAP 方式
- 二階段認證方式

註[1]：此設定檔為第三方提供，與校方管理單位無關，且本方不對設定檔有效性做任何擔保。<br>
註[2]：根憑證 (CA Certificate) 已包含在設定檔內部，如有資安疑慮可參見 [自行建立設定檔](Template/README.md) 自行設定。<br>
