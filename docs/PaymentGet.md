# PaymentGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PaymentGetData**](PaymentGetData.md) |  | 

## Example

```python
from moosyl.models.payment_get import PaymentGet

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentGet from a JSON string
payment_get_instance = PaymentGet.from_json(json)
# print the JSON string representation of the object
print(PaymentGet.to_json())

# convert the object into a dict
payment_get_dict = payment_get_instance.to_dict()
# create an instance of PaymentGet from a dict
payment_get_from_dict = PaymentGet.from_dict(payment_get_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


