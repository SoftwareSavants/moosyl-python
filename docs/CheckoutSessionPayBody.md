# CheckoutSessionPayBody


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**configuration_id** | **str** |  | 
**phone_number** | **str** |  | [optional] 
**pass_code** | **str** |  | [optional] 

## Example

```python
from moosyl.models.checkout_session_pay_body import CheckoutSessionPayBody

# TODO update the JSON string below
json = "{}"
# create an instance of CheckoutSessionPayBody from a JSON string
checkout_session_pay_body_instance = CheckoutSessionPayBody.from_json(json)
# print the JSON string representation of the object
print(CheckoutSessionPayBody.to_json())

# convert the object into a dict
checkout_session_pay_body_dict = checkout_session_pay_body_instance.to_dict()
# create an instance of CheckoutSessionPayBody from a dict
checkout_session_pay_body_from_dict = CheckoutSessionPayBody.from_dict(checkout_session_pay_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


