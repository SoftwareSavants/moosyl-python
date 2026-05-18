# CustomerGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CustomerGetData**](CustomerGetData.md) |  | 

## Example

```python
from moosyl.models.customer_get import CustomerGet

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerGet from a JSON string
customer_get_instance = CustomerGet.from_json(json)
# print the JSON string representation of the object
print(CustomerGet.to_json())

# convert the object into a dict
customer_get_dict = customer_get_instance.to_dict()
# create an instance of CustomerGet from a dict
customer_get_from_dict = CustomerGet.from_dict(customer_get_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


