# PaymentRequestRefreshStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**PaymentRequestGetData**](PaymentRequestGetData.md) |  | 
**banking_api_responses** | [**List[PaymentRequestRefreshStatusBankingApiResponsesInner]**](PaymentRequestRefreshStatusBankingApiResponsesInner.md) |  | 

## Example

```python
from moosyl.models.payment_request_refresh_status import PaymentRequestRefreshStatus

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentRequestRefreshStatus from a JSON string
payment_request_refresh_status_instance = PaymentRequestRefreshStatus.from_json(json)
# print the JSON string representation of the object
print(PaymentRequestRefreshStatus.to_json())

# convert the object into a dict
payment_request_refresh_status_dict = payment_request_refresh_status_instance.to_dict()
# create an instance of PaymentRequestRefreshStatus from a dict
payment_request_refresh_status_from_dict = PaymentRequestRefreshStatus.from_dict(payment_request_refresh_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


