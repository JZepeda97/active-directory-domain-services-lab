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

![Step 1 Add Roles and Features](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/1.png?raw=true)

---

### **2️⃣ Step 2 — Installation Type**
Selected **Role-based or feature-based installation**.  
This tells Windows you are adding a server role directly to this machine (not remote or multi-server deployment).

![Step 2 Installation Type](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/2.png?raw=true)

---

### **3️⃣ Step 3 — Server Selection**
Confirmed that the local server was selected as the installation target.

![Step 3 Server Selection](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/3.png?raw=true)

---

### **4️⃣ Step 4 — Server Roles**
Checked **Active Directory Domain Services**.  
This installs the services required for:
- user authentication  
- Group Policy  
- domain management  

![Step 4 Server Roles](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/4.png?raw=true)

---

### **5️⃣ Step 5 — Confirmation**
Reviewed the selected options and started installation of the AD DS binaries.

![Step 5 Confirmation](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/5.png?raw=true)

---

### **6️⃣ Step 6 — Promote This Server to a Domain Controller**
After installation, selected **Promote this server to a domain controller**.  
This makes the server the authority for authentication, domain logins, and Group Policy.

![Step 6 Promote](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/6.png?raw=true)

---

### **7️⃣ Step 7 — Deployment Configuration**
Chose **Add a new forest** and created a new domain:

**jzdomain.local**

![Step 7 Deployment Configuration](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/7.png?raw=true)

---

### **8️⃣ Step 8 — Domain Controller Options**
Configured:
- Domain Controller capability  
- DNS installation  
- Global Catalog  
- DSRM password (for recovery mode)

![Step 8 Domain Controller Options](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/8.png?raw=true)

---

### **9️⃣ Step 9 — NetBIOS Domain Name**
Verified the NetBIOS name matched the domain prefix.  
This ensures compatibility with older tools that rely on short naming.

![Step 9 NetBIOS](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/9.png?raw=true)

---

### **🔟 Step 10 — Review Options**
Reviewed the final configuration before installation and promotion began.

![Step 10 Review](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/10.png?raw=true)

---

### **🔟 Step 11 — Domain Creation Verification**
Opened **Active Directory Users and Computers (ADUC)** to confirm that the domain **jzdomain.local** was successfully created.  
The default containers (Builtin, Computers, Domain Controllers, Users, etc.) confirm the domain and directory structure are active.

![Step 11 Review](https://github.com/JZepeda97/active-directory-domain-services-lab/blob/main/11.png?raw=true)

---

# 📚 What I Learned
This lab helped me understand:
- How Active Directory is installed  
- How a Domain Controller works  
- The DNS requirements for AD  
- Deployment of domain services in a virtual environment  

---

### **Created by: Jorge Zepeda**
