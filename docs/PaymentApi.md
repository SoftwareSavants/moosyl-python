# moosyl.PaymentApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_payment_by_id**](PaymentApi.md#get_payment_by_id) | **GET** /payment/{id} | Get payment details
[**get_payment_by_id_status**](PaymentApi.md#get_payment_by_id_status) | **GET** /payment/{id}/status | Get payment status (heartbeat)
[**post_payment**](PaymentApi.md#post_payment) | **POST** /payment | Create a new payment
[**post_payment_by_id_simulate_transfer**](PaymentApi.md#post_payment_by_id_simulate_transfer) | **POST** /payment/{id}/simulate-transfer | Simulate a Gimtel transfer (sandbox)


# **get_payment_by_id**
> PaymentGet get_payment_by_id(id)

Get payment details

Retrieve detailed information about a payment by transaction ID. Requires secret API key.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.payment_get import PaymentGet
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
    api_instance = moosyl.PaymentApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get payment details
        api_response = api_instance.get_payment_by_id(id)
        print("The response of PaymentApi->get_payment_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->get_payment_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**PaymentGet**](PaymentGet.md)

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

# **get_payment_by_id_status**
> GetPaymentByIdStatus200Response get_payment_by_id_status(id)

Get payment status (heartbeat)

Returns the payment's status. For Gimtel payments, poll this every few seconds while the payer is on the payment screen: the payment stops being claimable about 10 minutes after the last poll.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.get_payment_by_id_status200_response import GetPaymentByIdStatus200Response
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
    api_instance = moosyl.PaymentApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get payment status (heartbeat)
        api_response = api_instance.get_payment_by_id_status(id)
        print("The response of PaymentApi->get_payment_by_id_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->get_payment_by_id_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**GetPaymentByIdStatus200Response**](GetPaymentByIdStatus200Response.md)

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

# **post_payment**
> PostPayment200Response post_payment(payment_create)

Create a new payment

Use this endpoint to create a new payment for an existing payment request.

**Testing (Sandbox Environment Only) — native methods only**

The magic phone numbers below only apply to native payment methods (e.g. Sedad,
NexConnect, native Bankily). They do not apply to Gimtel methods — see below.

| Phone Number | Status     |
|--------------|------------|
| 22222222     | Accepted   |
| 33333333     | Accepted   |
| 44444444     | Accepted   |
| Other        | Rejected   |

**Gimtel methods (Bankily via Gimtel, BCI Pay, Amanty)**

The payment is created as `pending` and the response includes `instructions`
(receiving phone, exact amount). The payer transfers from the phone number you
sent. Poll `GET /payment/{paymentId}/status` every few seconds while the payer
is on the payment screen — the payment stops being claimable about 10 minutes
after the last poll. Completion also fires the `payment-updated` webhook.

In sandbox, Gimtel methods are never completed by a magic phone number: call
`POST /payment/{paymentId}/simulate-transfer` instead to simulate the payer's
bank transfer and complete the payment.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.payment_create import PaymentCreate
from moosyl.models.post_payment200_response import PostPayment200Response
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
    api_instance = moosyl.PaymentApi(api_client)
    payment_create = moosyl.PaymentCreate() # PaymentCreate | 

    try:
        # Create a new payment
        api_response = api_instance.post_payment(payment_create)
        print("The response of PaymentApi->post_payment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->post_payment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payment_create** | [**PaymentCreate**](PaymentCreate.md)|  | 

### Return type

[**PostPayment200Response**](PostPayment200Response.md)

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

# **post_payment_by_id_simulate_transfer**
> PostPaymentByIdSimulateTransfer200Response post_payment_by_id_simulate_transfer(id)

Simulate a Gimtel transfer (sandbox)

Sandbox only. Completes a pending Gimtel payment as if the payer had transferred the exact amount.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.post_payment_by_id_simulate_transfer200_response import PostPaymentByIdSimulateTransfer200Response
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
    api_instance = moosyl.PaymentApi(api_client)
    id = 'id_example' # str | 

    try:
        # Simulate a Gimtel transfer (sandbox)
        api_response = api_instance.post_payment_by_id_simulate_transfer(id)
        print("The response of PaymentApi->post_payment_by_id_simulate_transfer:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->post_payment_by_id_simulate_transfer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**PostPaymentByIdSimulateTransfer200Response**](PostPaymentByIdSimulateTransfer200Response.md)

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

