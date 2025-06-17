# 💼 Find Jobs Using Google Dorking & Social Recon

This guide focuses on how to **find jobs using advanced search techniques (Google Dorking)** and **social media-based recon**, which is a vital skill for bug bounty hunters, researchers, OSINT specialists, and job seekers.

---

## 🎯 What You'll Learn

- How to find **hidden or lesser-known job listings**
- Discover **career pages** on company websites
- Search for **internal PDF job postings**
- Explore **resume databases** to identify hiring companies
- Use **social media** like Reddit, Twitter, and LinkedIn for real-time job alerts
- Dorking methods to discover **remote jobs**, **freelance gigs**, **internships**, and **govt jobs**

---

## 🔎 1. Google Dorking for Job Listings

Google dorking helps uncover indexed but obscure job listings, portals, and downloadable offers.

### 📘 Basic Dorks

```bash
intext:"we're hiring" AND ("developer" OR "software engineer")
```
Find generic job ads with common hiring phrases.

```bash
intitle:"careers" inurl:"/jobs" AND "cybersecurity"
```
Find companies hiring for cybersecurity roles on their own portals.

```bash
filetype:pdf "job opening" OR "apply now" -site:linkedin.com
```
Target downloadable job offers, resumes, or career bulletins.

```bash
site:greenhouse.io "open position" "frontend"
```
Find job openings from Greenhouse (used by many startups).

---

## 🧑‍💻 2. Resume Recon (Job Sourcing)

Finding resumes can lead to companies hiring or networking leads.

### 🧾 Resume-Based Dorking

```bash
site:linkedin.com/in intitle:"resume" AND ("developer" OR "engineer") AND "bangalore"
```
Find public resumes of professionals in a specific region or field.

```bash
inurl:cv intitle:"resume of" filetype:pdf
```
Target open CVs/resumes stored on misconfigured servers.

```bash
intitle:"index of" "resume.doc"
```
Search for file listings exposing personal CVs — great for lead discovery.

---

## 🌍 3. Social Media Job Recon (Live Opportunities)

Real-time job openings are often shared via posts, tweets, and threads.

### 🐦 Twitter

```bash
site:twitter.com "we're hiring" "full-stack developer" "remote"
```
Look for tweets from startups or HR teams about developer roles.

```bash
site:twitter.com "join our team" ("UI designer" OR "UX") "remote"
```
Target remote-friendly UI/UX design jobs.

### 🔺 Reddit

```bash
site:reddit.com/r/forhire "looking to hire" "python developer"
```

```bash
site:reddit.com/r/remotejobs "hiring now" "javascript"
```

Look for user-to-user job leads on Reddit. Subreddits like:
- `/r/forhire`
- `/r/remotework`
- `/r/techjobs`
- `/r/cscareerquestions`

---

## 📌 4. Find Specific Types of Jobs with Targeted Dorks

| 🎯 Target Job Type | 🧪 Sample Dork |
|--------------------|----------------|
| Remote Jobs        | `intext:"100% remote" intitle:"career opportunities"` |
| Freelance          | `inurl:freelance "apply now" site:jobs.toptal.com` |
| Internships        | `intitle:"summer internship" AND ("2024" OR "current")` |
| Government Jobs    | `site:.gov filetype:pdf "job vacancy"` |
| Company Specific   | `site:careers.google.com "open roles"` |
| Country-Based      | `site:.uk intitle:"work with us"` |

---

## 🛠️ 5. Bonus Tools for Job Recon

Once you’ve identified targets, use these browser extensions or tools:

| Tool/Extension           | Purpose |
|--------------------------|---------|
| **Hunter.io**            | Get email addresses from domain |
| **ContactOut**           | Find emails of LinkedIn profiles |
| **Wappalyzer**           | Know stack before applying |
| **Google Alerts**        | Set alerts for job dork terms |
| **LinkedIn Job Filter**  | Create custom filters |
| **Glassdoor/Indeed Dork**| Use `site:glassdoor.com "hiring"` |

---

## 🎓 6. Real-World Dork Use Cases (Case Studies)

### 🧠 Case 1: Find Remote Developer Jobs

```bash
intext:"remote only" AND ("hiring" OR "job opening") filetype:pdf
```

You can find company-hosted PDFs or blogs mentioning fully remote hiring.

---

### 💼 Case 2: Freelance Tech Gigs

```bash
site:peopleperhour.com "looking for developer"
```

Use this to extract freelance offers directly from freelance platforms.

---

### 🎯 Case 3: Discover Internal Job Boards

```bash
inurl:"/careers" intitle:"we're hiring"
```

Find smaller companies' internal job pages, sometimes not listed on LinkedIn or Google Jobs.

---

## 🧭 7. Suggested Dorking Flow

```bash
# Step 1: Choose Target Role
e.g., "Python developer", "React Intern"

# Step 2: Pick Type of Job
Remote, Freelance, Internship, Country-specific

# Step 3: Apply Filtered Dorks
Use intitle, inurl, site, filetype

# Step 4: Use Social Recon
Reddit, Twitter, LinkedIn Dorking

# Step 5: Analyze Job Stack or Company
Use Wappalyzer, BuiltWith

# Step 6: Apply or Network
Email, LinkedIn, or company contact
```

---

## ⚠️ Legal Disclaimer

This guide is for **educational purposes only**. Use all information **ethically** and **legally**. Do not exploit, scrape, or automate requests against platforms that disallow it.

---

## 👨‍💻 Author

**Raghav Arora**  
GitHub: [@thatraghavarora](https://github.com/thatraghavarora)
> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*

**Repo:** [Find Anything on Internet](https://github.com/thatraghavarora/Find-Anything-on-Internet)

