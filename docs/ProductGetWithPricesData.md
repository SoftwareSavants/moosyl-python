# ProductGetWithPricesData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**organization_id** | **UUID** |  | 
**environment_id** | **UUID** |  | 
**name** | **str** |  | 
**description** | **str** |  | 
**active** | **bool** |  | 
**created_at** | **datetime** |  | 
**prices** | [**List[ProductGetWithPricesDataPricesInner]**](ProductGetWithPricesDataPricesInner.md) |  | 

## Example

```python
from moosyl.models.product_get_with_prices_data import ProductGetWithPricesData

# TODO update the JSON string below
json = "{}"
# create an instance of ProductGetWithPricesData from a JSON string
product_get_with_prices_data_instance = ProductGetWithPricesData.from_json(json)
# print the JSON string representation of the object
print(ProductGetWithPricesData.to_json())

# convert the object into a dict
product_get_with_prices_data_dict = product_get_with_prices_data_instance.to_dict()
# create an instance of ProductGetWithPricesData from a dict
product_get_with_prices_data_from_dict = ProductGetWithPricesData.from_dict(product_get_with_prices_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


