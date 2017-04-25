# TeslaModelSApi_.DefaultApi

All URIs are relative to *https://virtserver.swaggerhub.com/TeslaDemoOrgApril/TeslaModelSAPI23/0.0.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**climateState**](DefaultApi.md#climateState) | **GET** /vehicles/{id}/data_request/climate_state | 
[**driveState**](DefaultApi.md#driveState) | **GET** /vehicles/{id}/data_request/drive_state | 
[**setTemps**](DefaultApi.md#setTemps) | **POST** /vehicles/{id}/command/set_temps | 
[**vehicleGet**](DefaultApi.md#vehicleGet) | **GET** /vehicle | 


<a name="climateState"></a>
# **climateState**
> InlineResponse2003 climateState(id)



Returns the current temperature and climate control state.

### Example
```javascript
var TeslaModelSApi_ = require('tesla_model_s_api_');

var apiInstance = new TeslaModelSApi_.DefaultApi();

var id = "id_example"; // String | The ID number of the car


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.climateState(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| The ID number of the car | 

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="driveState"></a>
# **driveState**
> InlineResponse2001 driveState(id)



Returns the driving and position state of the vehicle.

### Example
```javascript
var TeslaModelSApi_ = require('tesla_model_s_api_');

var apiInstance = new TeslaModelSApi_.DefaultApi();

var id = "id_example"; // String | The ID number of the car


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.driveState(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| The ID number of the car | 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="setTemps"></a>
# **setTemps**
> InlineResponse2002 setTemps(id, driverTemp, passengerTemp)



Set the temperature target for the HVAC system.

### Example
```javascript
var TeslaModelSApi_ = require('tesla_model_s_api_');

var apiInstance = new TeslaModelSApi_.DefaultApi();

var id = "id_example"; // String | The ID number of the car

var driverTemp = "driverTemp_example"; // String | The desired temperature on the driver's side in celcius.

var passengerTemp = "passengerTemp_example"; // String | The desired temperature on the passenger's side in celcius.


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.setTemps(id, driverTemp, passengerTemp, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| The ID number of the car | 
 **driverTemp** | **String**| The desired temperature on the driver&#39;s side in celcius. | 
 **passengerTemp** | **String**| The desired temperature on the passenger&#39;s side in celcius. | 

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="vehicleGet"></a>
# **vehicleGet**
> InlineResponse200 vehicleGet()



Details about owned vehicle

### Example
```javascript
var TeslaModelSApi_ = require('tesla_model_s_api_');

var apiInstance = new TeslaModelSApi_.DefaultApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.vehicleGet(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

