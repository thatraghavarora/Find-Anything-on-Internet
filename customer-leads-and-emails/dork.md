# 🌟 customer-leads-and-emails Dorking Guide (For Legal & Educational Use Only)

> ⚠️ This guide is strictly for ethical use: cybersecurity research, OSINT, academic learning, or legal marketing purposes.

---

## 📘 Objective

Learn how to **create your own custom Google Dorks** to find:

* Customer leads
* Email addresses
* CRM/contact exports
* Online contact forms
* Publicly exposed spreadsheets or documents

---

## 🧠 Understand What to Search For

### 🔹 Keywords

```
email
contact
get in touch
client
crm
lead
@domain.com
first name
last name
gmail.com
```

### 🔹 File Types

```
filetype:xls
filetype:xlsx
filetype:csv
filetype:pdf
filetype:txt
filetype:doc
filetype:docx
```

---

## 🔨 Build Custom Dorks

### 🔹 1. Leaked Email Lists

```
filetype:csv intext:@gmail.com
filetype:xlsx intext:@yahoo.com
filetype:xls intext:"email, phone"
filetype:txt "client email"
inurl:leads filetype:xlsx
```

### 🔹 2. Contact Forms / Pages

```
inurl:"/contact"
intitle:"contact us"
intext:"get in touch"
site:company.com inurl:contact
intitle:"get in touch" site:.edu
```

### 🔹 3. Industry-Specific Leads

```
site:linkedin.com/in intitle:"marketing manager"
site:crunchbase.com intitle:"SaaS" "contact email"
"client list" filetype:pdf
```

### 🔹 4. CRM or Export Files

```
filetype:xlsx intext:"client name" intext:"email"
filetype:csv intext:"first name,last name,email"
inurl:"/uploads" filetype:xlsx
filetype:xlsx intext:"leads" intext:"email"
```

---

## 🧱 Combine With Filters

### 🔹 City/Location Filtering

```
filetype:xlsx intext:@gmail.com "New York"
filetype:csv intext:"Los Angeles" intext:"clients"
```

### 🔹 Industry Filtering

```
filetype:csv intext:"marketing agency" intext:"email"
filetype:pdf intext:"real estate clients"
```

### 🔹 Domain Filtering

```
intext:@company.com filetype:xls
filetype:csv "@gmail.com" -site:facebook.com
```

---

## 🧰 Advanced Operators

| Operator    | Use Example             | Description                         |
| ----------- | ----------------------- | ----------------------------------- |
| `intitle:`  | `intitle:"client list"` | Title contains this text            |
| `intext:`   | `intext:"email, name"`  | Body text contains                  |
| `inurl:`    | `inurl:contact`         | URL contains keyword                |
| `filetype:` | `filetype:csv`          | Search specific document types      |
| `site:`     | `site:linkedin.com`     | Limit to a specific site            |
| `-site:`    | `-site:pinterest.com`   | Exclude site                        |
| `@domain`   | `@yahoo.com`            | Search for specific email providers |

---

## 📦 Example Output You Can Expect

| Dork                                       | Possible Result                   |
| ------------------------------------------ | --------------------------------- |
| `filetype:xls intext:@gmail.com`           | Customer contact spreadsheets     |
| `filetype:csv intext:"first name","email"` | CRM data exports                  |
| `inurl:contact intitle:contact us`         | Public contact forms for outreach |
| `filetype:pdf "lead list"`                 | B2B sales PDFs                    |

---

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
