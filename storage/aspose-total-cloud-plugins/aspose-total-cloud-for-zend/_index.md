---
title: "Aspose.Total Cloud for Zend"
type: docs
url: /aspose-total-cloud-for-zend/
weight: 30
---

## **Introduction**
### **Zend PHP Framework**
Zend Framework 2 is an open source framework for developing web applications and services using PHP 5.3+. Zend Framework 2 uses 100% object-oriented code and utilises most of the new features of PHP 5.3, namely namespaces, late static binding, lambda functions and closures.

Zend Framework 2 evolved from Zend Framework 1, a successful PHP framework with over 15 million downloads.

The component structure of Zend Framework 2 is unique; each component is designed with few dependencies on other components. ZF2 follows the SOLID object oriented design principle. This loosely coupled architecture allows developers to use whichever components they want. We call this a “use-at-will” design.
### **Aspose.Total for Cloud**
Aspose for Cloud is a cloud-based document generation, conversion and automation platform for developers. Before Aspose for Cloud APIs document processing and manipulation tasks were not so easy. Aspose for Cloud APIs give developers full control over documents and file formats.

Each API has been developed to offer you a wide range of features for file processing in cloud. Aspose for Cloud REST APIs are platform independent and can be utilized across any platform such as Node.js, Amazon, Salesforce etc. without any installation. Being language independent makes it a suitable choice for developers with expertise in any programming language. We also provide SDKs in different programming languages such as .NET, Java, PHP, Ruby, Node.js, ZF 2.0, Symfony2 and Laravel.
### **Aspose.Total Cloud for Zend**
Aspose.Total Cloud for Zend module provides a simple wrapper for the Aspose for Cloud PHP SDK, making it easily accessible anywhere in your application.
## **System Requirements and Supported Platforms**
### **System Requirements**
In order to install and use Aspose for Zend module you need to have one of the following Zend Framework version installed

- Zend Framework >= 2.0

Please feel free to contact us if you find any issues in installing or using this module.
### **Supported Platforms**
The following Zend Framework versions are currently supported

- Zend Framework >= 2.0
## **Support, Extend and Contribute**
### **Support**
From the very first days of Aspose, we knew that just giving our customers good products would not be enough. We also needed to deliver good service. We are developers ourselves and understand how frustrating it is when a technical issue or a quirk in the software stops you from doing what you need to do. We're here to solve problems, not create them.

This is why we offer free support. Anyone who uses our product, whether they have bought them or are using an evaluation, deserves our full attention and respect.

You can log any issues or suggestions related to Aspose for Zend using any of the following platforms

- [GitHub](https://github.com/asposeforcloud/Aspose_Cloud_SDK_For_PHP/issues)
### **Extend and Contribute**
Aspose for Zend is open source and its source code is available on the major social coding websites listed below. Developers are encouraged to download the source code and contribute by suggesting or adding new feature or improving the existing ones, so that others could also benefit from it.
### **Source Code**
You can get the latest source code from one of the following locations

- [GitHub](https://github.com/asposeforcloud/Aspose_Cloud_SDK_For_PHP)
## **Installing**
It is very simple and easy to install Aspose for Zend Module, please follow these simple steps

1. Add the following line to your composer.json file.

```java

"require": { "aspose/cloud-sdk-php": "dev-master" }

```

1. Execute command on shell.

```java

composer update

```
## **Using**
This example show you how to convert word documents to other formats.

```java

//Add following namespaces

use Aspose\Cloud\Common\AsposeApp;

use Aspose\Cloud\Common\Product;

use Aspose\Cloud\Common\Utils;

use Aspose\Cloud\Words\Converter;

//Use the following code in your controller or model

Product::$baseProductUri = 'http://api.aspose.com/v1.1';

AsposeApp::$appSID = "XXXXXXXXXX";

AsposeApp::$appKey = "XXXXXXXXXX";

//Set output path

AsposeApp::$outPutLocation = getcwd() . "/output/";

//Set input path

$inputFile = getcwd() . "/input/Test.docx";

$doc = new Converter('Test.docx');

$outputFormat = "pdf";

$outputPath = '';

$result = $doc->convertLocalFile($inputFile, $outputPath, $outputFormat);

```
