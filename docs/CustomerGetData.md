# CustomerGetData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**organization_id** | **UUID** |  | 
**external_user_id** | **str** |  | 
**phone** | **str** |  | 
**created_at** | **datetime** |  | 

## Example

```python
from moosyl.models.customer_get_data import CustomerGetData

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerGetData from a JSON string
customer_get_data_instance = CustomerGetData.from_json(json)
# print the JSON string representation of the object
print(CustomerGetData.to_json())

# convert the object into a dict
customer_get_data_dict = customer_get_data_instance.to_dict()
# create an instance of CustomerGetData from a dict
customer_get_data_from_dict = CustomerGetData.from_dict(customer_get_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


