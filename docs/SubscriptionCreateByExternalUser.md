# SubscriptionCreateByExternalUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**external_user_id** | **str** |  | 
**phone** | **str** |  | [optional] 
**price_id** | **str** |  | 
**trial** | [**SubscriptionCreateTrial**](SubscriptionCreateTrial.md) |  | [optional] 
**trial_period** | **str** |  | [optional] 
**trial_end** | [**SubscriptionCreateTrialEnd**](SubscriptionCreateTrialEnd.md) |  | [optional] 
**started_at** | [**SubscriptionCreateTrialEnd**](SubscriptionCreateTrialEnd.md) |  | [optional] 
**expires_at** | [**SubscriptionCreateTrialEnd**](SubscriptionCreateTrialEnd.md) |  | [optional] 

## Example

```python
from moosyl.models.subscription_create_by_external_user import SubscriptionCreateByExternalUser

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionCreateByExternalUser from a JSON string
subscription_create_by_external_user_instance = SubscriptionCreateByExternalUser.from_json(json)
# print the JSON string representation of the object
print(SubscriptionCreateByExternalUser.to_json())

# convert the object into a dict
subscription_create_by_external_user_dict = subscription_create_by_external_user_instance.to_dict()
# create an instance of SubscriptionCreateByExternalUser from a dict
subscription_create_by_external_user_from_dict = SubscriptionCreateByExternalUser.from_dict(subscription_create_by_external_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


