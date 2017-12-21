# AccountApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**balanceGet**](AccountApi.md#balanceGet) | **GET** /balance | 


<a name="balanceGet"></a>
# **balanceGet**
> balanceGet(apiKey)



This API get users balance. 

### Example
```java
// Import classes:
//import io.swagger.client.api.AccountApi;

AccountApi apiInstance = new AccountApi();
String apiKey = "apiKey_example"; // String | API Key
try {
    apiInstance.balanceGet(apiKey);
} catch (ApiException e) {
    System.err.println("Exception when calling AccountApi#balanceGet");
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

