# ProductGetWithPricesDataPricesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**product_id** | **UUID** |  | 
**amount** | **int** |  | 
**interval** | **str** |  | 
**active** | **bool** |  | 
**created_at** | **datetime** |  | 

## Example

```python
from moosyl.models.product_get_with_prices_data_prices_inner import ProductGetWithPricesDataPricesInner

# TODO update the JSON string below
json = "{}"
# create an instance of ProductGetWithPricesDataPricesInner from a JSON string
product_get_with_prices_data_prices_inner_instance = ProductGetWithPricesDataPricesInner.from_json(json)
# print the JSON string representation of the object
print(ProductGetWithPricesDataPricesInner.to_json())

# convert the object into a dict
product_get_with_prices_data_prices_inner_dict = product_get_with_prices_data_prices_inner_instance.to_dict()
# create an instance of ProductGetWithPricesDataPricesInner from a dict
product_get_with_prices_data_prices_inner_from_dict = ProductGetWithPricesDataPricesInner.from_dict(product_get_with_prices_data_prices_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


