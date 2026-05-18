# SubscriptionGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGetData**](SubscriptionGetData.md) |  | 

## Example

```python
from moosyl.models.subscription_get import SubscriptionGet

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGet from a JSON string
subscription_get_instance = SubscriptionGet.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGet.to_json())

# convert the object into a dict
subscription_get_dict = subscription_get_instance.to_dict()
# create an instance of SubscriptionGet from a dict
subscription_get_from_dict = SubscriptionGet.from_dict(subscription_get_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


