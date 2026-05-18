# SubscriptionGetData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**organization_id** | **UUID** |  | 
**customer_id** | **UUID** |  | 
**price_id** | **UUID** |  | 
**status** | **str** |  | 
**next_billing_date** | **datetime** |  | 
**started_at** | **datetime** |  | 
**cancelled_at** | **datetime** |  | 
**expires_at** | **datetime** |  | 

## Example

```python
from moosyl.models.subscription_get_data import SubscriptionGetData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGetData from a JSON string
subscription_get_data_instance = SubscriptionGetData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGetData.to_json())

# convert the object into a dict
subscription_get_data_dict = subscription_get_data_instance.to_dict()
# create an instance of SubscriptionGetData from a dict
subscription_get_data_from_dict = SubscriptionGetData.from_dict(subscription_get_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


