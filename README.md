📌 Project Objective :-

The objective of this project is to securely enable and manage cross-account access to Amazon S3 buckets, allowing designated AWS accounts (external or internal to the organization) to access, read, or write to specific S3 buckets without compromising security or governance standards.

📌 Project Description :-

1] This project implements a secure, scalable, and auditable solution for sharing Amazon S3 data between AWS accounts.

2] Account A (Bucket Owner): Owns the S3 bucket that needs to be shared.

3] Account B (Requester): Applications or users that require access to the S3 bucket.

4] IAM Roles & Policies: Provide controlled, temporary credentials.

5] S3 Access Grants / Bucket Policies: Define permissions for cross-account sharing.

6] This ensures controlled, secure, and fine-grained access management between accounts.


📌 Architecture Flow :-
<img width="1200" height="700" alt="image" src="https://github.com/user-attachments/assets/6e4d5d4e-feb3-4df1-9de2-021492b4cec5" />

📌 Benefits of This Setup

✅ Secure Data Sharing – No need to expose permanent credentials.

✅ Cost Efficient – Centralized storage, avoiding data duplication.

✅ Centralized Data Management – Single source of truth.

✅ Scalability – Supports multiple AWS accounts and apps.

✅ Auditability – Track access using CloudTrail and logs.

✅ Fine-Grained Permissions – Control access at bucket/object level.

✅ Multi-Tenant Support – Different accounts can access different data securely.

📖 How to Use:-
1.Create an S3 Bucket in Account A.

2.Set Up IAM Role & S3 Access Grants in Account A.

3.Configure Bucket Policies to allow cross-account access.

4.In Account B, request credentials using AWS SDK/CLI.

5.Access the S3 Bucket with temporary credentials.


