# ConfigurationListDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**type** | **str** |  | 
**organization_id** | **UUID** |  | 
**config** | **object** |  | 
**is_testing_mode** | **bool** |  | 

## Example

```python
from moosyl.models.configuration_list_data_inner import ConfigurationListDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigurationListDataInner from a JSON string
configuration_list_data_inner_instance = ConfigurationListDataInner.from_json(json)
# print the JSON string representation of the object
print(ConfigurationListDataInner.to_json())

# convert the object into a dict
configuration_list_data_inner_dict = configuration_list_data_inner_instance.to_dict()
# create an instance of ConfigurationListDataInner from a dict
configuration_list_data_inner_from_dict = ConfigurationListDataInner.from_dict(configuration_list_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


