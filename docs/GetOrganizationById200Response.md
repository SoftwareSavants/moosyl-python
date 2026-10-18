# GetOrganizationById200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GetOrganizationById200ResponseData**](GetOrganizationById200ResponseData.md) |  | 

## Example

```python
from moosyl.models.get_organization_by_id200_response import GetOrganizationById200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrganizationById200Response from a JSON string
get_organization_by_id200_response_instance = GetOrganizationById200Response.from_json(json)
# print the JSON string representation of the object
print(GetOrganizationById200Response.to_json())

# convert the object into a dict
get_organization_by_id200_response_dict = get_organization_by_id200_response_instance.to_dict()
# create an instance of GetOrganizationById200Response from a dict
get_organization_by_id200_response_from_dict = GetOrganizationById200Response.from_dict(get_organization_by_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


