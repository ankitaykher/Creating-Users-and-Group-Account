# Creating-Users-and-Group-Account

# Creating Users & Groups in Azure Active Directory — CLI-Only Lab

This project documents my hands-on experience following the lab guide from  
📄 `Creating Users and Group Account.docx`,  
with a twist — I completed every step manually using **Azure CLI in Bash**, not the Azure portal.

---

## 🎯 Objective

To create users and groups in **Microsoft Entra ID (formerly Azure Active Directory)** and assign users to groups using only the command line.

---

## 🧑‍💻 What I Did

### ✅ Step 1: Created a new user
```bash
az ad user create \
  --display-name "Test User One" \
  --user-principal-name testuser1@simplilearnhol100744.onmicrosoft.com \
  --password 'Azure@2025!'
```

---

### ✅ Step 2: Created a security group
```bash
az ad group create \
  --display-name "LabUsersGroup" \
  --mail-nickname "LabUsersGroup"
```

---

### ✅ Step 3: Added the user to the group
First, get the user’s Object ID:
```bash
az ad user show \
  --id testuser1@simplilearnhol100744.onmicrosoft.com \
  --query id --output tsv
```

Then add the user:
```bash
az ad group member add \
  --group "LabUsersGroup" \
  --member-id <user-object-id>
```

---

## 📂 Project Structure

```
.
├── README.md
├── commands.txt        # All CLI commands used
├── notes.md            # My observations & learnings
└── screenshots/        # CLI outputs & portal verification
```

---

## 💡 What I Learned

- Identity and access management (IAM) is critical in every cloud setup
- Azure CLI provides better clarity on how actions are performed under the hood
- Errors like RBAC permission issues aren’t blockers — they’re lessons
- Following a PDF is one thing — doing it manually teaches you much more

---

## 🧾 Reference Lab Document

This lab followed:  
**Demo_09_Creating Users and Group Account.docx**  
(*Objective: Add users to Azure subscription, create groups, and assign them manually*)

---

## 🔗 Connect with Me

If you're learning Azure too — let's connect on [LinkedIn](# Creating Users & Groups in Azure Active Directory — CLI-Only Lab

This project documents my hands-on experience following the lab guide from  
📄 `Demo_09_Creating Users and Group Account.docx`,  
with a twist — I completed every step manually using **Azure CLI in Bash**, not the Azure portal.

---

## 🎯 Objective

To create users and groups in **Microsoft Entra ID (formerly Azure Active Directory)** and assign users to groups using only the command line.

---

## 🧑‍💻 What I Did

### ✅ Step 1: Created a new user
```bash
az ad user create \
  --display-name "Test User One" \
  --user-principal-name testuser1@simplilearnhol100744.onmicrosoft.com \
  --password 'Azure@2025!'
```

---

### ✅ Step 2: Created a security group
```bash
az ad group create \
  --display-name "LabUsersGroup" \
  --mail-nickname "LabUsersGroup"
```

---

### ✅ Step 3: Added the user to the group
First, get the user’s Object ID:
```bash
az ad user show \
  --id testuser1@simplilearnhol100744.onmicrosoft.com \
  --query id --output tsv
```

Then add the user:
```bash
az ad group member add \
  --group "LabUsersGroup" \
  --member-id <user-object-id>
```

---

## 📂 Project Structure

```
.
├── README.md
├── commands.txt        # All CLI commands used
├── notes.md            # My observations & learnings
└── screenshots/        # CLI outputs & portal verification
```

---

## 💡 What I Learned

- Identity and access management (IAM) is critical in every cloud setup
- Azure CLI provides better clarity on how actions are performed under the hood
- Errors like RBAC permission issues aren’t blockers — they’re lessons
- Following a PDF is one thing — doing it manually teaches you much more

---

## 🧾 Reference Lab Document

This lab followed:  
**Demo_09_Creating Users and Group Account.docx**  
(*Objective: Add users to Azure subscription, create groups, and assign them manually*)

---

## 🔗 Connect with Me

If you're learning Azure too — let's connect on [LinkedIn](# Creating Users & Groups in Azure Active Directory — CLI-Only Lab

This project documents my hands-on experience following the lab guide from  
📄 `Demo_09_Creating Users and Group Account.docx`,  
with a twist — I completed every step manually using **Azure CLI in Bash**, not the Azure portal.

---

## 🎯 Objective

To create users and groups in **Microsoft Entra ID (formerly Azure Active Directory)** and assign users to groups using only the command line.

---

## 🧑‍💻 What I Did

### ✅ Step 1: Created a new user
```bash
az ad user create \
  --display-name "Test User One" \
  --user-principal-name testuser1@simplilearnhol100744.onmicrosoft.com \
  --password 'Azure@2025!'
```

---

### ✅ Step 2: Created a security group
```bash
az ad group create \
  --display-name "LabUsersGroup" \
  --mail-nickname "LabUsersGroup"
```

---

### ✅ Step 3: Added the user to the group
First, get the user’s Object ID:
```bash
az ad user show \
  --id testuser1@simplilearnhol100744.onmicrosoft.com \
  --query id --output tsv
```

Then add the user:
```bash
az ad group member add \
  --group "LabUsersGroup" \
  --member-id <user-object-id>
```

---

## 📂 Project Structure

```
.
├── README.md
├── commands.txt        # All CLI commands used
├── notes.md            # My observations & learnings
└── screenshots/        # CLI outputs & portal verification
```

---

## 💡 What I Learned

- Identity and access management (IAM) is critical in every cloud setup
- Azure CLI provides better clarity on how actions are performed under the hood
- Errors like RBAC permission issues aren’t blockers — they’re lessons
- Following a PDF is one thing — doing it manually teaches you much more

---

