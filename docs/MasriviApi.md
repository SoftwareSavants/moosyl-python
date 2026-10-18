# moosyl.MasriviApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**post_masrivi_initiate**](MasriviApi.md#post_masrivi_initiate) | **POST** /masrivi/initiate | Initiate Masrivi payment


# **post_masrivi_initiate**
> PostMasriviInitiate200Response post_masrivi_initiate(post_masrivi_initiate_request)

Initiate Masrivi payment

Creates a pending payment and returns form data to redirect customer to Masrivi payment page.

### Example

* Api Key Authentication (ApiKey):

```python
import moosyl
from moosyl.models.post_masrivi_initiate200_response import PostMasriviInitiate200Response
from moosyl.models.post_masrivi_initiate_request import PostMasriviInitiateRequest
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
    api_instance = moosyl.MasriviApi(api_client)
    post_masrivi_initiate_request = moosyl.PostMasriviInitiateRequest() # PostMasriviInitiateRequest | 

    try:
        # Initiate Masrivi payment
        api_response = api_instance.post_masrivi_initiate(post_masrivi_initiate_request)
        print("The response of MasriviApi->post_masrivi_initiate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MasriviApi->post_masrivi_initiate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_masrivi_initiate_request** | [**PostMasriviInitiateRequest**](PostMasriviInitiateRequest.md)|  | 

### Return type

[**PostMasriviInitiate200Response**](PostMasriviInitiate200Response.md)

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

