# SubscriptionList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionGetData]**](SubscriptionGetData.md) |  | 
**pagination** | [**ProductListPagination**](ProductListPagination.md) |  | 

## Example

```python
from moosyl.models.subscription_list import SubscriptionList

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionList from a JSON string
subscription_list_instance = SubscriptionList.from_json(json)
# print the JSON string representation of the object
print(SubscriptionList.to_json())

# convert the object into a dict
subscription_list_dict = subscription_list_instance.to_dict()
# create an instance of SubscriptionList from a dict
subscription_list_from_dict = SubscriptionList.from_dict(subscription_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


