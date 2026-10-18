# PaymentRequestGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PaymentRequestGetData**](PaymentRequestGetData.md) |  | 

## Example

```python
from moosyl.models.payment_request_get import PaymentRequestGet

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentRequestGet from a JSON string
payment_request_get_instance = PaymentRequestGet.from_json(json)
# print the JSON string representation of the object
print(PaymentRequestGet.to_json())

# convert the object into a dict
payment_request_get_dict = payment_request_get_instance.to_dict()
# create an instance of PaymentRequestGet from a dict
payment_request_get_from_dict = PaymentRequestGet.from_dict(payment_request_get_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


