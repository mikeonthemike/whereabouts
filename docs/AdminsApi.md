# WhereIsApi.AdminsApi

All URIs are relative to *https://virtserver.swaggerhub.com/mikeonthemike/whereIs/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**updateBaseLocation**](AdminsApi.md#updateBaseLocation) | **POST** /location | updates base location


<a name="updateBaseLocation"></a>
# **updateBaseLocation**
> [TeamMember] updateBaseLocation(teamMemberName, baseLocation)

updates base location

By passing in the appropriate parameters, you can set your location 

### Example
```javascript
var WhereIsApi = require('where_is_api');

var apiInstance = new WhereIsApi.AdminsApi();

var teamMemberName = "teamMemberName_example"; // String | pass a name in

var baseLocation = "baseLocation_example"; // String | location to be set


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.updateBaseLocation(teamMemberName, baseLocation, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamMemberName** | **String**| pass a name in | 
 **baseLocation** | **String**| location to be set | 

### Return type

[**[TeamMember]**](TeamMember.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

