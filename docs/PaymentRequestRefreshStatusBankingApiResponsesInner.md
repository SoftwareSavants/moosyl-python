# PaymentRequestRefreshStatusBankingApiResponsesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**transaction_id** | **str** |  | 
**configuration_id** | **str** |  | 
**configuration_type** | **str** |  | 
**outcome** | **str** |  | 
**body** | **str** |  | 

## Example

```python
from moosyl.models.payment_request_refresh_status_banking_api_responses_inner import PaymentRequestRefreshStatusBankingApiResponsesInner

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentRequestRefreshStatusBankingApiResponsesInner from a JSON string
payment_request_refresh_status_banking_api_responses_inner_instance = PaymentRequestRefreshStatusBankingApiResponsesInner.from_json(json)
# print the JSON string representation of the object
print(PaymentRequestRefreshStatusBankingApiResponsesInner.to_json())

# convert the object into a dict
payment_request_refresh_status_banking_api_responses_inner_dict = payment_request_refresh_status_banking_api_responses_inner_instance.to_dict()
# create an instance of PaymentRequestRefreshStatusBankingApiResponsesInner from a dict
payment_request_refresh_status_banking_api_responses_inner_from_dict = PaymentRequestRefreshStatusBankingApiResponsesInner.from_dict(payment_request_refresh_status_banking_api_responses_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


