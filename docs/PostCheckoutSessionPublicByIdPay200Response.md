# PostCheckoutSessionPublicByIdPay200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 
**reference_id** | **str** |  | [optional] 
**payment_code** | **str** |  | [optional] 
**success_url** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 
**form_data** | **object** |  | [optional] 

## Example

```python
from moosyl.models.post_checkout_session_public_by_id_pay200_response import PostCheckoutSessionPublicByIdPay200Response

# TODO update the JSON string below
json = "{}"
# create an instance of PostCheckoutSessionPublicByIdPay200Response from a JSON string
post_checkout_session_public_by_id_pay200_response_instance = PostCheckoutSessionPublicByIdPay200Response.from_json(json)
# print the JSON string representation of the object
print(PostCheckoutSessionPublicByIdPay200Response.to_json())

# convert the object into a dict
post_checkout_session_public_by_id_pay200_response_dict = post_checkout_session_public_by_id_pay200_response_instance.to_dict()
# create an instance of PostCheckoutSessionPublicByIdPay200Response from a dict
post_checkout_session_public_by_id_pay200_response_from_dict = PostCheckoutSessionPublicByIdPay200Response.from_dict(post_checkout_session_public_by_id_pay200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


