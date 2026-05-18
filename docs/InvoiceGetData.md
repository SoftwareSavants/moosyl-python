# InvoiceGetData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | 
**customer_id** | **UUID** |  | 
**organization_id** | **UUID** |  | 
**status** | **str** |  | 
**amount** | **str** |  | 
**due_date** | **datetime** |  | 
**payment_request_id** | **UUID** |  | 
**created_at** | **datetime** |  | 

## Example

```python
from moosyl.models.invoice_get_data import InvoiceGetData

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceGetData from a JSON string
invoice_get_data_instance = InvoiceGetData.from_json(json)
# print the JSON string representation of the object
print(InvoiceGetData.to_json())

# convert the object into a dict
invoice_get_data_dict = invoice_get_data_instance.to_dict()
# create an instance of InvoiceGetData from a dict
invoice_get_data_from_dict = InvoiceGetData.from_dict(invoice_get_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


