# GetCheckoutSessionPublicByIdPaymentStatus200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 
**claim_expires_at** | **str** |  | 
**success_url** | **str** |  | 

## Example

```python
from moosyl.models.get_checkout_session_public_by_id_payment_status200_response import GetCheckoutSessionPublicByIdPaymentStatus200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetCheckoutSessionPublicByIdPaymentStatus200Response from a JSON string
get_checkout_session_public_by_id_payment_status200_response_instance = GetCheckoutSessionPublicByIdPaymentStatus200Response.from_json(json)
# print the JSON string representation of the object
print(GetCheckoutSessionPublicByIdPaymentStatus200Response.to_json())

# convert the object into a dict
get_checkout_session_public_by_id_payment_status200_response_dict = get_checkout_session_public_by_id_payment_status200_response_instance.to_dict()
# create an instance of GetCheckoutSessionPublicByIdPaymentStatus200Response from a dict
get_checkout_session_public_by_id_payment_status200_response_from_dict = GetCheckoutSessionPublicByIdPaymentStatus200Response.from_dict(get_checkout_session_public_by_id_payment_status200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


