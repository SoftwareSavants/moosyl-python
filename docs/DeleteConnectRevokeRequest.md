# DeleteConnectRevokeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform_id** | **str** |  | 
**platform_secret** | **str** |  | 
**connection_id** | **str** |  | 

## Example

```python
from moosyl.models.delete_connect_revoke_request import DeleteConnectRevokeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteConnectRevokeRequest from a JSON string
delete_connect_revoke_request_instance = DeleteConnectRevokeRequest.from_json(json)
# print the JSON string representation of the object
print(DeleteConnectRevokeRequest.to_json())

# convert the object into a dict
delete_connect_revoke_request_dict = delete_connect_revoke_request_instance.to_dict()
# create an instance of DeleteConnectRevokeRequest from a dict
delete_connect_revoke_request_from_dict = DeleteConnectRevokeRequest.from_dict(delete_connect_revoke_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


