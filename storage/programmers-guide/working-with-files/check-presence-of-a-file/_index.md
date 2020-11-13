---
title: "Check Presence of a File"
type: docs
url: /check-presence-of-a-file/
weight: 50
---

## **Introduction**
This API allows you to check the presence of a file or folder in the [Aspose Cloud Storage](https://dashboard.aspose.cloud/#/).
## **API Explorer**
[Aspose.Storage Cloud API Reference](https://apireference.aspose.cloud/storage/) lets you try out [Check File Presence API](https://apireference.aspose.cloud/storage/#!/Storage/GetIsExist) right away in your browser! It allows you to effortlessly interact and try out every single operation our APIs exposes. Please check [this article](/total/create-new-app-and-get-app-key-and-sid/) to learn how to get your App Key and SID.
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



// cURL example to check presence of a file

curl -v "https://api.aspose.cloud/v1.1/storage/exist?path=input.pdf" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer A03jLSHkq6zu_A8kpxU6xPKOEkBFn7fX6_hhKkAO0-2AFeI0UgB_M_D4O1cLkZSbfgGpbpA7oos3P8BhpbvDqHjcIkzTnSXBPkBJpRpWGdj2DwuQ9kd_FuBMTiU5NBZ3gUOwDGuY7bUJejPw8NzOFsk6Lt9z9CCR2lOyWUpKzlPSTl3DSaIkZRKluuccL4sT-PqeDkOHgn6mewV0P0GsrBkoQo6LDk1RozojGDYvPDAqVPFHmwc20MHnMtXlE5CA-koBJa0LmXKFBRKNqv1COa9l4qrDRRtNcx1yJWPdpvY6udg3a1oD36qlzSNiMNaAFZNWESzK3lZEgr6uAFZeG6SC4SHcws6OITJKm7P_VAjGElvAEAtnaO4qng6myB2prDUNIYHcwQkN4DaUPoQguJnPXbeB2WKV-u07p3y0fxAUZ82TOcew_LO-vCb15pBSsvpIHX3n3XE-egWrngqShI3uDNE"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "FileExist": {

    "IsExist": true,

    "IsFolder": false

  },

  "Code": 200,

  "Status": "OK"

}

```

{{< /tab >}}

{{< /tabs >}}
## **SDKs**
Our API is completely independent of your operating system, database system or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone and time-consuming. Therefore, we have provided and support API [SDKs](https://github.com/aspose-storage-cloud) in many development languages in order to make it easier to integrate with us. If you use [SDK](https://github.com/aspose-storage-cloud), it hides the [REST API](https://apireference.aspose.cloud/storage/) calls and lets you use Aspose.Platform features in a native way for your preferred language.
## **SDK Examples**
{{< tabs tabTotal="5" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Ruby" tabName5="Python" >}}

{{< tab tabNum="1" >}}

{{< gist "" "a8258d0b8fd58eb053288a3cff0d1502" "Examples-.NET-CheckPresenceOfAFile.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "" "eaf2e8de18f69f1a0697ddf4eab27810" "Examples-Java-CheckPresenceOfAFile.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "" "40ddc3d17a9e4e30dd3cf523a82bae43" "Examples-PHP-CheckFilePresence.php" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}



{{< gist "" "e4e153a2cc06bed2a33bbf9311d88af6" "Examples-Ruby-CheckFilePresence.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "" "fbcea75cc30950ed47a4259fd2467130" "Examples-Python-CheckFilePresence.py" >}}

{{< /tab >}}

{{< /tabs >}}
