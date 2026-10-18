# PostConnectRevokeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform_id** | **str** |  | 
**platform_secret** | **str** |  | 
**connection_id** | **str** |  | 

## Example

```python
from moosyl.models.post_connect_revoke_request import PostConnectRevokeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PostConnectRevokeRequest from a JSON string
post_connect_revoke_request_instance = PostConnectRevokeRequest.from_json(json)
# print the JSON string representation of the object
print(PostConnectRevokeRequest.to_json())

# convert the object into a dict
post_connect_revoke_request_dict = post_connect_revoke_request_instance.to_dict()
# create an instance of PostConnectRevokeRequest from a dict
post_connect_revoke_request_from_dict = PostConnectRevokeRequest.from_dict(post_connect_revoke_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


