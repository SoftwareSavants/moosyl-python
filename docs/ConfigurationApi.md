# moosyl.ConfigurationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_configuration**](ConfigurationApi.md#get_configuration) | **GET** /configuration | List configurations
[**get_configuration_by_id**](ConfigurationApi.md#get_configuration_by_id) | **GET** /configuration/{id} | Get configuration


# **get_configuration**
> ConfigurationList get_configuration()

List configurations

Retrieve all configurations for the current environment

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.configuration_list import ConfigurationList
from moosyl.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = moosyl.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKey
configuration.api_key['ApiKey'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKey'] = 'Bearer'

# Enter a context with an instance of the API client
with moosyl.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moosyl.ConfigurationApi(api_client)

    try:
        # List configurations
        api_response = api_instance.get_configuration()
        print("The response of ConfigurationApi->get_configuration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationApi->get_configuration: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ConfigurationList**](ConfigurationList.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_configuration_by_id**
> ConfigurationGet get_configuration_by_id(id)

Get configuration

Retrieve a specific configuration by ID. Requires secret API key.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.configuration_get import ConfigurationGet
from moosyl.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = moosyl.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKey
configuration.api_key['ApiKey'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKey'] = 'Bearer'

# Enter a context with an instance of the API client
with moosyl.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moosyl.ConfigurationApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get configuration
        api_response = api_instance.get_configuration_by_id(id)
        print("The response of ConfigurationApi->get_configuration_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConfigurationApi->get_configuration_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**ConfigurationGet**](ConfigurationGet.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

