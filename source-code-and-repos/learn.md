# 🧠 Source Code and Repos Dorking Guide (For Legal & Educational Use Only)

> ⚠️ Created by **Raghav Arora**
>
> This guide is intended strictly for **educational**, **ethical hacking**, **bug bounty**, and **OSINT research** purposes.

---

## 🎯 Objective

Teach how to make your **own personal Google Dorks** to find publicly exposed source code, repositories, configuration files, and developer mistakes.

---

## 🔎 What We're Looking For

### 📂 Common File Types

```
filetype:env
filetype:log
filetype:xml
filetype:json
filetype:yaml
filetype:conf
filetype:config
filetype:ini
filetype:php
filetype:js
filetype:py
filetype:rb
filetype:go
filetype:java
filetype:sql
filetype:txt
```

### 🔑 Common Keywords

```
password
username
api_key
access_token
secret
smtp
ftp
AWS_ACCESS_KEY
DB_HOST
DB_PASSWORD
private_key
"BEGIN RSA PRIVATE KEY"
config
.env
settings
credentials
connectionString
client_secret
```

---

## 🏗️ Build Custom Dorks

### 🔹 Exposed Source Code Files

```
filetype:php intext:"DB_PASSWORD"
filetype:env intext:"DB_HOST"
filetype:xml intext:"<password>"
filetype:json intext:"access_token"
filetype:yaml intext:"secret:"
filetype:ini intext:"password"
filetype:txt intext:"api_key"
```

### 🔹 Git Repository Disclosures

```
inurl:.git/config
intitle:index.of ".git"
inurl:/repo filetype:zip
inurl:git filetype:sql
intitle:"index of" .git
inurl:.git/HEAD
```

### 🔹 AWS Keys / Tokens / Secrets

```
filetype:json intext:"AWS_SECRET_ACCESS_KEY"
filetype:env intext:"AWS_ACCESS_KEY_ID"
filetype:yaml intext:"aws_secret"
filetype:ini intext:"aws_access_key"
filetype:txt intext:"aws_access_key_id"
```

### 🔹 Public Config Files

```
filetype:conf intext:"password"
filetype:config intext:"host"
filetype:ini intext:"user"
filetype:txt intext:"ftp"
filetype:env intext:"MAIL_HOST"
filetype:yaml intext:"smtp:"
```

### 🔹 Database Credentials

```
filetype:env intext:"DB_PASSWORD"
filetype:xml intext:"<user>" intext:"<password>"
filetype:json intext:"db_user"
filetype:conf intext:"database"
filetype:sql intext:"insert into users"
```

### 🔹 API Key Leaks

```
filetype:js intext:"api_key"
filetype:py intext:"client_secret"
filetype:rb intext:"access_token"
filetype:go intext:"apikey"
```

---

## 💡 Combine Filters

### 🔹 Limit to Specific Domains

```
site:github.com filetype:env
site:gitlab.com intext:"api_key"
```

### 🔹 Exclude Certain Sources

```
filetype:env intext:"DB_HOST" -site:github.com
filetype:json intext:"token" -site:bitbucket.org
```

---

## 📋 Table: Custom Dorking Strategy

| Dork Example                        | Purpose                       |
| ----------------------------------- | ----------------------------- |
| `filetype:env intext:password`      | Exposed environment variables |
| `inurl:.git/config`                 | Public Git folder exposure    |
| `filetype:yaml intext:smtp`         | SMTP credentials              |
| `filetype:json intext:access_token` | Leaked tokens                 |
| `intitle:index.of .git`             | Misconfigured repos           |

---

## 🔐 Disclaimer

These dorks are only for **defensive security, auditing, bug bounty, and OSINT**. Unauthorized exploitation of systems/data is illegal.

---

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
