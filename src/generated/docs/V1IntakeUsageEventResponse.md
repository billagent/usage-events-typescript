# V1IntakeUsageEventResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**term_matches** | [**Array&lt;V1TermMatch&gt;**](V1TermMatch.md) | The matched terms for the event. If there is more than one returned it means that the count bridges two different price points. | [optional] [default to undefined]
**term_match_errors** | [**Array&lt;V1TermMatchError&gt;**](V1TermMatchError.md) | Holds the list of term match errors that occur, if they occur. | [optional] [default to undefined]

## Example

```typescript
import { V1IntakeUsageEventResponse } from '@billagent/usage-events';

const instance: V1IntakeUsageEventResponse = {
    term_matches,
    term_match_errors,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
