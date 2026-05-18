# moosyl.ConnectApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_connect_revoke**](ConnectApi.md#delete_connect_revoke) | **DELETE** /connect/revoke | Revoke a platform connection
[**post_connect_exchange**](ConnectApi.md#post_connect_exchange) | **POST** /connect/exchange | Exchange authorization code for API credentials


# **delete_connect_revoke**
> DeleteConnectRevoke200Response delete_connect_revoke(delete_connect_revoke_request)

Revoke a platform connection

Revoke a previously authorized connection between a platform and a Moosyl account.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.delete_connect_revoke200_response import DeleteConnectRevoke200Response
from moosyl.models.delete_connect_revoke_request import DeleteConnectRevokeRequest
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
    api_instance = moosyl.ConnectApi(api_client)
    delete_connect_revoke_request = moosyl.DeleteConnectRevokeRequest() # DeleteConnectRevokeRequest | 

    try:
        # Revoke a platform connection
        api_response = api_instance.delete_connect_revoke(delete_connect_revoke_request)
        print("The response of ConnectApi->delete_connect_revoke:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->delete_connect_revoke: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delete_connect_revoke_request** | [**DeleteConnectRevokeRequest**](DeleteConnectRevokeRequest.md)|  | 

### Return type

[**DeleteConnectRevoke200Response**](DeleteConnectRevoke200Response.md)

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

# **post_connect_exchange**
> PostConnectExchange200Response post_connect_exchange(post_connect_exchange_request)

Exchange authorization code for API credentials

Exchange a short-lived authorization code (obtained from the /connect flow) for the user's publishable key, secret key, and webhook secret. A webhook will be created using the provided endpoints.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.post_connect_exchange200_response import PostConnectExchange200Response
from moosyl.models.post_connect_exchange_request import PostConnectExchangeRequest
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
    api_instance = moosyl.ConnectApi(api_client)
    post_connect_exchange_request = moosyl.PostConnectExchangeRequest() # PostConnectExchangeRequest | 

    try:
        # Exchange authorization code for API credentials
        api_response = api_instance.post_connect_exchange(post_connect_exchange_request)
        print("The response of ConnectApi->post_connect_exchange:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->post_connect_exchange: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_connect_exchange_request** | [**PostConnectExchangeRequest**](PostConnectExchangeRequest.md)|  | 

### Return type

[**PostConnectExchange200Response**](PostConnectExchange200Response.md)

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

