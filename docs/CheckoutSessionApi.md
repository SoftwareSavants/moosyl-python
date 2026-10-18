# moosyl.CheckoutSessionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_checkout_session_public_by_id**](CheckoutSessionApi.md#get_checkout_session_public_by_id) | **GET** /checkout-session/public/{id} | Get public checkout session
[**get_checkout_session_public_by_id_payment_status**](CheckoutSessionApi.md#get_checkout_session_public_by_id_payment_status) | **GET** /checkout-session/public/{id}/payment-status | Poll a Gimtel checkout payment
[**post_checkout_session**](CheckoutSessionApi.md#post_checkout_session) | **POST** /checkout-session | Create checkout session
[**post_checkout_session_public_by_id_pay**](CheckoutSessionApi.md#post_checkout_session_public_by_id_pay) | **POST** /checkout-session/public/{id}/pay | Pay public checkout session
[**post_checkout_session_public_by_id_simulate_transfer**](CheckoutSessionApi.md#post_checkout_session_public_by_id_simulate_transfer) | **POST** /checkout-session/public/{id}/simulate-transfer | Simulate a Gimtel transfer (sandbox)
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

# **get_checkout_session_public_by_id_payment_status**
> GetCheckoutSessionPublicByIdPaymentStatus200Response get_checkout_session_public_by_id_payment_status(id, payment_id)

Poll a Gimtel checkout payment

Heartbeat for the hosted checkout: keeps the payment claimable while the payer is on the page and returns its status.

### Example


```python
import moosyl
from moosyl.models.get_checkout_session_public_by_id_payment_status200_response import GetCheckoutSessionPublicByIdPaymentStatus200Response
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
    payment_id = 'payment_id_example' # str | 

    try:
        # Poll a Gimtel checkout payment
        api_response = api_instance.get_checkout_session_public_by_id_payment_status(id, payment_id)
        print("The response of CheckoutSessionApi->get_checkout_session_public_by_id_payment_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CheckoutSessionApi->get_checkout_session_public_by_id_payment_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **payment_id** | **str**|  | 

### Return type

[**GetCheckoutSessionPublicByIdPaymentStatus200Response**](GetCheckoutSessionPublicByIdPaymentStatus200Response.md)

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

# **post_checkout_session_public_by_id_simulate_transfer**
> GetCheckoutSessionPublicByIdPaymentStatus200Response post_checkout_session_public_by_id_simulate_transfer(id, post_checkout_session_public_by_id_simulate_transfer_request)

Simulate a Gimtel transfer (sandbox)

Sandbox only. Completes the pending Gimtel payment as if the payer had transferred the exact amount.

### Example


```python
import moosyl
from moosyl.models.get_checkout_session_public_by_id_payment_status200_response import GetCheckoutSessionPublicByIdPaymentStatus200Response
from moosyl.models.post_checkout_session_public_by_id_simulate_transfer_request import PostCheckoutSessionPublicByIdSimulateTransferRequest
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
    post_checkout_session_public_by_id_simulate_transfer_request = moosyl.PostCheckoutSessionPublicByIdSimulateTransferRequest() # PostCheckoutSessionPublicByIdSimulateTransferRequest | 

    try:
        # Simulate a Gimtel transfer (sandbox)
        api_response = api_instance.post_checkout_session_public_by_id_simulate_transfer(id, post_checkout_session_public_by_id_simulate_transfer_request)
        print("The response of CheckoutSessionApi->post_checkout_session_public_by_id_simulate_transfer:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CheckoutSessionApi->post_checkout_session_public_by_id_simulate_transfer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **post_checkout_session_public_by_id_simulate_transfer_request** | [**PostCheckoutSessionPublicByIdSimulateTransferRequest**](PostCheckoutSessionPublicByIdSimulateTransferRequest.md)|  | 

### Return type

[**GetCheckoutSessionPublicByIdPaymentStatus200Response**](GetCheckoutSessionPublicByIdPaymentStatus200Response.md)

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

