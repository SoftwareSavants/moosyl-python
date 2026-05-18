# PaymentCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**configuration_id** | **UUID** |  | 
**transaction_id** | **str** |  | 
**phone_number** | **str** |  | 
**pass_code** | **str** |  | 

## Example

```python
from moosyl.models.payment_create import PaymentCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentCreate from a JSON string
payment_create_instance = PaymentCreate.from_json(json)
# print the JSON string representation of the object
print(PaymentCreate.to_json())

# convert the object into a dict
payment_create_dict = payment_create_instance.to_dict()
# create an instance of PaymentCreate from a dict
payment_create_from_dict = PaymentCreate.from_dict(payment_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


