# FaxApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**faxDocumentIdCostsGet**](FaxApi.md#faxDocumentIdCostsGet) | **GET** /fax/{document_id}/costs | 
[**faxGet**](FaxApi.md#faxGet) | **GET** /fax | 
[**faxJobIdStatusGet**](FaxApi.md#faxJobIdStatusGet) | **GET** /fax/{job_id}/status | 
[**incomingFaxesGet**](FaxApi.md#incomingFaxesGet) | **GET** /incoming-faxes | 
[**incomingFaxesNumberGet**](FaxApi.md#incomingFaxesNumberGet) | **GET** /incoming-faxes/{number} | 
[**provisionNumbersGet**](FaxApi.md#provisionNumbersGet) | **GET** /provision-numbers | 


<a name="faxDocumentIdCostsGet"></a>
# **faxDocumentIdCostsGet**
> faxDocumentIdCostsGet(apiKey, faxNumber, documentId)



This API get the cost of a sending fax. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FaxApi;

FaxApi apiInstance = new FaxApi();
String apiKey = "apiKey_example"; // String | API Key
String faxNumber = "faxNumber_example"; // String | Fax Number
BigDecimal documentId = new BigDecimal(); // BigDecimal | id of the file / document_id
try {
    apiInstance.faxDocumentIdCostsGet(apiKey, faxNumber, documentId);
} catch (ApiException e) {
    System.err.println("Exception when calling FaxApi#faxDocumentIdCostsGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **faxNumber** | **String**| Fax Number |
 **documentId** | **BigDecimal**| id of the file / document_id |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="faxGet"></a>
# **faxGet**
> faxGet(apiKey, limit, page)



This API get all fax history. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FaxApi;

FaxApi apiInstance = new FaxApi();
String apiKey = "apiKey_example"; // String | API Key
String limit = "limit_example"; // String | Number of records to return
String page = "page_example"; // String | Page to display
try {
    apiInstance.faxGet(apiKey, limit, page);
} catch (ApiException e) {
    System.err.println("Exception when calling FaxApi#faxGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **limit** | **String**| Number of records to return | [optional]
 **page** | **String**| Page to display | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="faxJobIdStatusGet"></a>
# **faxJobIdStatusGet**
> faxJobIdStatusGet(apiKey, jobId)



This API get the status of the fax. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FaxApi;

FaxApi apiInstance = new FaxApi();
String apiKey = "apiKey_example"; // String | API Key
BigDecimal jobId = new BigDecimal(); // BigDecimal | id of the fax job
try {
    apiInstance.faxJobIdStatusGet(apiKey, jobId);
} catch (ApiException e) {
    System.err.println("Exception when calling FaxApi#faxJobIdStatusGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **jobId** | **BigDecimal**| id of the fax job |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="incomingFaxesGet"></a>
# **incomingFaxesGet**
> incomingFaxesGet(apiKey)



This API get faxes . 

### Example
```java
// Import classes:
//import io.swagger.client.api.FaxApi;

FaxApi apiInstance = new FaxApi();
String apiKey = "apiKey_example"; // String | API Key
try {
    apiInstance.incomingFaxesGet(apiKey);
} catch (ApiException e) {
    System.err.println("Exception when calling FaxApi#incomingFaxesGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="incomingFaxesNumberGet"></a>
# **incomingFaxesNumberGet**
> incomingFaxesNumberGet(apiKey, number)



This API get faxes  by number. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FaxApi;

FaxApi apiInstance = new FaxApi();
String apiKey = "apiKey_example"; // String | API Key
String number = "number_example"; // String | Number in the fax
try {
    apiInstance.incomingFaxesNumberGet(apiKey, number);
} catch (ApiException e) {
    System.err.println("Exception when calling FaxApi#incomingFaxesNumberGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **number** | **String**| Number in the fax |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="provisionNumbersGet"></a>
# **provisionNumbersGet**
> provisionNumbersGet(apiKey, limit)



This API get Provision numbers. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FaxApi;

FaxApi apiInstance = new FaxApi();
String apiKey = "apiKey_example"; // String | API Key
String limit = "limit_example"; // String | Limit to display
try {
    apiInstance.provisionNumbersGet(apiKey, limit);
} catch (ApiException e) {
    System.err.println("Exception when calling FaxApi#provisionNumbersGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **limit** | **String**| Limit to display | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

