# 📚 ebooks-and-study-material Dorking Guide (For Educational Use Only)

> ⚠️ This guide is only for ethical research and academic purposes — such as finding public study material, educational documents, and legally shared content.

---

## 🎯 Objective

Learn how to craft your own custom Google Dorks to find:

- Free study guides
- Textbooks
- Exam notes
- University slides & PDFs
- Publicly available eBooks
- Research papers

---

## 🧠 Understand the Target Data

### 🔹 Keywords to Use
```
ebook
study material
university notes
exam guide
question bank
textbook
syllabus
academic
course material
lecture slides
```

### 🔹 File Types
```
filetype:pdf
filetype:doc
filetype:docx
filetype:ppt
filetype:pptx
filetype:txt
filetype:xls
```

---

## 🔨 How to Make a Custom eBook Dork

### 🧪 Step-by-Step Formula

**1. Start with a keyword:**
```
"mathematics textbook"
```

**2. Add a filetype filter:**
```
"mathematics textbook" filetype:pdf
```

**3. Add Google operator like `intitle`, `inurl`, or `intext`:**
```
intitle:"mathematics textbook" filetype:pdf
inurl:ebooks filetype:pdf
intext:"free download" filetype:pdf
```

**4. Add exclusion filters for irrelevant content:**
```
intitle:"mathematics textbook" filetype:pdf -site:amazon.com -site:pinterest.com
```

---

## 📘 Example Dorks to Find Study Material

### 🔹 Subject-Specific
```
intitle:"physics notes" filetype:pdf
intext:"chemistry study material" filetype:docx
intitle:"english grammar guide" filetype:pdf
inurl:"/downloads" "biology textbook" filetype:pdf
"computer science syllabus" filetype:doc
```

### 🔹 Exam-Oriented
```
"jee question paper" filetype:pdf
"neet previous year papers" filetype:pdf
"gate cs notes" filetype:pdf
"upsc mains answers" filetype:pdf
intext:"ssc cgl study guide" filetype:pdf
```

### 🔹 School/University Study Files
```
site:.edu "introduction to programming" filetype:pdf
site:mit.edu intitle:"lecture notes" filetype:pdf
site:harvard.edu "course material" filetype:doc
site:.ac.uk intitle:"syllabus" filetype:pdf
```

### 🔹 General eBook Repositories
```
inurl:"/ebooks" filetype:pdf
inurl:"/library" filetype:pdf
intitle:"download pdf" "data structures" filetype:pdf
inurl:"/publications" filetype:pdf
"free engineering books" filetype:pdf
```

---

## 🧰 Combine With Filters

### 🔹 Year or Edition
```
"mathematics textbook 2023" filetype:pdf
"mechanical engineering notes" filetype:pdf before:2020
```

### 🔹 Author or Institution
```
"by H.C. Verma" filetype:pdf
site:stanford.edu intitle:"lecture notes"
```

---

## 🚫 Avoid Common Pitfalls

- Do **not** search for copyrighted material that is not publicly shared.
- Always add `-site:` exclusions for commercial or junk sites (e.g., `-site:amazon.com`, `-site:quora.com`)
- Stick to `.edu`, `.ac.uk`, or `.org` for academic material.

---

## 💡 Pro Tip

Use `site:drive.google.com` or `site:dropbox.com` for publicly shared files:
```
site:drive.google.com "physics notes" filetype:pdf
site:dropbox.com "math ebook" filetype:pdf
```

---

## 🧪 Try This Combo (Template)

```
("exam guide" | "university notes" | "textbook") filetype:pdf -site:amazon.com -site:pinterest.com
```

---

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*


