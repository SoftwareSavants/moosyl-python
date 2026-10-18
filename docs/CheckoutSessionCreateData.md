# CheckoutSessionCreateData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**payment_request_id** | **UUID** |  | 
**environment_id** | **UUID** |  | 
**selected_configuration_id** | **UUID** |  | 
**status** | **str** |  | 
**success_url** | **str** |  | 
**cancel_url** | **str** |  | 
**expires_at** | **datetime** |  | 
**completed_at** | **datetime** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 

## Example

```python
from moosyl.models.checkout_session_create_data import CheckoutSessionCreateData

# TODO update the JSON string below
json = "{}"
# create an instance of CheckoutSessionCreateData from a JSON string
checkout_session_create_data_instance = CheckoutSessionCreateData.from_json(json)
# print the JSON string representation of the object
print(CheckoutSessionCreateData.to_json())

# convert the object into a dict
checkout_session_create_data_dict = checkout_session_create_data_instance.to_dict()
# create an instance of CheckoutSessionCreateData from a dict
checkout_session_create_data_from_dict = CheckoutSessionCreateData.from_dict(checkout_session_create_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


