# 🧠 Source Code and Repos Dorking Guide (For Educational Use Only)

> ⚠️ This guide is for cybersecurity research, OSINT learning, and ethical hacking only. Do not misuse this information.

---

## 🎯 Objective

Learn how to use Google Dorking techniques to discover publicly exposed **source code, repositories, config files, and developer traces** on the internet.

---

## 🧠 Understanding What to Look For

### 🔍 Target Keywords

```
github
bitbucket
gitlab
repo
repository
source code
.env
config
credentials
api_key
```

### 📄 File Types

```
filetype:env
filetype:xml
filetype:json
filetype:ini
filetype:txt
filetype:yaml
filetype:config
filetype:log
filetype:bak
```

### 📂 Paths and Directories

```
inurl:.git
inurl:/.env
inurl:/config
inurl:/credentials
intitle:"index of" config
intitle:"index of" .git
```

---

## 🛠️ How to Build Personal Dorks

### 1. Exposed Git Repositories

```
inurl:.git intitle:index.of
inurl:.git/HEAD
inurl:.git/config
intitle:"index of" ".git"
```

### 2. Configuration Files & Credentials

```
filetype:env "DB_PASSWORD"
filetype:ini "password="
filetype:xml "<password>"
filetype:config intext:API_KEY
filetype:json intext:"access_token"
```

### 3. Dev/Test Environments

```
intitle:"development config"
filetype:json inurl:dev
filetype:env inurl:test
inurl:dev site:github.com
```

### 4. API Keys in Repos or Logs

```
filetype:log intext:"api_key"
filetype:txt intext:"secret="
filetype:json intext:"token"
filetype:env intext:AWS_SECRET_ACCESS_KEY
```

---

## 💯 100+ Dorks for Source Code & Repos

```
inurl:"/.git/config"
inurl:"/.git/HEAD"
inurl:"/.svn/entries"
inurl:"/.hg"
inurl:"/CVS/Root"
inurl:"/config.json"
inurl:"/settings.py"
filetype:env "DB_USERNAME"
filetype:env "DB_PASSWORD"
filetype:env intext:"API_KEY"
filetype:ini intext:"password="
filetype:log intext:"mysql"
filetype:log intext:"password"
filetype:log intext:"user"
filetype:log intext:"login"
filetype:txt intext:"credentials"
filetype:xml intext:"password"
filetype:yaml intext:"access_key"
filetype:yaml intext:"secret_key"
filetype:json intext:"auth"
filetype:json intext:"key"
filetype:json intext:"private_key"
filetype:bak inurl:"backup"
filetype:bak intext:"password"
filetype:bak intext:"user"
filetype:bak intext:"config"
filetype:config intext:"username"
filetype:config intext:"password"
filetype:config intext:"token"
filetype:config intext:"secret"
filetype:txt intext:"admin"
filetype:txt intext:"ftp"
filetype:txt intext:"db"
filetype:txt intext:"ssh"
filetype:xml intext:"access"
filetype:xml intext:"secret"
filetype:xml intext:"token"
filetype:xml intext:"credential"
filetype:env intext:"GOOGLE"
filetype:env intext:"SLACK"
filetype:env intext:"SENDGRID"
filetype:env intext:"STRIPE"
filetype:env intext:"TWILIO"
filetype:env intext:"FACEBOOK"
filetype:env intext:"TWITTER"
filetype:env intext:"MAILGUN"
filetype:env intext:"MAILJET"
filetype:env intext:"MONGODB"
filetype:env intext:"REDIS"
filetype:env intext:"POSTGRES"
filetype:env intext:"MYSQL"
filetype:env intext:"SMTP"
filetype:env intext:"NO_AUTH"
filetype:env intext:"JWT"
filetype:env intext:"SECRET"
filetype:env intext:"TOKEN"
filetype:env intext:"DB_CONNECTION"
filetype:env intext:"API_SECRET"
filetype:env intext:"PRIVATE_KEY"
filetype:env intext:"SSH_KEY"
filetype:env intext:"AWS_SECRET_ACCESS_KEY"
filetype:json inurl:"firebaseio"
filetype:json intext:"project_id"
filetype:json intext:"storageBucket"
filetype:json intext:"authDomain"
filetype:json intext:"client_id"
filetype:json intext:"client_secret"
filetype:json intext:"refresh_token"
filetype:json intext:"type":"service_account"
filetype:json intext:"private_key_id"
filetype:json intext:"client_email"
filetype:json intext:"universe_domain"
filetype:json intext:"project_number"
filetype:json intext:"auth_provider_x509_cert_url"
filetype:json intext:"auth_uri"
filetype:json intext:"token_uri"
filetype:json intext:"private_key"
filetype:log inurl:"/logs/"
filetype:log inurl:"debug"
filetype:log inurl:"error"
filetype:log intext:"debug"
filetype:log intext:"trace"
filetype:log intext:"stack"
filetype:log intext:"exception"
filetype:log intext:"fail"
filetype:log intext:"warn"
filetype:log intext:"fatal"
filetype:log intext:"panic"
filetype:log intext:"caught"
filetype:log intext:"crash"
```

---

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
