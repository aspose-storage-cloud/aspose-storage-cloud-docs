---
title: "Create a New Folder on Third Party Storage"
type: docs
url: /create-a-new-folder-on-third-party-storage/
weight: 20
---

## **Introduction**
This API allows you to create a new folder on third party storage.

**Note:** You need to configure Third Party Storage with Aspose for Cloud before using this example. Please follow the instructions at [this page](/total/how-to-configure-3rd-party-cloud-storages/) to configure your required storage.
## **API Explorer**
[Aspose.Storage Cloud API Reference](https://apireference.aspose.cloud/storage/) lets you try out [Create a New Folder API](https://apireference.aspose.cloud/storage/#!/Folder/PutCreateFolder) right away in your browser! It allows you to effortlessly interact and try out every single operation our APIs exposes. Please check [this article](/total/create-new-app-and-get-app-key-and-sid/) to learn how to get your App Key and SID. 
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

// cURL example to create a new folder

curl -v "https://api.aspose.cloud/v1.1/storage/folder?path=Pictures&storage=DropboxStorage" \
-X PUT \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer qyc9asneEZsTZtRro3Qd2ZH38jQdBLabtIi5nE3DPgdbGolk0K8RQwB1kC1umqfp4rAKeP8gFTIRSRhl6uShnbX70X-_ieDHPAK1cCAH1Kiq6fz8lnHZc-zXmHir_TxsXrjvsjMGDwRmhjncUDMPhEU4Ah8rq0XT-8Q_dz2lWCnJsrYMXp8S2jf0QRb3xmIT5Bw1lRxsDa9PeBQ9BxDPBNYBepAUKkjNCSywA4nnoAIBeKc6mt7cmIO3J3Kv4mYk_r2z1Mog_lgmFmzYrLLPTcKNUzFHOtSAjMlz8Tn2uyihbfXJVqu7pCDd6I1yIxvcHbNIgBd01tFTjQpHUh_Pr5sKyhXg0RYLZNOSrREuRqcR04mSfR_E9RsN5k1TReZxhfUY8oacfCeUIMysGOvGB-F9J5DR41DwkxrezAeYUPE8hGBm"    

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
Our API is completely independent of your operating system, database system or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone and time-consuming. Therefore, we have provided and support API [SDKs](https://github.com/aspose-storage-cloud) in many development languages in order to make it easier to integrate with us. If you use [SDK](https://github.com/aspose-storage-cloud), it hides the [REST API](https://apireference.aspose.cloud/storage/) calls and lets you use Aspose.Storage features in a native way for your preferred language.
## **SDK Examples**
{{< tabs tabTotal="5" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Ruby" tabName5="Python" >}}

{{< tab tabNum="1" >}}

{{< gist "" "a8258d0b8fd58eb053288a3cff0d1502" "Examples-.NET-CreateNewFolderOnThirdPartyStorage.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "" "eaf2e8de18f69f1a0697ddf4eab27810" "Examples-Java-CreateNewFolderOnThirdPartyStorage.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "" "40ddc3d17a9e4e30dd3cf523a82bae43" "Examples-PHP-CreateFolderOnThirdPartyStorage.php" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}



{{< gist "" "e4e153a2cc06bed2a33bbf9311d88af6" "Examples-Ruby-CreateFolderOnThirdPartyStorage.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "" "fbcea75cc30950ed47a4259fd2467130" "Examples-Python-CreateFolderOnThirdPartyStorage.py" >}}

{{< /tab >}}

{{< /tabs >}}
