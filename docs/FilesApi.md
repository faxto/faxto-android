# FilesApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fileCleanGet**](FilesApi.md#fileCleanGet) | **GET** /file-clean | 
[**fileGeneratePreviewGet**](FilesApi.md#fileGeneratePreviewGet) | **GET** /file-generate-preview | 
[**filesGet**](FilesApi.md#filesGet) | **GET** /files | 
[**filesIdDelete**](FilesApi.md#filesIdDelete) | **DELETE** /files/{id} | 
[**filesPost**](FilesApi.md#filesPost) | **POST** /files | 


<a name="fileCleanGet"></a>
# **fileCleanGet**
> fileCleanGet(apiKey, documentId)



This API get clean file from document id. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FilesApi;

FilesApi apiInstance = new FilesApi();
String apiKey = "apiKey_example"; // String | API Key
String documentId = "documentId_example"; // String | Document ID in the fax
try {
    apiInstance.fileCleanGet(apiKey, documentId);
} catch (ApiException e) {
    System.err.println("Exception when calling FilesApi#fileCleanGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **documentId** | **String**| Document ID in the fax |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="fileGeneratePreviewGet"></a>
# **fileGeneratePreviewGet**
> fileGeneratePreviewGet(apiKey, documentId)



This API get generated preview file from document id. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FilesApi;

FilesApi apiInstance = new FilesApi();
String apiKey = "apiKey_example"; // String | API Key
String documentId = "documentId_example"; // String | Document ID in the fax
try {
    apiInstance.fileGeneratePreviewGet(apiKey, documentId);
} catch (ApiException e) {
    System.err.println("Exception when calling FilesApi#fileGeneratePreviewGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **documentId** | **String**| Document ID in the fax |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="filesGet"></a>
# **filesGet**
> filesGet(apiKey)



This API lists all the files 

### Example
```java
// Import classes:
//import io.swagger.client.api.FilesApi;

FilesApi apiInstance = new FilesApi();
String apiKey = "apiKey_example"; // String | API Key
try {
    apiInstance.filesGet(apiKey);
} catch (ApiException e) {
    System.err.println("Exception when calling FilesApi#filesGet");
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

<a name="filesIdDelete"></a>
# **filesIdDelete**
> filesIdDelete(apiKey, id)



This API deletes a single file. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FilesApi;

FilesApi apiInstance = new FilesApi();
String apiKey = "apiKey_example"; // String | API Key
BigDecimal id = new BigDecimal(); // BigDecimal | id of the file / document
try {
    apiInstance.filesIdDelete(apiKey, id);
} catch (ApiException e) {
    System.err.println("Exception when calling FilesApi#filesIdDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **id** | **BigDecimal**| id of the file / document |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="filesPost"></a>
# **filesPost**
> File filesPost(apiKey, file, addRemoteFile)



This API allows uploading of a single file. 

### Example
```java
// Import classes:
//import io.swagger.client.api.FilesApi;

FilesApi apiInstance = new FilesApi();
String apiKey = "apiKey_example"; // String | API Key
File file = new File("/path/to/file.txt"); // File | PDF file to upload
String addRemoteFile = "addRemoteFile_example"; // String | Given the remote file url
try {
    File result = apiInstance.filesPost(apiKey, file, addRemoteFile);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling FilesApi#filesPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **file** | **File**| PDF file to upload |
 **addRemoteFile** | **String**| Given the remote file url | [optional]

### Return type

[**File**](File.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

