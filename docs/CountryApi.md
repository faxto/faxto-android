# CountryApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**areacodesCountryCodeStateIdGet**](CountryApi.md#areacodesCountryCodeStateIdGet) | **GET** /areacodes/{countryCode}/{stateId} | 
[**countriesCountryCodeDidgroupsGet**](CountryApi.md#countriesCountryCodeDidgroupsGet) | **GET** /countries/{countryCode}/didgroups | 
[**countriesDidgroupsDidGroupIdProvisionPost**](CountryApi.md#countriesDidgroupsDidGroupIdProvisionPost) | **POST** /countries/didgroups/{didGroupId}/provision | 
[**countriesGet**](CountryApi.md#countriesGet) | **GET** /countries | 
[**statesCountryCodeGet**](CountryApi.md#statesCountryCodeGet) | **GET** /states/{countryCode} | 


<a name="areacodesCountryCodeStateIdGet"></a>
# **areacodesCountryCodeStateIdGet**
> areacodesCountryCodeStateIdGet(countryCode, stateId)



This API get areacodes . 

### Example
```java
// Import classes:
//import io.swagger.client.api.CountryApi;

CountryApi apiInstance = new CountryApi();
String countryCode = "countryCode_example"; // String | countryCode in the Country
String stateId = "stateId_example"; // String | stateId in the Country
try {
    apiInstance.areacodesCountryCodeStateIdGet(countryCode, stateId);
} catch (ApiException e) {
    System.err.println("Exception when calling CountryApi#areacodesCountryCodeStateIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **countryCode** | **String**| countryCode in the Country |
 **stateId** | **String**| stateId in the Country |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="countriesCountryCodeDidgroupsGet"></a>
# **countriesCountryCodeDidgroupsGet**
> countriesCountryCodeDidgroupsGet(countryCode, didGroupIds, stateId, cityNamePattern)



This API didgroups countryCode. 

### Example
```java
// Import classes:
//import io.swagger.client.api.CountryApi;

CountryApi apiInstance = new CountryApi();
String countryCode = "countryCode_example"; // String | countryCode in the Country
String didGroupIds = "didGroupIds_example"; // String | didGroupId in the Country
String stateId = "stateId_example"; // String | stateId in the Country
String cityNamePattern = "cityNamePattern_example"; // String | cityNamePattern in the Country
try {
    apiInstance.countriesCountryCodeDidgroupsGet(countryCode, didGroupIds, stateId, cityNamePattern);
} catch (ApiException e) {
    System.err.println("Exception when calling CountryApi#countriesCountryCodeDidgroupsGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **countryCode** | **String**| countryCode in the Country |
 **didGroupIds** | **String**| didGroupId in the Country |
 **stateId** | **String**| stateId in the Country |
 **cityNamePattern** | **String**| cityNamePattern in the Country |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="countriesDidgroupsDidGroupIdProvisionPost"></a>
# **countriesDidgroupsDidGroupIdProvisionPost**
> countriesDidgroupsDidGroupIdProvisionPost(didGroupId)



This API didgroups provision. 

### Example
```java
// Import classes:
//import io.swagger.client.api.CountryApi;

CountryApi apiInstance = new CountryApi();
String didGroupId = "didGroupId_example"; // String | didGroupId in the Country
try {
    apiInstance.countriesDidgroupsDidGroupIdProvisionPost(didGroupId);
} catch (ApiException e) {
    System.err.println("Exception when calling CountryApi#countriesDidgroupsDidGroupIdProvisionPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **didGroupId** | **String**| didGroupId in the Country |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="countriesGet"></a>
# **countriesGet**
> countriesGet()



This API get countries. 

### Example
```java
// Import classes:
//import io.swagger.client.api.CountryApi;

CountryApi apiInstance = new CountryApi();
try {
    apiInstance.countriesGet();
} catch (ApiException e) {
    System.err.println("Exception when calling CountryApi#countriesGet");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="statesCountryCodeGet"></a>
# **statesCountryCodeGet**
> statesCountryCodeGet(countryCode)



This API get States . 

### Example
```java
// Import classes:
//import io.swagger.client.api.CountryApi;

CountryApi apiInstance = new CountryApi();
String countryCode = "countryCode_example"; // String | countryCode in the Country
try {
    apiInstance.statesCountryCodeGet(countryCode);
} catch (ApiException e) {
    System.err.println("Exception when calling CountryApi#statesCountryCodeGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **countryCode** | **String**| countryCode in the Country |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

