# Activity-audit
# EX - 4 Auditing Cloud Activity Using AWS CloudTrail

## Aim

To enable and analyze AWS CloudTrail logs to audit user and resource activities in a cloud environment.

## Requirements
1. AWS Console access
2. CloudTrail service enabled
3. S3 bucket (for storing logs)
4. IAM permissions to view audit logs

## Procedure

### Step 1: Enable CloudTrail
Go to CloudTrail from AWS Console
Click Trails > Create trail
Name: CloudAuditTrail
Apply trail to all regions
Log events:
 - Management events: Read & Write
 - Data events: S3, Lambda (optional)
Create or select an S3 bucket for log storage
Enable CloudWatch Logs integration (optional)

### Step 2: Review Event History
Go to Event history
Filter events by:
- Username (IAM role or user)
- Event name (e.g., CreateBucket, TerminateInstances)
- Date/Time
- Resource type (e.g., S3, EC2)

### Step 3: Download or Export Logs

Use the Download CSV option to export logs
Analyze logs in Excel/Sheets for reporting

## Output:

<img width="1687" height="416" alt="image" src="https://github.com/user-attachments/assets/c45d17d2-002e-4c8c-9708-19f70e177c79" />

<img width="1489" height="601" alt="image" src="https://github.com/user-attachments/assets/591a57af-0389-44c0-ab69-50419ed3fb0c" />

<img width="1577" height="798" alt="image" src="https://github.com/user-attachments/assets/99ad5509-5640-441d-b2be-68d1eaa26f61" />

## Result

All AWS user activities, including volume creation, deletion, and permission changes, were successfully audited using CloudTrail.
