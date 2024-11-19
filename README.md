# **AWS Static Website Deployment with Security and Automation**

![Screenshot from 2024-11-19 20-11-30](https://github.com/user-attachments/assets/700d34f2-cf34-4cfc-9afe-e533d8bab6cb)


## **Project Overview**
This project demonstrates the deployment of a **static website** on **Amazon Web Services (AWS)** with a focus on security, scalability, and automation. The goal was to explore various AWS services and understand how they work together to build a robust, secure, and highly available web application. 

Throughout the project, I deepened my understanding of cloud computing concepts, AWS infrastructure, and automation practices, learning about why each service exists, the problem it solves, and how it fits into the larger solution.

## **Key Features**

- **Static Website Hosting:** Deployed a static website on **Amazon S3**.
- **Security Enhancements:** Disabled public access to the S3 bucket to protect sensitive data.
- **SSL & HTTPS:** Secured the website with **HTTPS** and an SSL certificate using **AWS Certificate Manager (ACM)**.
- **Global Content Delivery:** Integrated **AWS CloudFront** CDN to ensure low-latency access to content from anywhere in the world.
- **Domain Mapping:** Used **AWS Route 53** to map the website to a custom domain.
- **CI/CD Automation:** Configured an automated deployment pipeline using **AWS CodePipeline**.

## **Technologies Used**

- **Amazon S3** - For hosting the static website.
- **AWS Certificate Manager (ACM)** - For managing SSL certificates and securing the website with HTTPS.
- **AWS CloudFront** - For content delivery and reduced latency.
- **AWS Route 53** - For DNS management and domain mapping.
- **AWS CodePipeline** - For setting up continuous integration and continuous deployment (CI/CD).

## **Project Setup**

### **Prerequisites**
To get this project up and running locally or to deploy it to AWS, you will need:

- An active **AWS account**.
- AWS CLI installed and configured on your machine.
- Basic understanding of AWS services (S3, ACM, CloudFront, Route 53, CodePipeline).

### **Steps for Deployment**

1. **Set Up Amazon S3 Bucket:**
   - Create an S3 bucket to host your static website.
   - Upload your website files (HTML, CSS, JavaScript, etc.) to the bucket.
   - Disable public access to the bucket for security.

2. **Configure AWS Certificate Manager (ACM):**
   - Request an SSL certificate for your domain using ACM.
   - Attach the certificate to your S3 bucket for HTTPS access.

3. **Set Up CloudFront CDN:**
   - Create a CloudFront distribution for your S3 bucket.
   - Configure the distribution settings for low-latency global access.

4. **Map Domain Using Route 53:**
   - Set up Route 53 DNS records to map your custom domain to the CloudFront distribution.
   - Ensure that traffic to your domain is routed securely.

5. **Automate with CodePipeline:**
   - Create a pipeline using CodePipeline to automate deployments from a GitHub repository to your S3 bucket.
   - Configure build and deployment stages to deploy changes automatically.

## **Deployment Instructions**

1. **Clone this Repository:**

    ```bash
    git clone https://github.com/your-username/aws-static-website-deployment.git
    cd aws-static-website-deployment
    ```

2. **Configure AWS CLI:**
   - Run the following command to configure AWS CLI with your credentials:

    ```bash
    aws configure
    ```

3. **Follow the Steps Above for Deployment:**
   - Follow the steps mentioned in the "Project Setup" section to deploy the website on AWS.

## **Screenshots**

Include a screenshot or preview of the website once deployed, if possible:

![Screenshot from 2024-11-20 00-05-33](https://github.com/user-attachments/assets/edc685db-2298-4679-8e82-921efc59ed80)


## **Challenges Faced**

- **S3 Security Configuration:** Initially, I struggled with ensuring the S3 bucket was secure while still being accessible for website traffic. The solution involved fine-tuning the access permissions and leveraging AWS best practices for security.
- **Domain Mapping:** Ensuring the custom domain pointed correctly to the CloudFront distribution was a bit tricky, but AWS Route 53's easy-to-follow setup solved that.

## **Learnings**

This project gave me hands-on experience with **AWS services**, particularly around security, scalability, and automation. I gained practical insights into the following:

- How to host a static website securely using **Amazon S3**.
- Best practices for securing website traffic using **SSL certificates** via **AWS Certificate Manager (ACM)**.
- The benefits of using a **CloudFront CDN** for global content delivery and reduced latency.
- How to automate deployments using **AWS CodePipeline** for faster and more reliable updates.

## **Future Improvements**

- Add logging and monitoring using **Amazon CloudWatch** to track the performance and usage of the website.
- Enhance the security further by integrating **WAF (Web Application Firewall)** for protection against malicious traffic.
- Implement more complex CI/CD pipelines with additional stages such as **build and testing** before deployment.

## **Conclusion**

This project was an excellent opportunity to combine my theoretical knowledge with hands-on practice, reinforcing my understanding of cloud services and AWS. It also helped me improve my skills in deploying secure, scalable, and automated cloud applications.

---

**Author:** Anurag Hatole
**GitHub:** https://github.com/anuraghatole

---
