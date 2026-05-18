# moosyl.PricesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_prices_by_id**](PricesApi.md#get_prices_by_id) | **GET** /prices/{id} | Get price
[**patch_prices_by_id**](PricesApi.md#patch_prices_by_id) | **PATCH** /prices/{id} | Update price
[**patch_prices_by_id_archive**](PricesApi.md#patch_prices_by_id_archive) | **PATCH** /prices/{id}/archive | Archive price
[**post_prices**](PricesApi.md#post_prices) | **POST** /prices/ | Create price


# **get_prices_by_id**
> PriceGet get_prices_by_id(id)

Get price

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.price_get import PriceGet
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
    api_instance = moosyl.PricesApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get price
        api_response = api_instance.get_prices_by_id(id)
        print("The response of PricesApi->get_prices_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PricesApi->get_prices_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**PriceGet**](PriceGet.md)

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

# **patch_prices_by_id**
> PriceGet patch_prices_by_id(id, price_update)

Update price

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.price_get import PriceGet
from moosyl.models.price_update import PriceUpdate
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
    api_instance = moosyl.PricesApi(api_client)
    id = 'id_example' # str | 
    price_update = moosyl.PriceUpdate() # PriceUpdate | 

    try:
        # Update price
        api_response = api_instance.patch_prices_by_id(id, price_update)
        print("The response of PricesApi->patch_prices_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PricesApi->patch_prices_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **price_update** | [**PriceUpdate**](PriceUpdate.md)|  | 

### Return type

[**PriceGet**](PriceGet.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_prices_by_id_archive**
> Success patch_prices_by_id_archive(id)

Archive price

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.success import Success
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
    api_instance = moosyl.PricesApi(api_client)
    id = 'id_example' # str | 

    try:
        # Archive price
        api_response = api_instance.patch_prices_by_id_archive(id)
        print("The response of PricesApi->patch_prices_by_id_archive:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PricesApi->patch_prices_by_id_archive: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**Success**](Success.md)

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

# **post_prices**
> PriceGet post_prices(price_create)

Create price

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.price_create import PriceCreate
from moosyl.models.price_get import PriceGet
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
    api_instance = moosyl.PricesApi(api_client)
    price_create = moosyl.PriceCreate() # PriceCreate | 

    try:
        # Create price
        api_response = api_instance.post_prices(price_create)
        print("The response of PricesApi->post_prices:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PricesApi->post_prices: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **price_create** | [**PriceCreate**](PriceCreate.md)|  | 

### Return type

[**PriceGet**](PriceGet.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

