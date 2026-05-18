# CheckoutSessionGetLatestPayment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**amount** | **float** |  | 
**status** | **str** |  | 
**reference_id** | **str** |  | 
**payment_code** | **str** |  | [optional] 

## Example

```python
from moosyl.models.checkout_session_get_latest_payment import CheckoutSessionGetLatestPayment

# TODO update the JSON string below
json = "{}"
# create an instance of CheckoutSessionGetLatestPayment from a JSON string
checkout_session_get_latest_payment_instance = CheckoutSessionGetLatestPayment.from_json(json)
# print the JSON string representation of the object
print(CheckoutSessionGetLatestPayment.to_json())

# convert the object into a dict
checkout_session_get_latest_payment_dict = checkout_session_get_latest_payment_instance.to_dict()
# create an instance of CheckoutSessionGetLatestPayment from a dict
checkout_session_get_latest_payment_from_dict = CheckoutSessionGetLatestPayment.from_dict(checkout_session_get_latest_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


