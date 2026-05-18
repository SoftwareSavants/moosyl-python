# PriceCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | [optional] 
**product_id** | **UUID** |  | 
**amount** | **int** |  | 
**interval** | **str** |  | 
**active** | **bool** |  | [optional] 
**created_at** | **datetime** |  | [optional] 

## Example

```python
from moosyl.models.price_create import PriceCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PriceCreate from a JSON string
price_create_instance = PriceCreate.from_json(json)
# print the JSON string representation of the object
print(PriceCreate.to_json())

# convert the object into a dict
price_create_dict = price_create_instance.to_dict()
# create an instance of PriceCreate from a dict
price_create_from_dict = PriceCreate.from_dict(price_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


