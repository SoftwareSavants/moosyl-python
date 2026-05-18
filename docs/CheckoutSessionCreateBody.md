# CheckoutSessionCreateBody


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**payment_request_id** | **str** |  | [optional] 
**transaction_id** | **str** |  | [optional] 
**amount** | [**GetProductsPageParameter**](GetProductsPageParameter.md) |  | [optional] 
**phone_number** | **str** |  | [optional] 
**success_url** | **str** |  | [optional] 
**cancel_url** | **str** |  | [optional] 
**expires_in_minutes** | **float** |  | [optional] 

## Example

```python
from moosyl.models.checkout_session_create_body import CheckoutSessionCreateBody

# TODO update the JSON string below
json = "{}"
# create an instance of CheckoutSessionCreateBody from a JSON string
checkout_session_create_body_instance = CheckoutSessionCreateBody.from_json(json)
# print the JSON string representation of the object
print(CheckoutSessionCreateBody.to_json())

# convert the object into a dict
checkout_session_create_body_dict = checkout_session_create_body_instance.to_dict()
# create an instance of CheckoutSessionCreateBody from a dict
checkout_session_create_body_from_dict = CheckoutSessionCreateBody.from_dict(checkout_session_create_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


