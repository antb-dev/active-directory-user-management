# 👥 Active Directory User Account Management Guide

This repository is a step-by-step guide to managing user accounts in **Active Directory (AD)**, one of the most common tasks for IT Support and System Administrators.  

It demonstrates practical skills in **Windows Server administration, account lifecycle management, and group policy basics**.  
All screenshots are from a sample AD lab environment.  

---

## 🛠️ Prerequisites
- Windows Server with **Active Directory Domain Services (AD DS)** installed
- Administrative privileges on the Domain Controller
- Access to **Active Directory Users and Computers (ADUC)**

---

## 📖 Table of Contents
1. [Opening ADUC](#opening-aduc)  
2. [Creating a New User](#creating-a-new-user)  
3. [Resetting a User Password](#resetting-a-user-password)  
4. [Disabling or Enabling Accounts](#disabling-or-enabling-accounts)  
5. [Managing Group Memberships](#managing-group-memberships)  
6. [Deleting Accounts](#deleting-accounts)  

---

## 1️⃣ Opening ADUC
Open **Active Directory Users and Computers (ADUC):**
- Press `Win + R`, type `dsa.msc`, and hit **Enter**.  
- Or navigate via **Server Manager → Tools → Active Directory Users and Computers**.  



---

## 2️⃣ Creating a New User
1. In ADUC, right-click the desired **Organizational Unit (OU)**.  
2. Select **New → User**.  
3. Fill in user details (First Name, Last Name, User Logon Name).  
4. Set an initial password and configure whether the user must change it at next logon.  



---

## 3️⃣ Resetting a User Password
1. Right-click the user account in ADUC.  
2. Select **Reset Password**.  
3. Enter a new password and optionally force password change at next logon.  



---

## 4️⃣ Disabling or Enabling Accounts
- **Disable**: Right-click user → **Disable Account**.  
- **Enable**: Right-click disabled account → **Enable Account**.  

This is useful when employees leave temporarily (e.g., leave of absence).  

---

## 5️⃣ Managing Group Memberships
1. Open the user’s **Properties**.  
2. Go to the **Member Of** tab.  
3. Add or remove groups to adjust permissions and access.  

 


---

## 6️⃣ Deleting Accounts
- Right-click the user → **Delete**.  
- Use with caution, as deleting removes all user attributes permanently.  
- Best practice: disable first, then delete after offboarding is confirmed.  

---

## 📌 Notes & Best Practices
- Always follow your company’s **account lifecycle policy**.  
- Use **Group Policies (GPOs)** to enforce password complexity.  
- Document account changes for compliance.  
- Automate repetitive tasks with **PowerShell** (future repo idea).  

---

## 👤 About
Created as part of an IT Support learning portfolio to showcase **Active Directory administration skills**.  

