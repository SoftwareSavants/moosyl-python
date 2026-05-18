# PaymentRequestGetData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**amount** | **int** |  | 
**total_amount** | **int** |  | 
**phone_number** | **str** |  | 
**transaction_id** | **str** |  | 
**environment_id** | **UUID** |  | 
**retry_count** | **int** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 

## Example

```python
from moosyl.models.payment_request_get_data import PaymentRequestGetData

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentRequestGetData from a JSON string
payment_request_get_data_instance = PaymentRequestGetData.from_json(json)
# print the JSON string representation of the object
print(PaymentRequestGetData.to_json())

# convert the object into a dict
payment_request_get_data_dict = payment_request_get_data_instance.to_dict()
# create an instance of PaymentRequestGetData from a dict
payment_request_get_data_from_dict = PaymentRequestGetData.from_dict(payment_request_get_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


