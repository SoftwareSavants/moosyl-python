# CheckoutSessionSwitchMethod


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
from moosyl.models.checkout_session_switch_method import CheckoutSessionSwitchMethod

# TODO update the JSON string below
json = "{}"
# create an instance of CheckoutSessionSwitchMethod from a JSON string
checkout_session_switch_method_instance = CheckoutSessionSwitchMethod.from_json(json)
# print the JSON string representation of the object
print(CheckoutSessionSwitchMethod.to_json())

# convert the object into a dict
checkout_session_switch_method_dict = checkout_session_switch_method_instance.to_dict()
# create an instance of CheckoutSessionSwitchMethod from a dict
checkout_session_switch_method_from_dict = CheckoutSessionSwitchMethod.from_dict(checkout_session_switch_method_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


