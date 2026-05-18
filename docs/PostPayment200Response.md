# PostPayment200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**status** | **str** |  | 
**reference_id** | **str** |  | 
**metadata** | **object** |  | [optional] 

## Example

```python
from moosyl.models.post_payment200_response import PostPayment200Response

# TODO update the JSON string below
json = "{}"
# create an instance of PostPayment200Response from a JSON string
post_payment200_response_instance = PostPayment200Response.from_json(json)
# print the JSON string representation of the object
print(PostPayment200Response.to_json())

# convert the object into a dict
post_payment200_response_dict = post_payment200_response_instance.to_dict()
# create an instance of PostPayment200Response from a dict
post_payment200_response_from_dict = PostPayment200Response.from_dict(post_payment200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


