# GetOrganizationById200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**phone_number** | **str** |  | 
**website** | **str** |  | 

## Example

```python
from moosyl.models.get_organization_by_id200_response_data import GetOrganizationById200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrganizationById200ResponseData from a JSON string
get_organization_by_id200_response_data_instance = GetOrganizationById200ResponseData.from_json(json)
# print the JSON string representation of the object
print(GetOrganizationById200ResponseData.to_json())

# convert the object into a dict
get_organization_by_id200_response_data_dict = get_organization_by_id200_response_data_instance.to_dict()
# create an instance of GetOrganizationById200ResponseData from a dict
get_organization_by_id200_response_data_from_dict = GetOrganizationById200ResponseData.from_dict(get_organization_by_id200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


