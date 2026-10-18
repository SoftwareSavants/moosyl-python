# ConfigurationList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ConfigurationListDataInner]**](ConfigurationListDataInner.md) |  | 

## Example

```python
from moosyl.models.configuration_list import ConfigurationList

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigurationList from a JSON string
configuration_list_instance = ConfigurationList.from_json(json)
# print the JSON string representation of the object
print(ConfigurationList.to_json())

# convert the object into a dict
configuration_list_dict = configuration_list_instance.to_dict()
# create an instance of ConfigurationList from a dict
configuration_list_from_dict = ConfigurationList.from_dict(configuration_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


