# moosyl.SubscriptionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_subscriptions**](SubscriptionsApi.md#get_subscriptions) | **GET** /subscriptions/ | List subscriptions
[**get_subscriptions_by_external_user_by_external_user_id**](SubscriptionsApi.md#get_subscriptions_by_external_user_by_external_user_id) | **GET** /subscriptions/by-external-user/{externalUserId} | Get subscription by external user
[**get_subscriptions_by_id**](SubscriptionsApi.md#get_subscriptions_by_id) | **GET** /subscriptions/{id} | Get subscription
[**post_subscriptions**](SubscriptionsApi.md#post_subscriptions) | **POST** /subscriptions/ | Create subscription
[**post_subscriptions_by_external_user**](SubscriptionsApi.md#post_subscriptions_by_external_user) | **POST** /subscriptions/by-external-user | Create subscription by external user
[**post_subscriptions_by_id_cancel**](SubscriptionsApi.md#post_subscriptions_by_id_cancel) | **POST** /subscriptions/{id}/cancel | Cancel subscription


# **get_subscriptions**
> SubscriptionList get_subscriptions(status=status, page=page, limit=limit)

List subscriptions

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.subscription_list import SubscriptionList
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
    api_instance = moosyl.SubscriptionsApi(api_client)
    status = 'status_example' # str |  (optional)
    page = moosyl.GetProductsPageParameter() # GetProductsPageParameter |  (optional)
    limit = moosyl.GetProductsPageParameter() # GetProductsPageParameter |  (optional)

    try:
        # List subscriptions
        api_response = api_instance.get_subscriptions(status=status, page=page, limit=limit)
        print("The response of SubscriptionsApi->get_subscriptions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->get_subscriptions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **str**|  | [optional] 
 **page** | [**GetProductsPageParameter**](.md)|  | [optional] 
 **limit** | [**GetProductsPageParameter**](.md)|  | [optional] 

### Return type

[**SubscriptionList**](SubscriptionList.md)

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

# **get_subscriptions_by_external_user_by_external_user_id**
> SubscriptionGet get_subscriptions_by_external_user_by_external_user_id(external_user_id)

Get subscription by external user

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.subscription_get import SubscriptionGet
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
    api_instance = moosyl.SubscriptionsApi(api_client)
    external_user_id = 'external_user_id_example' # str | 

    try:
        # Get subscription by external user
        api_response = api_instance.get_subscriptions_by_external_user_by_external_user_id(external_user_id)
        print("The response of SubscriptionsApi->get_subscriptions_by_external_user_by_external_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->get_subscriptions_by_external_user_by_external_user_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **external_user_id** | **str**|  | 

### Return type

[**SubscriptionGet**](SubscriptionGet.md)

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

# **get_subscriptions_by_id**
> SubscriptionGet get_subscriptions_by_id(id)

Get subscription

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.subscription_get import SubscriptionGet
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
    api_instance = moosyl.SubscriptionsApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get subscription
        api_response = api_instance.get_subscriptions_by_id(id)
        print("The response of SubscriptionsApi->get_subscriptions_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->get_subscriptions_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**SubscriptionGet**](SubscriptionGet.md)

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

# **post_subscriptions**
> SubscriptionGet post_subscriptions(subscription_create)

Create subscription

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.subscription_create import SubscriptionCreate
from moosyl.models.subscription_get import SubscriptionGet
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
    api_instance = moosyl.SubscriptionsApi(api_client)
    subscription_create = moosyl.SubscriptionCreate() # SubscriptionCreate | 

    try:
        # Create subscription
        api_response = api_instance.post_subscriptions(subscription_create)
        print("The response of SubscriptionsApi->post_subscriptions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->post_subscriptions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_create** | [**SubscriptionCreate**](SubscriptionCreate.md)|  | 

### Return type

[**SubscriptionGet**](SubscriptionGet.md)

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

# **post_subscriptions_by_external_user**
> SubscriptionGet post_subscriptions_by_external_user(subscription_create_by_external_user)

Create subscription by external user

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.subscription_create_by_external_user import SubscriptionCreateByExternalUser
from moosyl.models.subscription_get import SubscriptionGet
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
    api_instance = moosyl.SubscriptionsApi(api_client)
    subscription_create_by_external_user = moosyl.SubscriptionCreateByExternalUser() # SubscriptionCreateByExternalUser | 

    try:
        # Create subscription by external user
        api_response = api_instance.post_subscriptions_by_external_user(subscription_create_by_external_user)
        print("The response of SubscriptionsApi->post_subscriptions_by_external_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->post_subscriptions_by_external_user: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_create_by_external_user** | [**SubscriptionCreateByExternalUser**](SubscriptionCreateByExternalUser.md)|  | 

### Return type

[**SubscriptionGet**](SubscriptionGet.md)

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

# **post_subscriptions_by_id_cancel**
> SubscriptionGet post_subscriptions_by_id_cancel(id)

Cancel subscription

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.subscription_get import SubscriptionGet
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
    api_instance = moosyl.SubscriptionsApi(api_client)
    id = 'id_example' # str | 

    try:
        # Cancel subscription
        api_response = api_instance.post_subscriptions_by_id_cancel(id)
        print("The response of SubscriptionsApi->post_subscriptions_by_id_cancel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->post_subscriptions_by_id_cancel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**SubscriptionGet**](SubscriptionGet.md)

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

