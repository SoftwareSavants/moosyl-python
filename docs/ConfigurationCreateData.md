# ConfigurationCreateData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**config** | **object** |  | 
**organization_id** | **UUID** |  | [optional] 
**is_testing_mode** | **bool** |  | [optional] 

## Example

```python
from moosyl.models.configuration_create_data import ConfigurationCreateData

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigurationCreateData from a JSON string
configuration_create_data_instance = ConfigurationCreateData.from_json(json)
# print the JSON string representation of the object
print(ConfigurationCreateData.to_json())

# convert the object into a dict
configuration_create_data_dict = configuration_create_data_instance.to_dict()
# create an instance of ConfigurationCreateData from a dict
configuration_create_data_from_dict = ConfigurationCreateData.from_dict(configuration_create_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


