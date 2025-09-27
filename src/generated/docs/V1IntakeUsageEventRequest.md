# V1IntakeUsageEventRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sku_id** | **string** | Required:this is the sku id that matches the sku id in the contract terms. If the sku id does not match a sku id in the contract or the the sku id is not an event type, a match will not occur. | [optional] [default to undefined]
**contract_uuid** | **string** | Required: this is the contract uuid associated with this event, if the contract is not found, or if the contract is not active, a match will not occur. | [optional] [default to undefined]
**event_time** | **string** | Optional:the time of the event, if the event time does not fit within the contract term dates a match will not occur. If this value is left out it will default to now(). | [optional] [default to undefined]
**request_type** | **string** | Required: the request type for the event, this is used to match to the term type. | [optional] [default to undefined]
**count** | **string** | Optional: Count field, defaults to 1 if not provided. | [optional] [default to undefined]

## Example

```typescript
import { V1IntakeUsageEventRequest } from '@billagent/usage-events';

const instance: V1IntakeUsageEventRequest = {
    sku_id,
    contract_uuid,
    event_time,
    request_type,
    count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
