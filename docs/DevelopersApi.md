# WhereIsApi.DevelopersApi

All URIs are relative to *https://virtserver.swaggerhub.com/mikeonthemike/whereIs/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**findTeamMember**](DevelopersApi.md#findTeamMember) | **GET** /whereAbouts | searches whereabouts
[**searchLocation**](DevelopersApi.md#searchLocation) | **GET** /location | searches locations
[**updateProjectLocation**](DevelopersApi.md#updateProjectLocation) | **POST** /whereAbouts | updates location for a given team member and date


<a name="findTeamMember"></a>
# **findTeamMember**
> [Whereabouts] findTeamMember(opts)

searches whereabouts

By passing in the appropriate parameter, you can find out where someone is 

### Example
```javascript
var WhereIsApi = require('where_is_api');

var apiInstance = new WhereIsApi.DevelopersApi();

var opts = { 
  'teamMemberName': "teamMemberName_example", // String | pass a name in
  'projectDate': "projectDate_example" // String | pass a date in
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.findTeamMember(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamMemberName** | **String**| pass a name in | [optional] 
 **projectDate** | **String**| pass a date in | [optional] 

### Return type

[**[Whereabouts]**](Whereabouts.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="searchLocation"></a>
# **searchLocation**
> [TeamMember] searchLocation(opts)

searches locations

By passing in the appropriate parameter, you can search for locations 

### Example
```javascript
var WhereIsApi = require('where_is_api');

var apiInstance = new WhereIsApi.DevelopersApi();

var opts = { 
  'teamMemberName': "teamMemberName_example" // String | pass a name in
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.searchLocation(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamMemberName** | **String**| pass a name in | [optional] 

### Return type

[**[TeamMember]**](TeamMember.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateProjectLocation"></a>
# **updateProjectLocation**
> [Whereabouts] updateProjectLocation(teamMemberName, projectLocation, _date)

updates location for a given team member and date

By passing in the appropriate parameters, you can set your location for a given date 

### Example
```javascript
var WhereIsApi = require('where_is_api');

var apiInstance = new WhereIsApi.DevelopersApi();

var teamMemberName = "teamMemberName_example"; // String | pass a name in

var projectLocation = "projectLocation_example"; // String | location to be set

var _date = "_date_example"; // String | date for the location change


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.updateProjectLocation(teamMemberName, projectLocation, _date, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamMemberName** | **String**| pass a name in | 
 **projectLocation** | **String**| location to be set | 
 **_date** | **String**| date for the location change | 

### Return type

[**[Whereabouts]**](Whereabouts.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

