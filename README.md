# @billagent/usage-events

BillAgent Usage Events API client for TypeScript/JavaScript

## Installation

```bash
npm install @billagent/usage-events
```

## Usage

```typescript
import { UsageEventsUsageTermMatcherServiceApi, Configuration } from '@billagent/usage-events';

// Configure the API client
const configuration = new Configuration({
  basePath: 'https://api.billagent.ai', // Replace with your API endpoint
  apiKey: 'your-api-key-here', // Replace with your API key
});

// Create the API instance
const api = new UsageEventsUsageTermMatcherServiceApi(configuration);

// Process a usage event
const usageEvent = {
  sku_id: 'your-sku-id',
  contract_uuid: 'your-contract-uuid',
  event_time: new Date().toISOString(),
  request_type: 'your-request-type',
  count: '1'
};

try {
  const response = await api.usageTermMatcherServiceIntakeUsageEvent(usageEvent);
  console.log('Term matches:', response.data.term_matches);
  console.log('Errors:', response.data.term_match_errors);
} catch (error) {
  console.error('Error processing usage event:', error);
}
```

## API Reference

### UsageEventsUsageTermMatcherServiceApi

#### `usageTermMatcherServiceIntakeUsageEvent(body: V1IntakeUsageEventRequest)`

Processes a usage event and returns matched terms.

**Parameters:**
- `body`: The usage event request object

**Returns:**
- Promise resolving to `V1IntakeUsageEventResponse`

## Types

### V1IntakeUsageEventRequest
- `sku_id` (string, required): SKU ID that matches contract terms
- `contract_uuid` (string, required): Contract UUID associated with the event
- `event_time` (string, optional): Event timestamp (ISO 8601 format)
- `request_type` (string, required): Request type for term matching
- `count` (string, optional): Count field (defaults to "1")

### V1IntakeUsageEventResponse
- `term_matches` (V1TermMatch[]): Array of matched terms
- `term_match_errors` (V1TermMatchError[]): Array of any errors

## Authentication

This SDK uses API key authentication. Include your API key in the configuration:

```typescript
const configuration = new Configuration({
  apiKey: 'your-api-key-here'
});
```

## License

Copyright 2025 BillAgent.ai Inc.

## Support

For support, visit [BillAgent.ai](https://www.billagent.ai) or contact support@billagent.ai