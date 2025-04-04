
Choose the best storage class for your use case:
- `S3 Standard` – for frequent access
- `S3 Intelligent-Tiering` – auto-cost optimization
- `S3 Glacier` / `Glacier Deep Archive` – for archival & backup
- `S3 One Zone-IA` – cost-effective for infrequent access

✅ **Versioning & Lifecycle Policies**  
Keep historical versions of your files and automate transitions to cheaper storage.

✅ **Advanced Security & Access Control**  
- Fine-grained permissions with **IAM**, **Bucket Policies**, and **ACLs**
- Encryption at rest and in transit (SSE-S3, SSE-KMS, SSL/TLS)

✅ **Static Website Hosting**  
Host lightweight websites directly from your S3 bucket!

✅ **Event-Driven Architecture**  
Trigger AWS Lambda, SNS, or SQS automatically on object events like upload, delete, etc.

✅ **Logging, Monitoring & Auditing**  
- Enable **Server Access Logging**
- Use **AWS CloudTrail** and **CloudWatch** for full observability

---

## 🌐 Use Case: Hosting a Static Website on S3

Follow these steps to go live with a static website:

```bash
# 1️⃣ Create an S3 Bucket
- Name it exactly like your domain (e.g., mysite.com)
- Disable "Block all public access"

# 2️⃣ Upload your static files
- index.html, styles.css, images, etc.

# 3️⃣ Enable Static Website Hosting
- Go to Bucket > Properties > Static website hosting
- Set index document (e.g., index.html)

# 4️⃣ (Optional) Add Bucket Policy for Public Read
- Allow public access to website files

# 5️⃣ Access Your Website
- Find your website URL in the Static Website Hosting section

📎 Example Output:
http://your-bucket-name.s3-website-region.amazonaws.com
