# moosyl.PaymentRequestApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_payment_request_by_id**](PaymentRequestApi.md#get_payment_request_by_id) | **GET** /payment-request/{id} | Get payment request
[**get_payment_request_by_transaction_by_transaction_id**](PaymentRequestApi.md#get_payment_request_by_transaction_by_transaction_id) | **GET** /payment-request/by-transaction/{transactionId} | Get payment request by transaction ID
[**patch_payment_request_by_transaction_id_refresh_status**](PaymentRequestApi.md#patch_payment_request_by_transaction_id_refresh_status) | **PATCH** /payment-request/{transactionId}/refresh-status | Refresh payment request status
[**post_payment_request**](PaymentRequestApi.md#post_payment_request) | **POST** /payment-request | Create payment request


# **get_payment_request_by_id**
> PaymentRequestGet get_payment_request_by_id(id)

Get payment request

Retrieve a payment request by ID

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.payment_request_get import PaymentRequestGet
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
    api_instance = moosyl.PaymentRequestApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get payment request
        api_response = api_instance.get_payment_request_by_id(id)
        print("The response of PaymentRequestApi->get_payment_request_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentRequestApi->get_payment_request_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**PaymentRequestGet**](PaymentRequestGet.md)

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

# **get_payment_request_by_transaction_by_transaction_id**
> PaymentRequestGet get_payment_request_by_transaction_by_transaction_id(transaction_id)

Get payment request by transaction ID

Retrieve a payment request by transaction ID

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.payment_request_get import PaymentRequestGet
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
    api_instance = moosyl.PaymentRequestApi(api_client)
    transaction_id = 'transaction_id_example' # str | 

    try:
        # Get payment request by transaction ID
        api_response = api_instance.get_payment_request_by_transaction_by_transaction_id(transaction_id)
        print("The response of PaymentRequestApi->get_payment_request_by_transaction_by_transaction_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentRequestApi->get_payment_request_by_transaction_by_transaction_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transaction_id** | **str**|  | 

### Return type

[**PaymentRequestGet**](PaymentRequestGet.md)

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

# **patch_payment_request_by_transaction_id_refresh_status**
> PaymentRequestRefreshStatus patch_payment_request_by_transaction_id_refresh_status(transaction_id)

Refresh payment request status

Refresh the status of a payment request by transaction ID. Requires secret API key.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.payment_request_refresh_status import PaymentRequestRefreshStatus
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
    api_instance = moosyl.PaymentRequestApi(api_client)
    transaction_id = 'transaction_id_example' # str | 

    try:
        # Refresh payment request status
        api_response = api_instance.patch_payment_request_by_transaction_id_refresh_status(transaction_id)
        print("The response of PaymentRequestApi->patch_payment_request_by_transaction_id_refresh_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentRequestApi->patch_payment_request_by_transaction_id_refresh_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transaction_id** | **str**|  | 

### Return type

[**PaymentRequestRefreshStatus**](PaymentRequestRefreshStatus.md)

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

# **post_payment_request**
> PaymentRequestGet post_payment_request(payment_request_create)

Create payment request

Create a new payment request that can be used to collect payments. Requires secret API key.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.payment_request_create import PaymentRequestCreate
from moosyl.models.payment_request_get import PaymentRequestGet
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
    api_instance = moosyl.PaymentRequestApi(api_client)
    payment_request_create = moosyl.PaymentRequestCreate() # PaymentRequestCreate | 

    try:
        # Create payment request
        api_response = api_instance.post_payment_request(payment_request_create)
        print("The response of PaymentRequestApi->post_payment_request:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentRequestApi->post_payment_request: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payment_request_create** | [**PaymentRequestCreate**](PaymentRequestCreate.md)|  | 

### Return type

[**PaymentRequestGet**](PaymentRequestGet.md)

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

