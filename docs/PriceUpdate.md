# PriceUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | [**PriceUpdateAmount**](PriceUpdateAmount.md) |  | [optional] 
**interval** | **str** |  | [optional] 
**replace_existing** | **bool** |  | [optional] 

## Example

```python
from moosyl.models.price_update import PriceUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of PriceUpdate from a JSON string
price_update_instance = PriceUpdate.from_json(json)
# print the JSON string representation of the object
print(PriceUpdate.to_json())

# convert the object into a dict
price_update_dict = price_update_instance.to_dict()
# create an instance of PriceUpdate from a dict
price_update_from_dict = PriceUpdate.from_dict(price_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


