# PaymentGetData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**amount** | **int** |  | 
**phone_number** | **str** |  | 
**pass_code** | **str** |  | 
**status** | **str** |  | 
**environment_id** | **UUID** |  | 
**payment_request_id** | **UUID** |  | 
**configuration_id** | **UUID** |  | 
**reference_id** | **str** |  | 
**metadata** | **object** |  | 
**payout_id** | **UUID** |  | 
**completed_at** | **datetime** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 

## Example

```python
from moosyl.models.payment_get_data import PaymentGetData

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentGetData from a JSON string
payment_get_data_instance = PaymentGetData.from_json(json)
# print the JSON string representation of the object
print(PaymentGetData.to_json())

# convert the object into a dict
payment_get_data_dict = payment_get_data_instance.to_dict()
# create an instance of PaymentGetData from a dict
payment_get_data_from_dict = PaymentGetData.from_dict(payment_get_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


