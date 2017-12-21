# NumberApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**numbersGet**](NumberApi.md#numbersGet) | **GET** /numbers | 


<a name="numbersGet"></a>
# **numbersGet**
> numbersGet(apiKey, page)



This API get users numbers. 

### Example
```java
// Import classes:
//import io.swagger.client.api.NumberApi;

NumberApi apiInstance = new NumberApi();
String apiKey = "apiKey_example"; // String | API Key
String page = "page_example"; // String | Page to display
try {
    apiInstance.numbersGet(apiKey, page);
} catch (ApiException e) {
    System.err.println("Exception when calling NumberApi#numbersGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **String**| API Key |
 **page** | **String**| Page to display | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

