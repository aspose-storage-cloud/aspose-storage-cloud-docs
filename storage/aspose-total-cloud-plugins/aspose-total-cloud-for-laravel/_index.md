---
title: "Aspose.Total Cloud for Laravel"
type: docs
url: /aspose-total-cloud-for-laravel/
weight: 20
---

## **Introduction**
### **Laravel PHP Framework**
Laravel is a web application framework with expressive, elegant syntax. Laravel believes that development must be an enjoyable, creative experience to be truly fulfilling. Laravel attempts to take the pain out of development by easing common tasks used in the majority of web projects, such as authentication, routing, sessions, and caching.

Laravel is accessible, yet powerful, providing powerful tools needed for large, robust applications. A superb inversion of control container, expressive migration system, and tightly integrated unit testing support give you the tools you need to build any application with which you are tasked.
### **Aspose.Total for Cloud**
Aspose for Cloud is a cloud-based document generation, conversion and automation platform for developers. Before Aspose for Cloud APIs document processing and manipulation tasks were not so easy. Aspose for Cloud APIs give developers full control over documents and file formats.

Each API has been developed to offer you a wide range of features for file processing in cloud. Aspose for Cloud REST APIs are platform independent and can be utilized across any platform such as Node.js, Amazon, Salesforce etc. without any installation. Being language independent makes it a suitable choice for developers with expertise in any programming language. We also provide SDKs in different programming languages such as .NET, Java, PHP, Ruby, Node.js, ZF 2.0, Symfony2 and Laravel.
### **Aspose.Total Cloud for Laravel**
Aspose.Total Cloud for Laravel package allows developers to use Aspose for Cloud PHP SDK in Laravel 4 & 5 applications to speed up your development process. This package serves as wrapper to Aspose for Cloud PHP SDK to be used as a Laravel Package.
## **System Requirements and Supported Platforms**
### **System Requirements**
In order to install and use Aspose for Laravel package you need to have one of the following Laravel Framework version installed

- Laravel Framework = 4.\*
- Laravel Framework = 5.\*

Please feel free to contact us if you find any issues in installing or using this package.
### **Supported Platforms**
The following Laravel Framework versions are currently supported

- Laravel Framework = 4.\*
- Laravel Framework = 5.\*
## **Support, Extend and Contribute**
### **Support**
From the very first days of Aspose, we knew that just giving our customers good products would not be enough. We also needed to deliver good service. We are developers ourselves and understand how frustrating it is when a technical issue or a quirk in the software stops you from doing what you need to do. We're here to solve problems, not create them.

This is why we offer free support. Anyone who uses our product, whether they have bought them or are using an evaluation, deserves our full attention and respect.

You can log any issues or suggestions related to Aspose for Laravel using any of the following platforms

- [GitHub](https://github.com/asposeforcloud/asposelaravel/issues)
### **Extend and Contribute**
Aspose for Laravel is open source and its source code is available on the major social coding websites listed below. Developers are encouraged to download the source code and contribute by suggesting or adding new feature or improving the existing ones, so that others could also benefit from it.
### **Source Code**
You can get the latest source code from one of the following locations

- [GitHub](https://github.com/asposeforcloud/asposelaravel)
## **Installing**
### **Installation**
It is very simple and easy to install Aspose for Laravel package, please follow these simple steps

1. Add the following line to your composer.json file.

```java

require: {

        "aspose/cloud-laravel": "~1.0"

}

```

1. Run from terminal.

```java

composer update

```
### **Laravel 4 Integration**
- Add package to the list of providers. In **config/app.php**, add the following line to the providers array.

```java

'Aspose\Cloud\CloudServiceProvider',

```

- Publish config file from the terminal.

```java

php artisan config:publish aspose/cloud-laravel

```

- Edit the new config file in the **config/packages/aspose/cloud-laravel** and enter your **App Key** & **App SID**.

```java

return array(

    'baseUri' => 'http://api.aspose.com/v1.1',

    'appSID' => '',

    'appKey' => ''

);

```

- In **config/packages/aspose**, rename **cloud-laravel** to **cloud**
### **Laravel 5 Integration**
- Add package to the list of providers. In **config/app.php**, add the following line to the providers array.

```java

'Aspose\Cloud\CloudServiceProvider',

```

- Publish config file from the terminal.

```java

php artisan vendor:publish

```

- Edit the new config file in the **config/asposecloud.php** and enter your **App Key** & **App SID**.

```java

return array(

    'baseUri' => 'http://api.aspose.com/v1.1',

    'appSID' => '',

    'appKey' => ''

);

```
## **Using**
### **Usage**
Anywhere in your application when you need to access class, just do:

```java

$object = Aspose::get($moduleName, $className, $fileName);

```

This will return you object of class and you can access properties and methods of class.

In order to access in **Laravel 5** application, use following namespace at the top of your file.

```java

use Aspose;

```
