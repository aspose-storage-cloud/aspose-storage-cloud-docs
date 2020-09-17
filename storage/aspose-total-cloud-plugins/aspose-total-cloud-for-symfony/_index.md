---
title: "Aspose.Total Cloud for Symfony"
type: docs
url: /aspose-total-cloud-for-symfony/
weight: 10
---

## **Introduction**
### **Symfony PHP Framework**
Symfony is a PHP web application framework for MVC applications. Symfony aims to speed up the creation and maintenance of web applications and to replace repetitive coding tasks. Symfony has a low performance overhead used with a bytecode cache.

Symfony is aimed at building robust applications in an enterprise context, and aims to give developers full control over the configuration: from the directory structure to the foreign libraries, almost everything can be customized. To match enterprise development guidelines, Symfony is bundled with additional tools to help developers test, debug and document projects.
### **Aspose.Total for Cloud**
Aspose for Cloud is a cloud-based document generation, conversion and automation platform for developers. Before Aspose for Cloud APIs document processing and manipulation tasks were not so easy. Aspose for Cloud APIs give developers full control over documents and file formats.

Each API has been developed to offer you a wide range of features for file processing in cloud. Aspose for Cloud REST APIs are platform independent and can be utilized across any platform such as Node.js, Amazon, Salesforce etc. without any installation. Being language independent makes it a suitable choice for developers with expertise in any programming language. We also provide SDKs in different programming languages such as .NET, Java, PHP, Ruby, Node.js, ZF 2.0, Symfony2 and Laravel.
### **Aspose.Total Cloud for Symfony**
This is a symfony2 bundle to use Aspose cloud service in symfony2 applications quickly and easily. Aspose for Cloud is a REST API to work with a number of file formats including word processing documents, spreadsheets, presentations, PDFs and images.
## **System Requirements and Supported Platforms**
### **System Requirements**
In order to install and use Aspose for Symfony bundle you need to have one of the following Symfony Framework version installed

- Symfony Framework >= 2.0

Please feel free to contact us if you find any issues in installing or using this bundle.
### **Supported Platforms**
The following Symfony Framework versions are currently supported

- Symfony Framework >= 2.0
## **Support, Extend and Contribute**
### **Support**
From the very first days of Aspose, we knew that just giving our customers good products would not be enough. We also needed to deliver good service. We are developers ourselves and understand how frustrating it is when a technical issue or a quirk in the software stops you from doing what you need to do. We're here to solve problems, not create them.

This is why we offer free support. Anyone who uses our product, whether they have bought them or are using an evaluation, deserves our full attention and respect.

You can log any issues or suggestions related to Aspose for Symfony using any of the following platforms

- [GitHub](https://github.com/asposeforcloud/asposesymfony/issues)
### **Extend and Contribute**
Aspose for Symfony is open source and its source code is available on the major social coding websites listed below. Developers are encouraged to download the source code and contribute by suggesting or adding new feature or improving the existing ones, so that others could also benefit from it.
### **Source Code**
You can get the latest source code from one of the following locations

- [GitHub](https://github.com/asposeforcloud/asposesymfony)
## **Installing**
It is very simple and easy to install Aspose for Symfony Bundle, please follow these simple steps

1. Add the following lines to your composer.json file.

```java

// composer.json

{

    require: {

        "aspose/cloud-bundle": "~0.3"

    },

    "prefer-stable": true,

}

```

1. Install the new dependencies by running "composer update" from the directory where your composer.json file is located.
1. Update your AppKernel.php by registering the new bundle.

```java

// app/AppKernel.php

public function registerBundles()

{

    // ...

     new Aspose\Bundle\CloudBundle\AsposeCloudBundle(),

    // ...

);

}

```

1. Add you Aspose API key to your config

```java

// app/config/config.yml

aspose_cloud:

    url: http://api.aspose.com/v1.1

    app:

        sid: yoursidhere

        key: yourkeyhere

        outputLocation: "%kernel.cache_dir%/aspose_cloud/" # let the API save files in the cache directory by default

```
## **Using**
To configure the initial credentials in the static fields of the AsposeApp, first get it from the container.

```java

// Bundle/Controller/DemoController.php

$app = $this->get('aspose.app');

$wordConverter = $this->get('aspose.wordsconverter');

$wordConverter->setFilename($absolutePath)

              ->convert();

```
