# 🛡️ vulnerable-servers-and-CVEs Dorking Guide (For Legal & Educational Use Only)

> ⚠️ This guide is strictly for educational, research, and legal security testing purposes only. Unauthorized access is illegal and unethical.

---

## 🎯 Objective

Learn how to **create your own custom Google Dorks** to identify:

* Vulnerable servers
* Exposed software versions
* Unpatched systems
* Publicly indexed CVEs (Common Vulnerabilities and Exposures)
* Misconfigured services

---

## 🧠 Understand What to Search For

### 🔍 Target Elements

```
Apache/2.2.15
nginx/1.10.3
OpenSSH_7.2p2
phpMyAdmin
Index of /
server status
config file
.env

CVE-2021-XXXXX
CVE-2023-XXXXX
exploit
login page
vulnerable software
"powered by"
```

### 📄 File Types (often leaked or exposed)

```
filetype:conf
filetype:xml
filetype:env
filetype:ini
filetype:log
filetype:txt
filetype:bak
filetype:zip
filetype:sql
```

---

## 🔨 Build Custom Dorks

### 🔹 1. Discover Software Versions

```
intitle:"index of /" "Apache/2.2.15"
intitle:"phpinfo()" "PHP Version 5.6"
"Server: nginx/1.10.3" inurl:status
intext:"X-Powered-By: ASP.NET"
"powered by" "vulnerable-app"
```

### 🔹 2. Search by CVE

```
intitle:"CVE-2022" filetype:txt
intext:"CVE-2023-" filetype:log
inurl:exploit intext:"CVE-2021-"
intitle:"CVE" site:github.com
intext:"cve" site:exploit-db.com
```

### 🔹 3. Exposed Config Files

```
filetype:env DB_PASSWORD
filetype:xml "password"
filetype:conf "admin"
filetype:ini "sql"
filetype:log "error"
filetype:txt "root"
filetype:bak inurl:wp-config
```

### 🔹 4. Admin or Login Panels

```
inurl:admin/login
intitle:"admin panel"
inurl:wp-admin
inurl:phpmyadmin
inurl:login.jsp
intitle:"dashboard login"
```

### 🔹 5. Database or Backup Files

```
inurl:backup filetype:zip
inurl:dump filetype:sql
filetype:sql "insert into"
filetype:db "users"
filetype:bak "admin"
```

---

## 🧱 Combine With Filters

### 🔹 Domain Specific

```
site:example.com inurl:admin
site:.edu filetype:sql
site:.gov intext:"CVE"
```

### 🔹 Technology Stack Filtering

```
"Apache/2.4" inurl:status
"PHP/5.4" filetype:php
"nginx" intitle:"index of /"
```

---

## ⚙️ Advanced Operators

| Operator    | Use Example               | Description                    |
| ----------- | ------------------------- | ------------------------------ |
| `intitle:`  | `intitle:"Apache Status"` | Title contains this text       |
| `intext:`   | `intext:"CVE-2023"`       | Body text contains             |
| `inurl:`    | `inurl:admin`             | URL contains keyword           |
| `filetype:` | `filetype:env`            | Search specific document types |
| `site:`     | `site:example.com`        | Limit to a specific site       |
| `-site:`    | `-site:github.com`        | Exclude site                   |
| `*`         | `intitle:*admin*`         | Wildcard match                 |

---

## ✅ Use Cases

| Dork                         | Purpose                    |
| ---------------------------- | -------------------------- |
| `filetype:env DB_PASSWORD`   | Exposed environment files  |
| `intitle:"phpinfo()"`        | PHP version disclosure     |
| `filetype:conf apache`       | Apache configuration leaks |
| `filetype:sql "INSERT INTO"` | Raw database dumps         |
| `intitle:"CVE" filetype:log` | CVE reports in logs        |

---

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*

---
