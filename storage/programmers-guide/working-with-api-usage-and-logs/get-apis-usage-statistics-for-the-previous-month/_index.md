---
title: "Get APIs Usage Statistics for the Previous Month"
type: docs
url: storage/get-apis-usage-statistics-for-the-previous-month/
weight: 30
---

## **Introduction**
This API allows you to get your usage statistics and server logs for the pervious month. The information returned is in XLSX format so you can save response to XLSX format.
## **API Explorer**
[Aspose.Platform Cloud API Reference](https://apireference.aspose.cloud/platform/) lets you try out [Get Pervious Month Usage API](https://apireference.aspose.cloud/platform/#!/Usage/Usage_GetUserUsagePreviousMonth) right away in your browser! It allows you to effortlessly interact and try out every single operation our APIs exposes. Please check [this article](/create-new-app-and-get-app-key-and-sid/) to learn how to get your App Key and SID. 
## **cURL Example**
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get Access Token
// Get App Key and App SID from https://dashboard.aspose.cloud/

curl -v "https://api.aspose.cloud/oauth2/token" \
-X POST \
-d 'grant_type=client_credentials&client_id=0B17F60A-6D69-426B-9ABD-79F35A6E9F7B&client_secret=53b8b19adffa41a3e87dbbd8858977ae' \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get APIs Usage Statistics for the current Month

curl -v "https://api.aspose.cloud/v1.1/usage/previousPeriod" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer qyc9asneEZsTZtRro3Qd2ZH38jQdBLabtIi5nE3DPgdbGolk0K8RQwB1kC1umqfp4rAKeP8gFTIRSRhl6uShnbX70X-_ieDHPAK1cCAH1Kiq6fz8lnHZc-zXmHir_TxsXrjvsjMGDwRmhjncUDMPhEU4Ah8rq0XT-8Q_dz2lWCnJsrYMXp8S2jf0QRb3xmIT5Bw1lRxsDa9PeBQ9BxDPBNYBepAUKkjNCSywA4nnoAIBeKc6mt7cmIO3J3Kv4mYk_r2z1Mog_lgmFmzYrLLPTcKNUzFHOtSAjMlz8Tn2uyihbfXJVqu7pCDd6I1yIxvcHbNIgBd01tFTjQpHUh_Pr5sKyhXg0RYLZNOSrREuRqcR04mSfR_E9RsN5k1TReZxhfUY8oacfCeUIMysGOvGB-F9J5DR41DwkxrezAeYUPE8hGBm" \
-o statistics.xlsx    

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

An .xlsx file

```

{{< /tab >}}

{{< /tabs >}}
## **SDKs**
Our API is completely independent of your operating system, database system or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone and time-consuming. Therefore, we have provided and support API [SDKs](https://github.com/aspose-storage-cloud) in many development languages in order to make it easier to integrate with us. If you use [SDK](https://github.com/aspose-storage-cloud), it hides the [REST API](https://apireference.aspose.cloud/storage/) calls and lets you use Aspose.Platform features in a native way for your preferred language.
