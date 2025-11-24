# Active Directory Domain Services (AD DS) Lab

This project demonstrates how I installed and configured Active Directory Domain Services (AD DS) on a Windows Server 2019 virtual machine. The goal of this lab is to learn how to deploy AD DS, promote a server to a Domain Controller, set up DNS, and create a new domain.

---

## 🔧 Lab Overview
- **Server OS:** Windows Server 2019  
- **Role Installed:** Active Directory Domain Services (AD DS)  
- **Domain Created:** jzdomain.local  
- **Network Type:** NAT + Host-Only Adapter  
- **Purpose:** Build a working Active Directory environment for system administration practice.

---

## 🛠 Skills Demonstrated
- Installing server roles  
- Creating an Active Directory forest  
- DNS configuration  
- Domain controller promotion  
- Windows Server administration  
- Documentation and lab design  

---

# 📌 **AD DS Installation Steps (With Screenshot Placeholders)**



---

### **1️⃣ Step 1 — Add Roles and Features**
Opened **Server Manager** and clicked **Add Roles and Features** to begin the AD DS installation process.

![Step 1 Add Roles and Features](IMAGE_HERE)

---

### **2️⃣ Step 2 — Installation Type**
Selected **Role-based or feature-based installation**.  
This tells Windows you are adding a server role directly to this machine (not remote or multi-server deployment).

![Step 2 Installation Type](IMAGE_HERE)

---

### **3️⃣ Step 3 — Server Selection**
Confirmed that the local server was selected as the installation target.

![Step 3 Server Selection](IMAGE_HERE)

---

### **4️⃣ Step 4 — Server Roles**
Checked **Active Directory Domain Services**.  
This installs the services required for:
- user authentication  
- Group Policy  
- domain management  

![Step 4 Server Roles](IMAGE_HERE)

---

### **5️⃣ Step 5 — Confirmation**
Reviewed the selected options and started installation of the AD DS binaries.

![Step 5 Confirmation](IMAGE_HERE)

---

### **6️⃣ Step 6 — Promote This Server to a Domain Controller**
After installation, selected **Promote this server to a domain controller**.  
This makes the server the authority for authentication, domain logins, and Group Policy.

![Step 6 Promote](IMAGE_HERE)

---

### **7️⃣ Step 7 — Deployment Configuration**
Chose **Add a new forest** and created a new domain:

**jzdomain.local**

![Step 7 Deployment Configuration](IMAGE_HERE)

---

### **8️⃣ Step 8 — Domain Controller Options**
Configured:
- Domain Controller capability  
- DNS installation  
- Global Catalog  
- DSRM password (for recovery mode)

![Step 8 Domain Controller Options](IMAGE_HERE)

---

### **9️⃣ Step 9 — NetBIOS Domain Name**
Verified the NetBIOS name matched the domain prefix.  
This ensures compatibility with older tools that rely on short naming.

![Step 9 NetBIOS](IMAGE_HERE)

---

### **🔟 Step 10 — Review Options**
Reviewed the final configuration before installation and promotion began.

![Step 10 Review](IMAGE_HERE)

---

# 📚 What I Learned
This lab helped me understand:
- How Active Directory is installed  
- How a Domain Controller works  
- The DNS requirements for AD  
- Deployment of domain services in a virtual environment  

---

### **Created by: Jorge Zepeda**
