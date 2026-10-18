# moosyl.CustomersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_customers**](CustomersApi.md#get_customers) | **GET** /customers/ | List customers or filter by id/external user
[**patch_customers_by_id**](CustomersApi.md#patch_customers_by_id) | **PATCH** /customers/{id} | Update customer
[**post_customers**](CustomersApi.md#post_customers) | **POST** /customers/ | Create customer


# **get_customers**
> CustomerList get_customers(id=id, external_user_id=external_user_id, page=page, limit=limit)

List customers or filter by id/external user

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.customer_list import CustomerList
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
    api_instance = moosyl.CustomersApi(api_client)
    id = 'id_example' # str |  (optional)
    external_user_id = 'external_user_id_example' # str |  (optional)
    page = moosyl.GetProductsPageParameter() # GetProductsPageParameter |  (optional)
    limit = moosyl.GetProductsPageParameter() # GetProductsPageParameter |  (optional)

    try:
        # List customers or filter by id/external user
        api_response = api_instance.get_customers(id=id, external_user_id=external_user_id, page=page, limit=limit)
        print("The response of CustomersApi->get_customers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomersApi->get_customers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | [optional] 
 **external_user_id** | **str**|  | [optional] 
 **page** | [**GetProductsPageParameter**](.md)|  | [optional] 
 **limit** | [**GetProductsPageParameter**](.md)|  | [optional] 

### Return type

[**CustomerList**](CustomerList.md)

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

# **patch_customers_by_id**
> CustomerGet patch_customers_by_id(id, customer_update)

Update customer

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.customer_get import CustomerGet
from moosyl.models.customer_update import CustomerUpdate
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
    api_instance = moosyl.CustomersApi(api_client)
    id = 'id_example' # str | 
    customer_update = moosyl.CustomerUpdate() # CustomerUpdate | 

    try:
        # Update customer
        api_response = api_instance.patch_customers_by_id(id, customer_update)
        print("The response of CustomersApi->patch_customers_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomersApi->patch_customers_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **customer_update** | [**CustomerUpdate**](CustomerUpdate.md)|  | 

### Return type

[**CustomerGet**](CustomerGet.md)

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

# **post_customers**
> CustomerGet post_customers(customer_create)

Create customer

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.customer_create import CustomerCreate
from moosyl.models.customer_get import CustomerGet
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
    api_instance = moosyl.CustomersApi(api_client)
    customer_create = moosyl.CustomerCreate() # CustomerCreate | 

    try:
        # Create customer
        api_response = api_instance.post_customers(customer_create)
        print("The response of CustomersApi->post_customers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomersApi->post_customers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_create** | [**CustomerCreate**](CustomerCreate.md)|  | 

### Return type

[**CustomerGet**](CustomerGet.md)

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

