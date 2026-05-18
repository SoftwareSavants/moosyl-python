# moosyl.OrganizationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_organization_by_id**](OrganizationApi.md#get_organization_by_id) | **GET** /organization/{id} | Get organization details


# **get_organization_by_id**
> GetOrganizationById200Response get_organization_by_id(id)

Get organization details

Retrieve organization information. Requires secret API key.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.get_organization_by_id200_response import GetOrganizationById200Response
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
    api_instance = moosyl.OrganizationApi(api_client)
    id = 'id_example' # str | 

    try:
        # Get organization details
        api_response = api_instance.get_organization_by_id(id)
        print("The response of OrganizationApi->get_organization_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganizationApi->get_organization_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**GetOrganizationById200Response**](GetOrganizationById200Response.md)

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

