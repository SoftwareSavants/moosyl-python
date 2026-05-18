# CronResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cancelled** | **float** |  | [optional] 
**expired** | **float** |  | [optional] 
**updated** | **float** |  | [optional] 
**processed** | **float** |  | [optional] 
**failed** | **float** |  | [optional] 
**total** | **float** |  | [optional] 
**processed_at** | **str** |  | 

## Example

```python
from moosyl.models.cron_result import CronResult

# TODO update the JSON string below
json = "{}"
# create an instance of CronResult from a JSON string
cron_result_instance = CronResult.from_json(json)
# print the JSON string representation of the object
print(CronResult.to_json())

# convert the object into a dict
cron_result_dict = cron_result_instance.to_dict()
# create an instance of CronResult from a dict
cron_result_from_dict = CronResult.from_dict(cron_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


