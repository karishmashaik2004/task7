# ☁️ Task 7: Configure Load Balancing and Auto Scaling (AWS)

## 🎯 Objective
To deploy a simple web app on AWS EC2 instances using a **Load Balancer** and **Auto Scaling Group**, ensuring high availability and scalability.

---

## 🛠️ Tools Used
- AWS EC2  
- Application Load Balancer (ALB)  
- Auto Scaling Group  
- Apache Web Server  

---

## ⚙️ Steps Performed

1. **Launched EC2 Instance**
   - Amazon Linux 2 AMI  
   - Installed Apache web server using user data script.

2. **Configured Web Page**
   Instead of uploading an HTML file, created the webpage directly inside EC2 using this command:
   ```bash
   echo "<h2>Hello from EC2 instance: $(hostname)</h2><p>Served via Load Balancer</p>" | sudo tee /var/www/html/index.html
