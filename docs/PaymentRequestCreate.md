# PaymentRequestCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**phone_number** | **str** |  | [optional] 
**transaction_id** | **str** |  | 
**amount** | [**GetProductsPageParameter**](GetProductsPageParameter.md) |  | 

## Example

```python
from moosyl.models.payment_request_create import PaymentRequestCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentRequestCreate from a JSON string
payment_request_create_instance = PaymentRequestCreate.from_json(json)
# print the JSON string representation of the object
print(PaymentRequestCreate.to_json())

# convert the object into a dict
payment_request_create_dict = payment_request_create_instance.to_dict()
# create an instance of PaymentRequestCreate from a dict
payment_request_create_from_dict = PaymentRequestCreate.from_dict(payment_request_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


