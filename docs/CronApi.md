# moosyl.CronApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**post_cron_billing_cycle**](CronApi.md#post_cron_billing_cycle) | **POST** /cron/billing-cycle | Process billing cycles
[**post_cron_expire_subscriptions**](CronApi.md#post_cron_expire_subscriptions) | **POST** /cron/expire-subscriptions | Process due cancellations and expirations


# **post_cron_billing_cycle**
> CronResult post_cron_billing_cycle()

Process billing cycles

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.cron_result import CronResult
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
    api_instance = moosyl.CronApi(api_client)

    try:
        # Process billing cycles
        api_response = api_instance.post_cron_billing_cycle()
        print("The response of CronApi->post_cron_billing_cycle:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CronApi->post_cron_billing_cycle: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CronResult**](CronResult.md)

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

# **post_cron_expire_subscriptions**
> CronResult post_cron_expire_subscriptions()

Process due cancellations and expirations

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.cron_result import CronResult
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
    api_instance = moosyl.CronApi(api_client)

    try:
        # Process due cancellations and expirations
        api_response = api_instance.post_cron_expire_subscriptions()
        print("The response of CronApi->post_cron_expire_subscriptions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CronApi->post_cron_expire_subscriptions: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CronResult**](CronResult.md)

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

