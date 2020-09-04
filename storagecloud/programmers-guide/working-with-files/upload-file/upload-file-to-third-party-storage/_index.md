---
title: "Upload File to Third Party Storage"
type: docs
url: /upload-file-to-third-party-storage/
weight: 20
---

## **Introduction**
This API allows you to upload files to the third party storage.

**Note:** You need to configure Third Party Storage with Aspose for Cloud before using this example. Please follow the instructions at [this page](https://docs.aspose.cloud/display/totalcloud/How+to+Configure+3rd+Party+Cloud+Storages) to configure your required storage.
## **API Explorer**
[Aspose.Storage Cloud API Reference](https://apireference.aspose.cloud/storage/) lets you try out [Upload a File API](https://apireference.aspose.cloud/storage/#!/File/PutCreate) right away in your browser! It allows you to effortlessly interact and try out every single operation our APIs exposes. Please check [this article](https://docs.aspose.cloud/display/totalcloud/Create+New+App+and+Get+App+Key+and+SID) to learn how to get your App Key and SID.
## **cURL Example**
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get Access Token

// Get App Key and App SID from https://dashboard.aspose.cloud/

curl -v "https://api.aspose.cloud/oauth2/token" \

-X POST \

-d 'grant\_type=client\_credentials&client\_id=0B17F60A-6D69-426B-9ABD-79F35A6E9F7B&client\_secret=53b8b19adffa41a3e87dbbd8858977ae' \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

// cURL example to upload file to Third Party Storage

curl -v "https://api.aspose.cloud/v1.1/storage/file?path=testfile.txt&storage=DropboxStorage" \

-X PUT \

-T testfile.txt \

-H "Content-Type: multipart/form-data" \

-H "Accept: application/json" \

-H "Authorization: Bearer qyc9asneEZsTZtRro3Qd2ZH38jQdBLabtIi5nE3DPgdbGolk0K8RQwB1kC1umqfp4rAKeP8gFTIRSRhl6uShnbX70X-\_ieDHPAK1cCAH1Kiq6fz8lnHZc-zXmHir\_TxsXrjvsjMGDwRmhjncUDMPhEU4Ah8rq0XT-8Q\_dz2lWCnJsrYMXp8S2jf0QRb3xmIT5Bw1lRxsDa9PeBQ9BxDPBNYBepAUKkjNCSywA4nnoAIBeKc6mt7cmIO3J3Kv4mYk\_r2z1Mog\_lgmFmzYrLLPTcKNUzFHOtSAjMlz8Tn2uyihbfXJVqu7pCDd6I1yIxvcHbNIgBd01tFTjQpHUh\_Pr5sKyhXg0RYLZNOSrREuRqcR04mSfR\_E9RsN5k1TReZxhfUY8oacfCeUIMysGOvGB-F9J5DR41DwkxrezAeYUPE8hGBm"



```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Code": 200,

  "Status": "OK"

}

```

{{< /tab >}}

{{< /tabs >}}
## **SDKs**
Our API is completely independent of your operating system, database system or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone and time-consuming. Therefore, we have provided and support API [SDKs](https://github.com/aspose-storage-cloud) in many development languages in order to make it easier to integrate with us. If you use [SDK](https://github.com/aspose-storage-cloud), it hides the [REST API](https://apireference.aspose.cloud/storage/#!/File/PutCreate) calls and lets you use Aspose.Storage features in a native way for your preferred language.
## **SDK Examples**
{{< tabs tabTotal="5" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Ruby" tabName5="Python" >}}

{{< tab tabNum="1" >}}

{{< gist "" "a8258d0b8fd58eb053288a3cff0d1502" "Examples-.NET-UploadFileToThirdPartyStorage.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "" "eaf2e8de18f69f1a0697ddf4eab27810" "Examples-Java-UploadFileToThirdPartyStorage.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "" "40ddc3d17a9e4e30dd3cf523a82bae43" "Examples-PHP-UploadFileToThirdPartyStorage.php" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "" "e4e153a2cc06bed2a33bbf9311d88af6" "Examples-Ruby-UploadFileToThirdPartyStorage.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "" "fbcea75cc30950ed47a4259fd2467130" "Examples-Python-UploadFileToThirdPartyStorage.py" >}}

{{< /tab >}}

{{< /tabs >}}
