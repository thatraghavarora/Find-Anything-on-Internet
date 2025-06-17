# 🐞 Bug Bounty Program Finder (Using Google Dorks)

Quick guide to find bug bounty programs using Google Dorks. This teaches how to build your own dorks to search for hidden or public bounty pages.

---

## 🔧 Build Your Own Dork — 3 Simple Steps

### ✅ 1. Choose What You Want to Find:

- Bug bounty policy
- Responsible disclosure pages
- HackerOne/Intigriti/Security pages
- Private program leaks
- Scope URLs (subdomains, etc.)

---

### ✅ 2. Combine Keywords + Operators

#### 🧱 Keywords:
- `bug bounty`
- `responsible disclosure`
- `security.txt`
- `report vulnerability`
- `rewards`
- `hackerone.com`, `intigriti.com`, `bugcrowd.com`

#### 🔍 Useful Google Operators:
- `site:`
- `inurl:`
- `intitle:`
- `intext:`
- `filetype:`

---

### ✅ 3. Start Building Dorks

#### 🔹 Find Bounty Policy Pages:
```bash
intext:"bug bounty program" site:.com
intitle:"report a vulnerability" site:.gov
intext:"responsible disclosure policy" site:.org
```

#### 🔹 Get HackerOne/Intigriti Hosted Programs:
```bash
site:hackerone.com inurl:reports
site:intigriti.com inurl:programs
```

#### 🔹 Search for Security Pages:
```bash
intitle:"security" inurl:security site:*.com
inurl:"/security" "report vulnerability"
```

#### 🔹 Find `security.txt` Files:
```bash
inurl:".well-known/security.txt" -github
```

#### 🔹 Public Programs with Scope URLs:
```bash
site:bugcrowd.com intext:"target scope"
site:hackerone.com intitle:"domains"
```

---

## 💡 Combine Smart Filters

#### 🔸 Specific Industry:
```bash
intext:"bug bounty" site:*.edu
intext:"responsible disclosure" site:*.gov
```

#### 🔸 Exclude Irrelevant:
```bash
intext:"security" -site:github.com -site:linkedin.com
```

#### 🔸 Look for PDF Disclosures:
```bash
filetype:pdf "bug bounty program"
```

---

## 🎯 Tips to Go Further

- Look at `/security`, `/bug-bounty`, `/vulnerability-disclosure` URLs
- Search program leaks on Pastebin, GitHub Gists, or archives
- Use `cache:` to view removed bounty pages
- Track companies with HackerOne/Intigriti profiles but no links
- Hunt on startups via AngelList/Crunchbase with dorks like:
```bash
intitle:"security" site:*.tech
```

---

## 📁 Examples to Try Right Now

```bash
inurl:"/security" "report bug" site:.co
intitle:"bug bounty" site:*.ai
inurl:"/bug-bounty" filetype:pdf
intitle:"responsible disclosure" inurl:security site:*.cloud
```

---

## 📌 Output Goals

- List of bounty programs
- Scope discovery
- Hidden security.txt or program URLs
- Reporting methods & rewards

---

## 🛠️ Recommended Next Step

Once you find a program:

1. Collect domains and subdomains
2. Feed into recon tools (`subfinder`, `httpx`)
3. Start scanning for low-hanging bugs (CORS, open redirect, JS leaks, etc.)

---

> 👨‍💻 Maintained in `Find-Anything-on-Internet` by [@thatraghavarora](https://github.com/thatraghavarora)
> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
