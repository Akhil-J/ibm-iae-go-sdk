[![Build Status](https://api.travis-ci.com/IBM/ibm-iae-go-sdk.svg?branch=master)](https://app.travis-ci.com/IBM/ibm-iae-go-sdk)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

# IBM Cloud Analytics Engine Go SDK Version 2.2.0
Go client library to interact with the various [IBM Analytics Engine APIs](https://cloud.ibm.com/apidocs/ibm-analytics-engine).

## Table of Contents
<!--
  The TOC below is generated using the `markdown-toc` node package.

      https://github.com/jonschlinkert/markdown-toc

  You should regenerate the TOC after making changes to this file.

      npx markdown-toc -i README.md
  -->

<!-- toc -->

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
    + [`go get` command](#go-get-command)
    + [Go modules](#go-modules)
    + [`dep` dependency manager](#dep-dependency-manager)
- [Using the SDK](#using-the-sdk)
- [Questions](#questions)
- [Issues](#issues)
- [Open source @ IBM](#open-source--ibm)
- [Contributing](#contributing)
- [License](#license)

<!-- tocstop -->

## Overview

The IBM Cloud IBM Analytics Engine API Go SDK allows developers to programmatically interact with the following IBM Cloud services:

Service Name | Package name 
--- | --- 
[IBM Analytics Engine v2](https://cloud.ibm.com/apidocs/ibm-analytics-engine/ibm-analytics-engine-v2) | ibmanalyticsengineapiv2
[IBM Analytics Engine v3](https://cloud.ibm.com/apidocs/ibm-analytics-engine/ibm-analytics-engine-v3) | ibmanalyticsengineapiv3

**NOTE**

IBM Analytics Engine v2 is for the classic plans : Lite, Standard Hourly and Standard monthly.
These plans are now deprecated.

IBM Analytics Engine v3 is for the Standard Serverless for Apache Spark plan

## Prerequisites

[ibm-cloud-onboarding]: https://cloud.ibm.com/registration

* An [IBM Cloud][ibm-cloud-onboarding] account.
* An IAM API key to allow the SDK to access your account. Create one [here](https://cloud.ibm.com/iam/apikeys).
* Go version 1.18 or above.

## Installation
The current version of this SDK: 2.2.0

There are a few different ways to download and install the IBM Analytics Engine API Go SDK project for use by your
Go application:

#### `go get` command  
Use this command to download and install the SDK (along with its dependencies) to allow your Go application to use it:

```
go get -u github.com/IBM/ibm-iae-go-sdk/...
```

If you are creating a new go project then create a folder inside $GOPATH and install packages. For example:
```
mkdir -p ~/go/src/go-test
cd ~/go/src/go-test
go get -u github.com/IBM/ibm-iae-go-sdk/...
```

#### Go modules  
If your application is using Go modules, you can add a suitable import to your Go application, like this:

```go
import (
	"github.com/IBM/ibm-iae-go-sdk/ibmanalyticsengineapiv2"
)
```

then run `go mod tidy` to download and install the new dependency and update your Go application's `go.mod` file.

If you are creating a new go project then create a folder outside $GOPATH, init module, and install packages. For example:
```
mkdir -p ~/go-test
cd ~/go-test
go mod init <some-name>
go get -u github.com/IBM/ibm-iae-go-sdk
```

## Using the SDK
For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md)

In [setting client options programatically](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md#setting-client-options-programmatically) to instantiate the class, provide the following two values:
1. [IAM API Key](https://cloud.ibm.com/docs/iam?topic=iam-userapikey#create_user_key)
1. [Service URLs](https://cloud.ibm.com/apidocs/ibm-analytics-engine#service-endpoints)

## Questions

If you are having difficulties using this SDK or have a question about the IBM Cloud services,
please ask a question at 
[Stack Overflow](http://stackoverflow.com/questions/ask?tags=ibm-cloud).

## Issues
If you encounter an issue with the project, you are welcome to submit a
[bug report](<github-repo-url>/issues).
Before that, please search for similar issues. It's possible that someone has already reported the problem.

## Open source @ IBM
Find more open source projects on the [IBM Github Page](http://ibm.github.io/)

## Contributing
See [CONTRIBUTING](CONTRIBUTING.md).

## License

This SDK project is released under the Apache 2.0 license.
The license's full text can be found in [LICENSE](LICENSE).
