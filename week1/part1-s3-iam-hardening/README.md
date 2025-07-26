# 🛡️ Week 1 – Part 1: Securing an S3 Bucket & IAM User Access

This project simulates a misconfigured public S3 bucket and an over-privileged IAM user. The goal is to fix both issues using AWS security best practices like the principle of least privilege, proper bucket policies, and access logging.

## 🔍 Objective

- Simulate a public S3 bucket and excessive IAM permissions.
- Apply the principle of least privilege with IAM policies and bucket policies.
- Enable access logging for visibility and auditing.

## 🧪 Steps Performed

1. Searched and navigated to the S3 service in the AWS Console.
2. Created a new S3 bucket: `koredesec-cloudsec-demo`.
3. Uploaded a sample file: `sensitive.txt`.
4. Disabled the “Block all public access” settings (simulating misconfiguration).
5. Copied and tested the public object URL to confirm exposure.
6. Opened the link in Incognito mode to confirm public access.
7. Created a new IAM user named `junior-analyst` with full S3 access (initially).
8. Scoped down the IAM user permissions to limit access only to the demo bucket.
9. Created and attached a secure S3 bucket policy.
10. Re-tested access using the IAM user.
11. Enabled **S3 server access logging** to an external logging bucket.

## 📂 Files

- [`IAM-policy.json`](./IAM-policy.json) – Scoped IAM policy for `junior-analyst`
- [`bucket-policy.json`](./bucket-policy.json) – Final secured bucket policy
- `/screenshots/` – Folder containing all screenshots of the steps

## 📸 Screenshot Summary

| Step | Screenshot Filename | Description |
|------|----------------------|-------------|
| 1 | `1-S3.png` | Searching for S3 in the AWS console |
| 2 | `2-Disable-blockpublic-access.png` | Disabling block public access settings |
| 3 | `3-S3-creation.png` | Creating the S3 bucket |
| 4 | `4-S3-public-access-json.png` | Bucket is now publicly accessible |
| 5 | `5-S3-upload.png` | Uploading the `sensitive.txt` file |
| 6 | `6-Iam-user-creation-summary.png` | IAM user creation summary screen |
| 7 | `7-Iam-user-creation.png` | IAM user creation with S3 permissions |
| 8 | `8-iam-junior-analyst-policy.png` | Scoped IAM policy attached to the user |
| 9 | `9-server-access-logging.png` | Enabling server access logging |
| 10 | `10-test-confirming-policy.png` | Testing access with IAM credentials |

## 📝 Write-Up

Read the full blog post on Medium:

🔗 [Week 1 – Securing S3 & IAM on AWS (Medium)](https://medium.com/@Korede_Sec/week-1-securing-s3-and-iam-in-aws-simulating-and-fixing-real-world-cloud-misconfigurations-b86ec65a19d8)

