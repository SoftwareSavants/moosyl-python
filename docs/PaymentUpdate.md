# PaymentUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**amount** | **float** |  | [optional] 

## Example

```python
from moosyl.models.payment_update import PaymentUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentUpdate from a JSON string
payment_update_instance = PaymentUpdate.from_json(json)
# print the JSON string representation of the object
print(PaymentUpdate.to_json())

# convert the object into a dict
payment_update_dict = payment_update_instance.to_dict()
# create an instance of PaymentUpdate from a dict
payment_update_from_dict = PaymentUpdate.from_dict(payment_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


