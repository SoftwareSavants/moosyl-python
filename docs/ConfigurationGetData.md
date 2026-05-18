# ConfigurationGetData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**type** | **str** |  | 
**organization_id** | **UUID** |  | 
**config** | **object** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 
**is_testing_mode** | **bool** |  | 

## Example

```python
from moosyl.models.configuration_get_data import ConfigurationGetData

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigurationGetData from a JSON string
configuration_get_data_instance = ConfigurationGetData.from_json(json)
# print the JSON string representation of the object
print(ConfigurationGetData.to_json())

# convert the object into a dict
configuration_get_data_dict = configuration_get_data_instance.to_dict()
# create an instance of ConfigurationGetData from a dict
configuration_get_data_from_dict = ConfigurationGetData.from_dict(configuration_get_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


