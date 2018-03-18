# ga-for-python

[Google Analytics API Client Library for Python](https://developers.google.com/api-client-library/python/apis/analytics/v3)  
[Hello Analytics API: Python quickstart for service accounts](https://developers.google.com/analytics/devguides/reporting/core/v3/quickstart/service-py)  

# Installing

`pip install --upgrade google-api-python-client`  

1 [Google Cloud Platform](https://console.developers.google.com/apis/)  

如何用Python連接Google anlaytics API去獲取數據，
Python是引入json的密鑰文件，而不是直接用服務端id和密鑰。

> 憑證 / 建立服務帳戶金鑰 / JSON 下載

key_file.json
```
{ 
	"project_id": "xx-xx-xxx",
	"client_email": "xx-xx@xx-xx-xxx.iam.gserviceaccount.com",
}
```

HelloAnalytics.py
```
def main():
	key_file_location = 'key_file.json' #'<REPLACE_WITH_JSON_FILE>'
```

2 [Google Analytics](https://www.google.com.tw/intl/zh-TW/analytics/)   

在使用者管理的給這個服務器ID授權，權限級別是分析的即可

> 管理者 / 使用者管理 /   
電子郵件 `xx-xx@xx-xx-xxx.iam.gserviceaccount.com`  
權限 `檢視及分析`  

查看視圖ID
> Google Analytics (分析) 套件 / 資源和應用程式 / 資料檢視 / 所有網站資料 (view_id 視圖ID)

# Run the sample

`python HelloAnalytics.py`  

> View (Profile): 所有網站資料  
Total Sessions: 2



