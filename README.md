# 🛡️ 100 Days of AWS Cloud Security  
**Real-World Security Projects | Documented Weekly by [@KoredeSec](https://github.com/KoredeSec)**

Welcome to my 100 Days of AWS Cloud Security journey, where I dive into practical AWS security projects and document everything.  
This isn’t theory, it’s a build-in-public challenge to level up, break things, secure them, and grow as a DevSecOps engineer.
---

## 📌 What This Is

Every week, I take on one hands-on AWS cloud security task that simulates real-world risks and solutions.

Each task includes:
- 📁 A dedicated folder with code, configs, and write-ups
- 📷 Screenshots & architecture diagrams (where applicable)
- ✍️ A full breakdown post on [my Medium](https://medium.com/@Korede_Sec)

---


## 🎯 Week 1: Securing Your First S3 Bucket & IAM User  
🔐 *Root Account Monitoring with CloudTrail + SNS Alerts*

**What I did:**
- Created a secure IAM user with MFA  
- Set up CloudTrail across regions  
- Configured an S3 bucket with access control and logging  
- Monitored root user activity via SNS alerts  

👉 [View Week 1 Project](./week1)

## 🎯 Week 1 Projects

### 🔒 [Part 1 – Securing S3 and IAM Access](./week1/part1-s3-iam-hardening)
> Simulate a public S3 bucket and excessive IAM permissions.  
> Apply security best practices to restrict access and enable audit logging.

- Created a misconfigured public S3 bucket and IAM user with excessive access
- Fixed it by applying least privilege IAM policy and secure bucket policy
- Enabled S3 server access logging to monitor activity

📖 [Read Full Blog Post](https://medium.com/@Korede_Sec/week-1-securing-s3-and-iam-in-aws-simulating-and-fixing-real-world-cloud-misconfigurations-b86ec65a19d8)

---

### 📡 [Part 2 – Monitoring Root Activity with CloudTrail, KMS, SNS & EventBridge](./week1/part2-root-monitoring)
> Set up a detection and alerting pipeline for sensitive root account activity on AWS.

- Created a CloudTrail trail with a custom encrypted S3 bucket using KMS
- Configured SNS topic for real-time alerts
- Created an EventBridge rule to detect root login events

📖 [Read Full Blog Post](https://medium.com/@Korede_Sec/️week-1-part-2-monitoring-root-activity-on-aws-using-cloudtrail-kms-sns-eventbridge-043b0a2f53ad)


---

## 📅 Weekly Progress Tracker

| Week | Project Title | Status |
|------|----------------|--------|
| 1 | IAM + S3 Security + Root Monitoring via CloudTrail & SNS | ✅ Completed |
| 2 | To Be Announced | ⏳ Upcoming |
| 3 | To Be Announced | ⏳ Upcoming |
| 4 | To Be Announced | ⏳ Upcoming |
| 5 | To Be Announced | ⏳ Upcoming |

_This table will update as new tasks drop weekly._

---

## 🧰 Tools & Services Used

- **AWS Services**: IAM, S3, CloudTrail, SNS, EC2, VPC, GuardDuty, Security Hub  
- **AWS CLI** and **Console UI**  
- **Bash** & **Python** scripts  
- **Git & GitHub** for version control  
- **Medium** for documentation  

---

## 🧑‍💻 About Me

I'm **Ibrahim Yusuf**, aka **KoredeSec**   
- 🎓 Cybersecurity student @ Osun State University  
- 👨🏽‍💻 President, NACSS UNIOSUN  
- 📜 ISC2 CC | Microsoft SC-200 | Google Cybersecurity certified  
- 🛠️ Builder of security projects using AWS, Microsoft 365, and open-source tools  
- 🇳🇬 Proudly learning, building, and teaching from Nigeria

I’m doing this to sharpen my skills, build a solid public portfolio, and inspire others in similar situations to **build regardless of limitations**.

---

## ✍️ My Blog Writeups

Each project has a full technical breakdown on Medium:

📖 [https://medium.com/@Korede_Sec](https://medium.com/@Korede_Sec)

You’ll find lessons learned, diagrams, screenshots, commands, and real talk about what worked (and what didn’t).

---

## 🤝 Let’s Connect

- 💼 [LinkedIn](https://www.linkedin.com/in/ibrahim-yusuf-38a267301) 
- 📧 [Email](mailto:yusufibrahimakanji741@gmail.com)
- 🌍 [Medium](https://medium.com/@Korede_Sec)
- 🗣️ [GitHub Discussions](https://github.com/KoredeSec/aws-cloud-security-journey/discussions)

---

## 🧭 How to Use This Repo

```bash
git clone https://github.com/KoredeSec/aws-cloud-security-journey.git

cd aws-cloud-security-journey/week1

```
Inside each week’s folder:
- README.md – project summary
- scripts/ – IAM policies, shell scripts, configs
- screenshots/ – walkthroughs & proofs


### ⚠️ Disclaimer
This repository is for educational purposes only.
No secrets or credentials are stored here. Always secure your own AWS environments.


