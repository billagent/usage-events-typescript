# V1TermMatch

An error that occurred during term matching

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contract_uuid** | **string** | The matched contract uuid for the event. | [optional] [default to undefined]
**sku_id** | **string** | The matched sku id in the contract for the event. | [optional] [default to undefined]
**term_type** | **string** | The matched term type for the event. | [optional] [default to undefined]
**price** | **number** | The price of the event per the matched term. | [optional] [default to undefined]
**line_item_description** | **string** | The invoice_line_description of the matched widget. | [optional] [default to undefined]
**description** | **string** | The description of the matched term or bucket. | [optional] [default to undefined]
**count** | **string** | The count of the event. | [optional] [default to undefined]
**event_time** | **string** | The time of the event. | [optional] [default to undefined]

## Example

```typescript
import { V1TermMatch } from '@billagent/usage-events';

const instance: V1TermMatch = {
    contract_uuid,
    sku_id,
    term_type,
    price,
    line_item_description,
    description,
    count,
    event_time,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
