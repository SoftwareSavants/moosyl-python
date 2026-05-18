# PostConnectExchangeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform_id** | **str** |  | 
**platform_secret** | **str** |  | 
**code** | **str** |  | 
**webhook_payment_created_endpoint** | **str** |  | 
**webhook_payment_updated_endpoint** | **str** |  | 

## Example

```python
from moosyl.models.post_connect_exchange_request import PostConnectExchangeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PostConnectExchangeRequest from a JSON string
post_connect_exchange_request_instance = PostConnectExchangeRequest.from_json(json)
# print the JSON string representation of the object
print(PostConnectExchangeRequest.to_json())

# convert the object into a dict
post_connect_exchange_request_dict = post_connect_exchange_request_instance.to_dict()
# create an instance of PostConnectExchangeRequest from a dict
post_connect_exchange_request_from_dict = PostConnectExchangeRequest.from_dict(post_connect_exchange_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


