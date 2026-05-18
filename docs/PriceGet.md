# PriceGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ProductGetWithPricesDataPricesInner**](ProductGetWithPricesDataPricesInner.md) |  | 

## Example

```python
from moosyl.models.price_get import PriceGet

# TODO update the JSON string below
json = "{}"
# create an instance of PriceGet from a JSON string
price_get_instance = PriceGet.from_json(json)
# print the JSON string representation of the object
print(PriceGet.to_json())

# convert the object into a dict
price_get_dict = price_get_instance.to_dict()
# create an instance of PriceGet from a dict
price_get_from_dict = PriceGet.from_dict(price_get_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


