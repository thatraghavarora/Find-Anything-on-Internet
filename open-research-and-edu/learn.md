# 🎓 How to Make Google Dorks to Find Open Research & Educational Material

> ⚠️ For educational and legal use only. Use ethically and responsibly.

---

## 🔧 Basic Building Blocks of a Dork

You’ll combine **Google Search Operators** with **targeted keywords** to build custom search queries.

| Operator       | Purpose                                                  |
|----------------|----------------------------------------------------------|
| `site:`        | Restrict results to specific sites or domains            |
| `filetype:`    | Search for specific document types (pdf, doc, ppt, etc.) |
| `inurl:`       | Match keywords in the URL                                |
| `intitle:`     | Match keywords in the title of the page                  |
| `intext:`      | Match keywords in the body text                          |
| `allintext:`   | Match all given keywords in the body text                |
| `allintitle:`  | Match all given keywords in the title                    |
| `allinurl:`    | Match all given keywords in the URL                      |

---

## 🎯 Targeting Academic & Research Content

To find open research and educational content, target:

- **Academic domains** like `.edu`, `.ac.uk`, `.edu.in`
- **Government and research portals**: `.gov`, `.org`, `researchgate.net`, `ieee.org`, `arxiv.org`, etc.
- **Document types**: `pdf`, `ppt`, `doc`, `docx`, `xls`

---

## 🧪 Sample Keywords

Use relevant academic/research-related keywords:

- `research paper`
- `thesis`
- `journal`
- `conference proceedings`
- `project report`
- `whitepaper`
- `course notes`
- `lectures`
- `assignments`

---

## 🛠️ Dork Creation Examples

### 🎓 Find academic papers on AI from university sites
```text
site:.edu filetype:pdf intitle:"artificial intelligence"
```

### 🧪 Search for open-access thesis documents
```text
site:.ac.uk filetype:pdf intitle:"thesis"
```

### 📄 Discover research papers on cybersecurity
```text
filetype:pdf intext:"cybersecurity" (site:arxiv.org | site:ieee.org)
```

### 🧠 Lecture notes or slides
```text
filetype:ppt site:.edu inurl:slides intitle:"lecture"
```

### 📝 Machine Learning course material
```text
filetype:pdf inurl:ml intitle:"machine learning" site:.edu
```

### 🧾 Government or institutional reports
```text
site:.gov filetype:pdf intext:"annual report"
```

---

## 💡 Tips for Custom Dork Building

* Combine multiple operators for precision.
* Use `OR` and parentheses for flexible results:
  ```text
  site:.edu OR site:.ac.uk filetype:pdf intext:"deep learning"
  ```
* Filter with `-` to exclude irrelevant content:
  ```text
  site:.edu filetype:pdf intitle:"project report" -"high school"
  ```

---

## ✅ Final Advice

* Try different variations of your keywords.
* Combine operators smartly.
* Stick to legal, educational, and ethical use only.

---

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
