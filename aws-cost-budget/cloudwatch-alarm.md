# CloudWatch Alarm Configuration

## Alarm Details
- **Alarm Name**: monthly-billing-alert
- **Region**: us-east-1 (N. Virginia)
- **Description**: Optional field available for markdown formatting

## Metric Configuration
- **Namespace**: AWS/Billing
- **Metric Name**: EstimatedCharges (Total Estimated Charge)
- **Currency**: USD
- **Data Source**: Global billing metrics
- **Period Options**: 1h, 3h, 12h, 1d available

## Alarm States
- **In Alarm**: Metric exceeds defined threshold
- **OK**: Metric within defined threshold  
- **Insufficient Data**: Not enough data available or alarm just started

## Actions Configuration
- **Alarm State Trigger**: In alarm (when threshold exceeded)
- **Notification Method**: SNS Topic
- **SNS Topic**: monthly-billing
- **Topic ARN**: arn:aws:sns:us-east-1:[REDACTED ACCOUNT ID]:monthly-billing
- **Email Endpoint**: [REDACTED EMAIL]

## Setup Process
1. Navigate to CloudWatch → Alarms → Create alarm
2. Select metric: AWS/Billing → EstimatedCharges
3. Configure threshold and conditions
4. Add SNS action for notifications
5. Set alarm name and optional description
6. Review and create alarm

## Available Regions for Billing Metrics
- Global (recommended for billing)
- N. Virginia (us-east-1)
- Multiple other regions available but billing metrics are typically global
