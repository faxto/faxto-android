# FaxApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**faxDocumentIdCostsGet**](FaxApi.md#faxDocumentIdCostsGet) | **GET** /fax/{document_id}/costs | 
[**faxHistoryGet**](FaxApi.md#faxHistoryGet) | **GET** /fax-history | 
[**faxJobIdStatusGet**](FaxApi.md#faxJobIdStatusGet) | **GET** /fax/{job_id}/status | 
[**faxPost**](FaxApi.md#faxPost) | **POST** /fax | 


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

<a name="faxHistoryGet"></a>
# **faxHistoryGet**
> faxHistoryGet(apiKey, limit, page)



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
    apiInstance.faxHistoryGet(apiKey, limit, page);
} catch (ApiException e) {
    System.err.println("Exception when calling FaxApi#faxHistoryGet");
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

<a name="faxPost"></a>
# **faxPost**
> faxPost(apiKey, faxNumber, documentId, tsiNumber, file, deleteFile)



This API send the fax. When we send fax using API, Fax.to send a POST to the Callback URL you specified in https://fax.to/member/api/live. Fax.to send POST data with the following information fax_job_id, status and message. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FaxApi;

FaxApi apiInstance = new FaxApi();
String apiKey = "apiKey_example"; // String | API Key
String faxNumber = "faxNumber_example"; // String | Fax Number
Integer documentId = 56; // Integer | Document id. If you want to use existing document you need to specify the document_id
String tsiNumber = "tsiNumber_example"; // String | If we want to to change the text or number that appear on 'from' or 'sender' of the fax
File file = new File("/path/to/file.txt"); // File | PDF file to upload
Integer deleteFile = 56; // Integer | Whether to delete file after fax transaction. (put 1 to delete)
try {
    apiInstance.faxPost(apiKey, faxNumber, documentId, tsiNumber, file, deleteFile);
} catch (ApiException e) {
    System.err.println("Exception when calling FaxApi#faxPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **faxNumber** | **String**| Fax Number |
 **documentId** | **Integer**| Document id. If you want to use existing document you need to specify the document_id | [optional]
 **tsiNumber** | **String**| If we want to to change the text or number that appear on &#39;from&#39; or &#39;sender&#39; of the fax | [optional]
 **file** | **File**| PDF file to upload | [optional]
 **deleteFile** | **Integer**| Whether to delete file after fax transaction. (put 1 to delete) | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

