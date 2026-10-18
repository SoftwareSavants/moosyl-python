# SubscriptionCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | [optional] 
**customer_id** | **UUID** |  | 
**price_id** | **UUID** |  | 
**cancelled_at** | **datetime** |  | [optional] 
**expires_at** | **datetime** |  | [optional] 
**trial** | [**SubscriptionCreateTrial**](SubscriptionCreateTrial.md) |  | [optional] 
**trial_period** | **str** |  | [optional] 
**trial_end** | [**SubscriptionCreateTrialEnd**](SubscriptionCreateTrialEnd.md) |  | [optional] 
**started_at** | [**SubscriptionCreateTrialEnd**](SubscriptionCreateTrialEnd.md) |  | [optional] 

## Example

```python
from moosyl.models.subscription_create import SubscriptionCreate

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionCreate from a JSON string
subscription_create_instance = SubscriptionCreate.from_json(json)
# print the JSON string representation of the object
print(SubscriptionCreate.to_json())

# convert the object into a dict
subscription_create_dict = subscription_create_instance.to_dict()
# create an instance of SubscriptionCreate from a dict
subscription_create_from_dict = SubscriptionCreate.from_dict(subscription_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


