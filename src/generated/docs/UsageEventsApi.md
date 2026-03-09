# UsageEventsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**termMatcherServiceIntakeEvent**](#termmatcherserviceintakeevent) | **POST** /product/usage-intake | Process a usage event|

# **termMatcherServiceIntakeEvent**
> V1IntakeEventResponse termMatcherServiceIntakeEvent(body)

Matches usage events to contract terms and returns event price and matched term metadata.

### Example

```typescript
import {
    UsageEventsApi,
    Configuration,
    V1IntakeEventRequest
} from '@billagent/usage-events';

const configuration = new Configuration();
const apiInstance = new UsageEventsApi(configuration);

let body: V1IntakeEventRequest; //

const { status, data } = await apiInstance.termMatcherServiceIntakeEvent(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **V1IntakeEventRequest**|  | |


### Return type

**V1IntakeEventResponse**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A successful response. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

