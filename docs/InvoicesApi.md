# moosyl.InvoicesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_invoices**](InvoicesApi.md#get_invoices) | **GET** /invoices/ | List invoices or filter by id/external user


# **get_invoices**
> InvoiceList get_invoices(id=id, external_user_id=external_user_id, subscription_id=subscription_id, page=page, limit=limit)

List invoices or filter by id/external user

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.invoice_list import InvoiceList
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
    api_instance = moosyl.InvoicesApi(api_client)
    id = 'id_example' # str |  (optional)
    external_user_id = 'external_user_id_example' # str |  (optional)
    subscription_id = 'subscription_id_example' # str |  (optional)
    page = moosyl.GetProductsPageParameter() # GetProductsPageParameter |  (optional)
    limit = moosyl.GetProductsPageParameter() # GetProductsPageParameter |  (optional)

    try:
        # List invoices or filter by id/external user
        api_response = api_instance.get_invoices(id=id, external_user_id=external_user_id, subscription_id=subscription_id, page=page, limit=limit)
        print("The response of InvoicesApi->get_invoices:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->get_invoices: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | [optional] 
 **external_user_id** | **str**|  | [optional] 
 **subscription_id** | **str**|  | [optional] 
 **page** | [**GetProductsPageParameter**](.md)|  | [optional] 
 **limit** | [**GetProductsPageParameter**](.md)|  | [optional] 

### Return type

[**InvoiceList**](InvoiceList.md)

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

