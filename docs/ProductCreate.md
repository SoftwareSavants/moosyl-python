# ProductCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | [optional] 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**active** | **bool** |  | [optional] 
**created_at** | **datetime** |  | [optional] 

## Example

```python
from moosyl.models.product_create import ProductCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ProductCreate from a JSON string
product_create_instance = ProductCreate.from_json(json)
# print the JSON string representation of the object
print(ProductCreate.to_json())

# convert the object into a dict
product_create_dict = product_create_instance.to_dict()
# create an instance of ProductCreate from a dict
product_create_from_dict = ProductCreate.from_dict(product_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


