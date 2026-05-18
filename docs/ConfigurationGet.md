# ConfigurationGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ConfigurationGetData**](ConfigurationGetData.md) |  | 

## Example

```python
from moosyl.models.configuration_get import ConfigurationGet

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigurationGet from a JSON string
configuration_get_instance = ConfigurationGet.from_json(json)
# print the JSON string representation of the object
print(ConfigurationGet.to_json())

# convert the object into a dict
configuration_get_dict = configuration_get_instance.to_dict()
# create an instance of ConfigurationGet from a dict
configuration_get_from_dict = ConfigurationGet.from_dict(configuration_get_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


