# SNS Topic and Subscription Setup

## Topic Details
- **Topic Name**: monthly-billing
- **Topic ARN**: arn:aws:sns:us-east-1:[REDACTED ACCOUNT ID]:monthly-billing
- **Topic Type**: Standard
- **Topic Owner**: [REDACTED ACCOUNT ID]
- **Region**: us-east-1 (N. Virginia)

## Subscriptions
### Confirmed Subscription
- **Endpoint**: [REDACTED EMAIL]
- **Protocol**: EMAIL
- **Status**: Confirmed
- **Subscription ID**: [REDACTED]

### Pending Subscription (if applicable)
- **Endpoint**: [REDACTED EMAIL]
- **Status**: Pending confirmation
- **ARN**: [REDACTED]

## Subscription Process
1. Topic created in SNS console
2. Email subscription added
3. Confirmation email sent to recipient
4. Subscription confirmed via email link
5. Status updated to "Confirmed"

## Features
- **High Throughput FIFO**: Available but using Standard topic
- **Mobile Push**: Available option
- **SMS**: Available option
- **Multiple Endpoints**: Can support up to 10 email recipients
