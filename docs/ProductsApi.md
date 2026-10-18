# moosyl.ProductsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_products**](ProductsApi.md#get_products) | **GET** /products/ | List products or filter by id
[**get_products_by_id**](ProductsApi.md#get_products_by_id) | **GET** /products/{id} | Get product with prices
[**patch_products_by_id**](ProductsApi.md#patch_products_by_id) | **PATCH** /products/{id} | Update product
[**patch_products_by_id_archive**](ProductsApi.md#patch_products_by_id_archive) | **PATCH** /products/{id}/archive | Archive product
[**post_products**](ProductsApi.md#post_products) | **POST** /products/ | Create product


# **get_products**
> ProductList get_products(id=id, page=page, limit=limit)

List products or filter by id

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.product_list import ProductList
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
    api_instance = moosyl.ProductsApi(api_client)
    id = 'id_example' # str |  (optional)
    page = moosyl.GetProductsPageParameter() # GetProductsPageParameter |  (optional)
    limit = moosyl.GetProductsPageParameter() # GetProductsPageParameter |  (optional)

    try:
        # List products or filter by id
        api_response = api_instance.get_products(id=id, page=page, limit=limit)
        print("The response of ProductsApi->get_products:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductsApi->get_products: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | [optional] 
 **page** | [**GetProductsPageParameter**](.md)|  | [optional] 
 **limit** | [**GetProductsPageParameter**](.md)|  | [optional] 

### Return type

[**ProductList**](ProductList.md)

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

# **get_products_by_id**
> ProductGetWithPrices get_products_by_id(id)

Get product with prices

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.product_get_with_prices import ProductGetWithPrices
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
    api_instance = moosyl.ProductsApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get product with prices
        api_response = api_instance.get_products_by_id(id)
        print("The response of ProductsApi->get_products_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductsApi->get_products_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**ProductGetWithPrices**](ProductGetWithPrices.md)

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

# **patch_products_by_id**
> ProductGet patch_products_by_id(id, product_update)

Update product

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.product_get import ProductGet
from moosyl.models.product_update import ProductUpdate
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
    api_instance = moosyl.ProductsApi(api_client)
    id = 'id_example' # str | 
    product_update = moosyl.ProductUpdate() # ProductUpdate | 

    try:
        # Update product
        api_response = api_instance.patch_products_by_id(id, product_update)
        print("The response of ProductsApi->patch_products_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductsApi->patch_products_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **product_update** | [**ProductUpdate**](ProductUpdate.md)|  | 

### Return type

[**ProductGet**](ProductGet.md)

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

# **patch_products_by_id_archive**
> Success patch_products_by_id_archive(id)

Archive product

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
    api_instance = moosyl.ProductsApi(api_client)
    id = 'id_example' # str | 

    try:
        # Archive product
        api_response = api_instance.patch_products_by_id_archive(id)
        print("The response of ProductsApi->patch_products_by_id_archive:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductsApi->patch_products_by_id_archive: %s\n" % e)
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

# **post_products**
> ProductGet post_products(product_create)

Create product

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.product_create import ProductCreate
from moosyl.models.product_get import ProductGet
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
    api_instance = moosyl.ProductsApi(api_client)
    product_create = moosyl.ProductCreate() # ProductCreate | 

    try:
        # Create product
        api_response = api_instance.post_products(product_create)
        print("The response of ProductsApi->post_products:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductsApi->post_products: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_create** | [**ProductCreate**](ProductCreate.md)|  | 

### Return type

[**ProductGet**](ProductGet.md)

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

