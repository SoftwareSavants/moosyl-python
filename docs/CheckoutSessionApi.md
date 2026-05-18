# moosyl.CheckoutSessionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_checkout_session_public_by_id**](CheckoutSessionApi.md#get_checkout_session_public_by_id) | **GET** /checkout-session/public/{id} | Get public checkout session
[**post_checkout_session**](CheckoutSessionApi.md#post_checkout_session) | **POST** /checkout-session | Create checkout session
[**post_checkout_session_public_by_id_pay**](CheckoutSessionApi.md#post_checkout_session_public_by_id_pay) | **POST** /checkout-session/public/{id}/pay | Pay public checkout session
[**post_checkout_session_public_by_id_switch_method**](CheckoutSessionApi.md#post_checkout_session_public_by_id_switch_method) | **POST** /checkout-session/public/{id}/switch-method | Switch public checkout method


# **get_checkout_session_public_by_id**
> CheckoutSessionGet get_checkout_session_public_by_id(id)

Get public checkout session

Get checkout session details without an API key.

### Example


```python
import moosyl
from moosyl.models.checkout_session_get import CheckoutSessionGet
from moosyl.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = moosyl.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with moosyl.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moosyl.CheckoutSessionApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get public checkout session
        api_response = api_instance.get_checkout_session_public_by_id(id)
        print("The response of CheckoutSessionApi->get_checkout_session_public_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CheckoutSessionApi->get_checkout_session_public_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**CheckoutSessionGet**](CheckoutSessionGet.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_checkout_session**
> CheckoutSessionCreate post_checkout_session(checkout_session_create_body)

Create checkout session

Create a hosted checkout session from paymentRequestId, or from transactionId (optionally creating the payment request when amount is provided).

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.checkout_session_create import CheckoutSessionCreate
from moosyl.models.checkout_session_create_body import CheckoutSessionCreateBody
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
    api_instance = moosyl.CheckoutSessionApi(api_client)
    checkout_session_create_body = moosyl.CheckoutSessionCreateBody() # CheckoutSessionCreateBody | 

    try:
        # Create checkout session
        api_response = api_instance.post_checkout_session(checkout_session_create_body)
        print("The response of CheckoutSessionApi->post_checkout_session:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CheckoutSessionApi->post_checkout_session: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **checkout_session_create_body** | [**CheckoutSessionCreateBody**](CheckoutSessionCreateBody.md)|  | 

### Return type

[**CheckoutSessionCreate**](CheckoutSessionCreate.md)

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

# **post_checkout_session_public_by_id_pay**
> PostCheckoutSessionPublicByIdPay200Response post_checkout_session_public_by_id_pay(id, checkout_session_pay_body)

Pay public checkout session

Create payment for a checkout session without requiring API key in the client.

### Example


```python
import moosyl
from moosyl.models.checkout_session_pay_body import CheckoutSessionPayBody
from moosyl.models.post_checkout_session_public_by_id_pay200_response import PostCheckoutSessionPublicByIdPay200Response
from moosyl.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = moosyl.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with moosyl.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moosyl.CheckoutSessionApi(api_client)
    id = 'id_example' # str | 
    checkout_session_pay_body = moosyl.CheckoutSessionPayBody() # CheckoutSessionPayBody | 

    try:
        # Pay public checkout session
        api_response = api_instance.post_checkout_session_public_by_id_pay(id, checkout_session_pay_body)
        print("The response of CheckoutSessionApi->post_checkout_session_public_by_id_pay:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CheckoutSessionApi->post_checkout_session_public_by_id_pay: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **checkout_session_pay_body** | [**CheckoutSessionPayBody**](CheckoutSessionPayBody.md)|  | 

### Return type

[**PostCheckoutSessionPublicByIdPay200Response**](PostCheckoutSessionPublicByIdPay200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_checkout_session_public_by_id_switch_method**
> CheckoutSessionSwitchMethod post_checkout_session_public_by_id_switch_method(id, checkout_session_select_method_body)

Switch public checkout method

Switch checkout method and cancel the latest pending payment when present.

### Example


```python
import moosyl
from moosyl.models.checkout_session_select_method_body import CheckoutSessionSelectMethodBody
from moosyl.models.checkout_session_switch_method import CheckoutSessionSwitchMethod
from moosyl.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = moosyl.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with moosyl.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moosyl.CheckoutSessionApi(api_client)
    id = 'id_example' # str | 
    checkout_session_select_method_body = moosyl.CheckoutSessionSelectMethodBody() # CheckoutSessionSelectMethodBody | 

    try:
        # Switch public checkout method
        api_response = api_instance.post_checkout_session_public_by_id_switch_method(id, checkout_session_select_method_body)
        print("The response of CheckoutSessionApi->post_checkout_session_public_by_id_switch_method:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CheckoutSessionApi->post_checkout_session_public_by_id_switch_method: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **checkout_session_select_method_body** | [**CheckoutSessionSelectMethodBody**](CheckoutSessionSelectMethodBody.md)|  | 

### Return type

[**CheckoutSessionSwitchMethod**](CheckoutSessionSwitchMethod.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response for status 200 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

