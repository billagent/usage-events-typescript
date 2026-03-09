# V1IntakeEventRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contract_uuid** | **string** | Required: this is the contract uuid associated with this event, if the contract is not found, or if the contract is not active, a match will not occur. | [optional] [default to undefined]
**event_time** | **string** | Optional:the time of the event, if the event time does not fit within the contract term dates a match will not occur. If this value is left out it will default to now(). | [optional] [default to undefined]
**milestone_event_match** | [**V1MilestoneEventMatch**](V1MilestoneEventMatch.md) |  | [optional] [default to undefined]
**usage_event_match** | [**V1UsageEventMatch**](V1UsageEventMatch.md) |  | [optional] [default to undefined]

## Example

```typescript
import { V1IntakeEventRequest } from '@billagent/usage-events';

const instance: V1IntakeEventRequest = {
    contract_uuid,
    event_time,
    milestone_event_match,
    usage_event_match,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
