# 🔐 Week 1 – Part 2: Monitoring Root Activity on AWS using CloudTrail, KMS, SNS & EventBridge

This project detects sensitive root account activity in AWS using a full pipeline: CloudTrail for logging, KMS for encryption, SNS for real-time alerts, and EventBridge to automate the detection logic.

## 🔍 Objective

- Simulate root account usage and detect it.
- Set up centralized logging using CloudTrail and KMS.
- Create real-time alerts using SNS + EventBridge.

## 🧪 Steps Performed

1. Signed in to AWS using the root account.
2. Accessed the Billing Console to simulate sensitive activity.
3. Created a CloudTrail trail (using the existing S3 bucket).
4. Created a **KMS key** with appropriate key policy for CloudTrail.
5. Enabled encryption for CloudTrail using the KMS key.
6. Verified CloudTrail logs were written to the S3 bucket.
7. Created an SNS topic (`RootActivityTopic`) and email subscription.
8. Verified the email subscription via confirmation link.
9. Created an **EventBridge rule** to detect root sign-in and trigger SNS.
10. Logged in again as root to test and received an alert.

## 📂 Files

- [`kms-policy.json`](./kms-policy.json) – Custom KMS key policy for CloudTrail
- [`eventbridge-rule.json`](./eventbridge-rule.json) – Rule that detects root login
- `/screenshots/` – Folder containing visual proof for each stage

## 📸 Screenshot Summary

| Step | Screenshot Filename | Description |
|------|----------------------|-------------|
| 1 | `11-root-login.png` | Root account sign-in |
| 2 | `12-billing-console.png` | Viewing billing console (simulated sensitive action) |
| 3 | `13-cloudtrail-setup.png` | CloudTrail setup UI |
| 4 | `14-kms-key-creation.png` | Creating new KMS key |
| 5 | `15-kms-key-json-policy.png` | Final KMS key policy in JSON |
| 6 | `16-kms-key-created.png` | Confirmation that KMS key was created |
| 7 | `17-cloud-trail-setup-summary.png` | Summary of CloudTrail configuration |
| 8 | `18-cloudtrail-creation.png` | Trail successfully created |
| 9 | `19-cloudtrail-log.png` | CloudTrail log entry for root login |
| 10 | `20-Sns-topic-subscription.png` | SNS topic created, waiting for confirmation |
| 11 | `21-subscription-confirmation.png` | Email confirmation link |
| 12 | `22-subscription-confirmed.png` | Email subscription confirmed |
| 13 | `23-eventbridge-rule.png` | EventBridge rule detecting root login |

## 📝 Write-Up

Read the full blog post on Medium:

🔗 [Week 1 – Part 2: Monitoring Root Activity on AWS (Medium)](https://medium.com/@Korede_Sec/️week-1-part-2-monitoring-root-activity-on-aws-using-cloudtrail-kms-sns-eventbridge-043b0a2f53ad)

