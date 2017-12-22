# swagger-android-client

## Requirements

Building the API client library requires [Maven](https://maven.apache.org/) to be installed.

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn deploy
```

Refer to the [official documentation](https://maven.apache.org/plugins/maven-deploy-plugin/usage.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
    <groupId>io.swagger</groupId>
    <artifactId>swagger-android-client</artifactId>
    <version>1.0.0</version>
    <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "io.swagger:swagger-android-client:1.0.0"
```

### Others

At first generate the JAR by executing:

    mvn package

Then manually install the following JARs:

* target/swagger-android-client-1.0.0.jar
* target/lib/*.jar

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

import io.swagger.client.api.AccountApi;

public class AccountApiExample {

    public static void main(String[] args) {
        AccountApi apiInstance = new AccountApi();
        String apiKey = "apiKey_example"; // String | API Key
        try {
            apiInstance.balanceGet(apiKey);
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountApi#balanceGet");
            e.printStackTrace();
        }
    }
}

```

## Documentation for API Endpoints

All URIs are relative to *https://fax.to/api/v2*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AccountApi* | [**balanceGet**](docs/AccountApi.md#balanceGet) | **GET** /balance | 
*CountryApi* | [**areacodesCountryCodeStateIdGet**](docs/CountryApi.md#areacodesCountryCodeStateIdGet) | **GET** /areacodes/{countryCode}/{stateId} | 
*CountryApi* | [**countriesCountryCodeDidgroupsGet**](docs/CountryApi.md#countriesCountryCodeDidgroupsGet) | **GET** /countries/{countryCode}/didgroups | 
*CountryApi* | [**countriesDidgroupsDidGroupIdProvisionPost**](docs/CountryApi.md#countriesDidgroupsDidGroupIdProvisionPost) | **POST** /countries/didgroups/{didGroupId}/provision | 
*CountryApi* | [**countriesGet**](docs/CountryApi.md#countriesGet) | **GET** /countries | 
*CountryApi* | [**statesCountryCodeGet**](docs/CountryApi.md#statesCountryCodeGet) | **GET** /states/{countryCode} | 
*FaxApi* | [**faxDocumentIdCostsGet**](docs/FaxApi.md#faxDocumentIdCostsGet) | **GET** /fax/{document_id}/costs | 
*FaxApi* | [**faxGet**](docs/FaxApi.md#faxGet) | **GET** /fax | 
*FaxApi* | [**faxJobIdStatusGet**](docs/FaxApi.md#faxJobIdStatusGet) | **GET** /fax/{job_id}/status | 
*FaxApi* | [**incomingFaxesGet**](docs/FaxApi.md#incomingFaxesGet) | **GET** /incoming-faxes | 
*FaxApi* | [**incomingFaxesNumberGet**](docs/FaxApi.md#incomingFaxesNumberGet) | **GET** /incoming-faxes/{number} | 
*FaxApi* | [**provisionNumbersGet**](docs/FaxApi.md#provisionNumbersGet) | **GET** /provision-numbers | 
*FilesApi* | [**fileCleanGet**](docs/FilesApi.md#fileCleanGet) | **GET** /file-clean | 
*FilesApi* | [**fileGeneratePreviewGet**](docs/FilesApi.md#fileGeneratePreviewGet) | **GET** /file-generate-preview | 
*FilesApi* | [**filesGet**](docs/FilesApi.md#filesGet) | **GET** /files | 
*FilesApi* | [**filesIdDelete**](docs/FilesApi.md#filesIdDelete) | **DELETE** /files/{id} | 
*FilesApi* | [**filesPost**](docs/FilesApi.md#filesPost) | **POST** /files | 
*NumberApi* | [**numbersGet**](docs/NumberApi.md#numbersGet) | **GET** /numbers | 


## Documentation for Models



## Documentation for Authorization

All endpoints do not require authorization.
Authentication schemes defined for the API:

## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author



