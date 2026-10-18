# PostMasriviInitiateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**transaction_id** | **str** |  | 
**configuration_id** | **str** |  | 
**phone_number** | **str** |  | [optional] 
**accept_url** | **str** |  | [optional] 
**decline_url** | **str** |  | [optional] 
**cancel_url** | **str** |  | [optional] 

## Example

```python
from moosyl.models.post_masrivi_initiate_request import PostMasriviInitiateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PostMasriviInitiateRequest from a JSON string
post_masrivi_initiate_request_instance = PostMasriviInitiateRequest.from_json(json)
# print the JSON string representation of the object
print(PostMasriviInitiateRequest.to_json())

# convert the object into a dict
post_masrivi_initiate_request_dict = post_masrivi_initiate_request_instance.to_dict()
# create an instance of PostMasriviInitiateRequest from a dict
post_masrivi_initiate_request_from_dict = PostMasriviInitiateRequest.from_dict(post_masrivi_initiate_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


