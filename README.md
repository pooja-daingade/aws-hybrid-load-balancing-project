# AWS ALB + NLB Architecture Project

## 📌 Overview
This project demonstrates a real-world AWS architecture combining Network Load Balancer (NLB) and Application Load Balancer (ALB).

- NLB handles high-performance traffic at Layer 4
- ALB handles intelligent routing at Layer 7
- Used for scalable and highly available web applications

---

## 🏗️ Architecture
<img width="1536" height="1024" alt="ALB+NLB Architecture" src="https://github.com/user-attachments/assets/ba0ef684-9760-4bbc-9fc3-9dd737123c2f" />


### Flow:
Client → NLB → ALB → Target Groups → EC2 Instances

---

## ⚙️ Services Used

- AWS EC2
- Application Load Balancer (ALB)
- Network Load Balancer (NLB)
- Target Groups
- Auto Scaling (optional)


---

## 🔧 Implementation Steps

### Step 1: Create EC2 Instances
- Launch multiple EC2 instances
- Install web server (Apache/Nginx)
- Create different pages (Home, Mobile, Laptop)

---

### Step 2: Create Target Groups
- Create separate target groups:
  - Home TG
  - Mobile TG
  - Laptop TG
- Register EC2 instances

---

### Step 3: Create ALB
- Configure ALB (Layer 7)
- Add listeners:
  - `/home/`
  - `/mobile/`
  - `/laptop/`
- Attach target groups

---

### Step 4: Create NLB
- Configure NLB (Layer 4)
- Forward traffic to ALB

---

### Step 5: Testing
- Access via NLB DNS
- Verify routing works correctly

---

## 📸 Screenshots

### ALB
<img width="1919" height="872" alt="ALB" src="https://github.com/user-attachments/assets/07d37076-16b3-4d8e-ba56-78f32dbdd772" />


### NLB
<img width="1919" height="879" alt="NLB" src="https://github.com/user-attachments/assets/7f1a9e84-5f1f-4ba0-ba84-e9f14313e71e" />

---

## 🎯 Key Learnings

- Difference between ALB and NLB
- Layer 4 vs Layer 7 routing
- High availability architecture
- Load balancing strategies

---

## 📌 Use Cases

- High traffic applications
- Microservices architecture
- Real-time applications

---

## 👨‍💻 Author
Pooja Daingade
