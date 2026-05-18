# CheckoutSessionGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CheckoutSessionCreateData**](CheckoutSessionCreateData.md) |  | 
**organization** | [**GetOrganizationById200ResponseData**](GetOrganizationById200ResponseData.md) |  | 
**payment_request** | [**PaymentRequestGetData**](PaymentRequestGetData.md) |  | 
**configurations** | [**List[ConfigurationListDataInner]**](ConfigurationListDataInner.md) |  | 
**latest_payment** | [**CheckoutSessionGetLatestPayment**](CheckoutSessionGetLatestPayment.md) |  | [optional] 

## Example

```python
from moosyl.models.checkout_session_get import CheckoutSessionGet

# TODO update the JSON string below
json = "{}"
# create an instance of CheckoutSessionGet from a JSON string
checkout_session_get_instance = CheckoutSessionGet.from_json(json)
# print the JSON string representation of the object
print(CheckoutSessionGet.to_json())

# convert the object into a dict
checkout_session_get_dict = checkout_session_get_instance.to_dict()
# create an instance of CheckoutSessionGet from a dict
checkout_session_get_from_dict = CheckoutSessionGet.from_dict(checkout_session_get_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


