# 💼 Job-Finding Google Dorks

A curated list of Google Dorks to help you find job opportunities via Google, social media, and hidden job postings.

---

## 🧠 Google Job Search Dorks

### 🔹 `intitle:"careers"`  
**Finds pages with "careers" in the title.**  
Example:  
```
intitle:"careers" site:linkedin.com
```

---

### 🔹 `inurl:"/jobs"`  
**Searches for pages where the URL contains `/jobs`.**  
Example:  
```
inurl:"/jobs" site:indeed.com
```

---

### 🔹 `intext:"we are hiring"`  
**Finds pages that mention "we are hiring".**  
Example:  
```
intext:"we are hiring" site:startup.jobs
```

---

### 🔹 `intitle:"job openings"`  
**Targets job listings or recruitment posts.**  
Example:  
```
intitle:"job openings" site:glassdoor.com
```

---

### 🔹 `filetype:pdf job openings`  
**Finds job listings in PDF format.**  
Example:  
```
filetype:pdf "job openings" "marketing"
```

---

### 🔹 `"work with us" AND site:.org`  
**Searches for non-profits or organizations hiring.**  
Example:  
```
"work with us" AND site:.org
```

---

### 🔹 `intitle:"career opportunities" AND "apply now"`  
**Find career pages where applications are open.**  
Example:  
```
intitle:"career opportunities" AND "apply now"
```

---

## 🌐 Social Media Dorking

### 🔹 `site:twitter.com "we're hiring"`  
**Finds tweets by companies actively hiring.**  
Example:  
```
site:twitter.com "we're hiring"
```

---

### 🔹 `site:linkedin.com "open position"`  
**Finds LinkedIn posts about open positions.**  
Example:  
```
site:linkedin.com "open position"
```

---

### 🔹 `site:facebook.com "job alert"`  
**Targets Facebook job alert posts.**  
Example:  
```
site:facebook.com "job alert"
```

---

## 📦 Dorks for Specific Job Types

### 🔹 `intext:"remote developer job"`  
**Find remote developer jobs listed on any site.**  
Example:  
```
intext:"remote developer job" filetype:pdf
```

---

### 🔹 `intext:"hiring graphic designer"`  
**Find companies hiring graphic designers.**  
Example:  
```
intext:"hiring graphic designer" site:dribbble.com
```

---

### 🔹 `intitle:"walk-in interview"`  
**Find pages about walk-in interviews.**  
Example:  
```
intitle:"walk-in interview" site:naukri.com
```

---

## 🛠️ Make Your Own Dork (Template)

Here’s a basic template to create your own dork:

```
intitle:"[job title]" OR intext:"[we are hiring]" site:[job site or domain]
```

Example for a backend job:

```
intitle:"backend developer" OR intext:"we are hiring backend" site:angel.co
```

---

## 🧲 Bonus: Find Jobs at Startups

### 🔹 `intitle:"careers" site:vercel.com`  
Finds the Vercel company career page. Works for any tech startup.  
Just replace `vercel.com` with any company domain.

---

## 🧠 Tip: Use Quotes Smartly

- `"full stack developer"` = exact match
- `full stack developer` = any order, more results

---

## 📌 Use Cases

- Job hunting without recruiters  
- Finding unlisted openings  
- Discovering PDFs and offline postings  
- Finding hiring posts on Twitter & LinkedIn  

---

## 🧑‍💻 Maintained by

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*

> For: [Find Anything on Internet](https://github.com/thatraghavarora/Find-Anything-on-Internet)

