# PostConnectExchange200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**publishable_key** | **str** |  | 
**secret_key** | **str** |  | 
**webhook_secret** | **str** |  | 

## Example

```python
from moosyl.models.post_connect_exchange200_response_data import PostConnectExchange200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of PostConnectExchange200ResponseData from a JSON string
post_connect_exchange200_response_data_instance = PostConnectExchange200ResponseData.from_json(json)
# print the JSON string representation of the object
print(PostConnectExchange200ResponseData.to_json())

# convert the object into a dict
post_connect_exchange200_response_data_dict = post_connect_exchange200_response_data_instance.to_dict()
# create an instance of PostConnectExchange200ResponseData from a dict
post_connect_exchange200_response_data_from_dict = PostConnectExchange200ResponseData.from_dict(post_connect_exchange200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


