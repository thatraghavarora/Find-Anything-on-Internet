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

## 💯 100+ Ready-to-Use Customer Leads & Emails Dorks

```
filetype:csv intext:@gmail.com
filetype:xlsx intext:@yahoo.com
filetype:xls intext:"email, phone"
filetype:txt "client email"
inurl:leads filetype:xlsx
inurl:"/contact"
intitle:"contact us"
intext:"get in touch"
site:company.com inurl:contact
intitle:"get in touch" site:.edu
site:linkedin.com/in intitle:"marketing manager"
site:crunchbase.com intitle:"SaaS" "contact email"
"client list" filetype:pdf
filetype:xlsx intext:"client name" intext:"email"
filetype:csv intext:"first name,last name,email"
inurl:"/uploads" filetype:xlsx
filetype:xlsx intext:"leads" intext:"email"
filetype:xlsx intext:@gmail.com "New York"
filetype:csv intext:"Los Angeles" intext:"clients"
filetype:csv intext:"marketing agency" intext:"email"
filetype:pdf intext:"real estate clients"
intext:@company.com filetype:xls
filetype:csv "@gmail.com" -site:facebook.com
filetype:docx intext:@hotmail.com
filetype:pdf intext:"email list"
filetype:xlsx intext:"newsletter subscribers"
filetype:xls intext:"customer contact"
filetype:csv intext:@outlook.com
filetype:txt "email, name"
filetype:doc intext:@protonmail.com
filetype:csv intext:"email|name"
filetype:pdf intext:"client database"
filetype:xlsx intext:"sales leads"
filetype:xls intext:"email addresses"
filetype:txt intext:"mailing list"
filetype:csv intext:"prospective clients"
filetype:doc intext:"emails" intext:"clients"
filetype:docx intext:"client email list"
filetype:pdf intext:"email directory"
filetype:csv intext:@live.com
filetype:txt intext:@aol.com
filetype:xls intext:"email" intext:"location"
filetype:csv intext:@icloud.com
filetype:pdf intext:@zoho.com
filetype:xlsx intext:"contact info"
filetype:xls intext:"contact list"
filetype:csv intext:"business contacts"
filetype:xlsx intext:"outreach list"
filetype:doc intext:"sales contacts"
filetype:pdf intext:"marketing list"
filetype:csv intext:"hr contacts"
filetype:xlsx intext:"vendor email"
filetype:pdf intext:"alumni emails"
filetype:xls intext:"investor contacts"
filetype:csv intext:"partner list"
filetype:txt intext:"phone email"
filetype:csv intext:"email directory"
filetype:doc intext:"newsletter emails"
filetype:xlsx intext:"webinar attendees"
filetype:csv intext:"job applicants"
filetype:xlsx intext:"conference attendees"
filetype:pdf intext:"organization email"
filetype:csv intext:"event registrants"
filetype:csv intext:"ticket buyers"
filetype:xls intext:"support emails"
filetype:doc intext:"purchase leads"
filetype:csv intext:"community members"
filetype:xlsx intext:"registered users"
filetype:txt intext:"freelancer email"
filetype:xls intext:"service providers"
filetype:csv intext:"NGO email list"
filetype:pdf intext:"committee emails"
filetype:csv intext:"school email list"
filetype:xlsx intext:"student contacts"
filetype:csv intext:"teacher contacts"
filetype:doc intext:"parent email"
filetype:csv intext:"hospital staff email"
filetype:xls intext:"clinic email list"
filetype:xlsx intext:"gov contact email"
filetype:csv intext:"city council email"
filetype:docx intext:"municipal contacts"
filetype:pdf intext:"media contact list"
filetype:csv intext:"press contact"
filetype:xlsx intext:"marketing contacts"
filetype:pdf intext:"pr email"
filetype:csv intext:"church email list"
filetype:xlsx intext:"volunteer list"
filetype:doc intext:"temple email"
filetype:pdf intext:"mosque contacts"
filetype:csv intext:"sports club email"
filetype:xls intext:"gym contact list"
filetype:xlsx intext:"event planners email"
filetype:csv intext:"birthday organizer"
filetype:txt intext:"email, twitter"
filetype:csv intext:"email, linkedin"
filetype:doc intext:"name, email"
filetype:xls intext:"website, email"
filetype:csv intext:"sales contact"
filetype:xlsx intext:"channel partner email"
filetype:docx intext:"distributor email"
filetype:xlsx intext:"startup email list"
filetype:csv intext:"accelerator contact"
filetype:doc intext:"incubator email"
```

---

## 🔐 Disclaimer

This is for **educational & ethical research only**. Never use this data for spam, scams, or unlawful activity.

---
> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
