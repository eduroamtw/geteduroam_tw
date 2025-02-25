# geteduroam_tw
因為臺灣沒有官方的 geteduroam 能用，所以我手搓了一些大學的設定檔[1]。<br>
製作這些設定檔時，參考了 `Srednja šola Jesenice` 以及 `eVA(UK) - eduroam Visitor Access UK` 的設定檔格式，在此註明。<br>
目前僅支援認證方式為 PEAP-MSCHAPv2 / TTLS-PAP 的學校，不支援 PEAP-GTC<br>
設定檔內已包含：<br>
- Server CA 根憑證[2]
- 啟用匿名身分
- EAP 方式
- 二階段認證方式
註[1]：此設定檔為第三方提供，與校方管理單位無關。<br>
註[2]：根憑證已包含在設定檔內部，如有資安疑慮可參見 `自行建立設定檔(TBD)` 自行設定。<br>