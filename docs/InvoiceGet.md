# InvoiceGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InvoiceGetData**](InvoiceGetData.md) |  | 

## Example

```python
from moosyl.models.invoice_get import InvoiceGet

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceGet from a JSON string
invoice_get_instance = InvoiceGet.from_json(json)
# print the JSON string representation of the object
print(InvoiceGet.to_json())

# convert the object into a dict
invoice_get_dict = invoice_get_instance.to_dict()
# create an instance of InvoiceGet from a dict
invoice_get_from_dict = InvoiceGet.from_dict(invoice_get_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


