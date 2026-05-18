# ProductListPagination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **float** |  | 
**limit** | **float** |  | 
**total** | **float** |  | 
**total_pages** | **float** |  | 

## Example

```python
from moosyl.models.product_list_pagination import ProductListPagination

# TODO update the JSON string below
json = "{}"
# create an instance of ProductListPagination from a JSON string
product_list_pagination_instance = ProductListPagination.from_json(json)
# print the JSON string representation of the object
print(ProductListPagination.to_json())

# convert the object into a dict
product_list_pagination_dict = product_list_pagination_instance.to_dict()
# create an instance of ProductListPagination from a dict
product_list_pagination_from_dict = ProductListPagination.from_dict(product_list_pagination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


