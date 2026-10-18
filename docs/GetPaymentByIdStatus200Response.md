# GetPaymentByIdStatus200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**status** | **str** |  | 
**reference_id** | **str** |  | 
**claim_expires_at** | **str** |  | 

## Example

```python
from moosyl.models.get_payment_by_id_status200_response import GetPaymentByIdStatus200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetPaymentByIdStatus200Response from a JSON string
get_payment_by_id_status200_response_instance = GetPaymentByIdStatus200Response.from_json(json)
# print the JSON string representation of the object
print(GetPaymentByIdStatus200Response.to_json())

# convert the object into a dict
get_payment_by_id_status200_response_dict = get_payment_by_id_status200_response_instance.to_dict()
# create an instance of GetPaymentByIdStatus200Response from a dict
get_payment_by_id_status200_response_from_dict = GetPaymentByIdStatus200Response.from_dict(get_payment_by_id_status200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


