# S3-Static-Website

### AWS S3 Static Website Deployment

This project demonstrates how to host a fully static personal website using AWS S3 and CloudFront. It includes:

✅ A responsive HTML/CSS site  
✅ Public S3 hosting  
✅ Optional HTTPS setup with CloudFront  

---

## 📌 Technologies Used
- HTML/CSS
- AWS S3 (Static Site Hosting)
- AWS IAM (Permissions)
CloudFront

---

## 🚀 How to Deploy This Project

1. Create an S3 bucket named khomotso
2. Upload `index.html` 
3. Enable Static Website Hosting in **S3 > Properties**
4. Set permissions:
   - Go to **Permissions > Bucket Policy**
   - Paste this JSON:
     ```json
     {
       "Version": "2012-10-17",
     "Id:"Policy1745262987729",
       "Statement": [
         {
           "Sid":"Stmt1745262985563",
           "Effect": "Allow",
           "Principal": "*",
           "Action": "s3:GetObject",
           "Resource": "arn:aws:s3:::khomotso/*"
         }
       ]
     }
     ```
5. Visit your **Static Website Endpoint** to see your site live!

---

### Live Website  
![Live URL](https://khomotso.s3.eu-north-1.amazonaws.com/bk-homes+(7).png)

---

## 📡 Live Demo (if applicable)
🌐 [http://acs.amazonaws.com/groups/global/AllUsers]

### S3 Bucket Setup  
![S3 Dashboard]![S3 Dashboard](https://github.com/user-attachments/assets/f9f761cd-c468-4f1b-9569-0cdec76978b5)


---

##  Author
**Khomotso Matsapola**  
 
