# 🎬 How to Make Google Dorks for Movie & Media Indexes  
**By Raghav Arora** | ⚠️ For educational use only. Do not access unauthorized content.

---

## 📘 What Is a Media Index?

A **media index** is usually an open directory exposed on a web server that lists files like movies, TV shows, or audio. These are often created accidentally by misconfigured servers.

---

## 🛠️ Google Search Operators You’ll Use

| Operator       | Use                                         |
|----------------|---------------------------------------------|
| `intitle:`     | Match page titles (like “Index of”)         |
| `inurl:`       | Match specific words in URLs                 |
| `filetype:`    | Search by file type (e.g., mkv, mp4, mp3)    |
| `-`            | Exclude specific words                      |
| `" "`          | Search exact phrases                        |

---

## 🧪 Common Patterns of Open Index Pages

- `Index of /`
- `Parent Directory`
- Directory listing pages from Apache, Nginx, etc.

---

## 🧱 Build Your Own Dork

### 🔹 Base Format
```text
intitle:"index of /" +keyword
```

### 🔹 Target File Extensions
```text
intitle:"index of /" (mp4 | mkv | avi | flac | mp3)
```

### 🔹 Exclude Irrelevant Stuff
```text
intitle:"index of /" (mp4 | mkv) -html -php -asp
```

---

## 🧠 Example Dorks

### 🎥 General Movie Index
```text
intitle:"index of /" (mp4 | mkv | avi) inurl:movies
```

### 📺 TV Series Index
```text
intitle:"index of /" inurl:tv (mkv | mp4 | avi)
```

### 🎵 Music/Audio Index
```text
intitle:"index of /" (mp3 | flac | wav) inurl:music
```

### 🎞️ Bollywood or Hindi Movies
```text
intitle:"index of /" (mkv | mp4) inurl:hindi
```

### 🍿 Anime Content
```text
intitle:"index of /" (mp4 | mkv) inurl:anime
```

### 📁 Only Large Media Files (by size in KB/MB)
```text
intitle:"index of /" +last modified +parent directory -html -php (mkv | mp4)
```

---

## 🧩 Tips for Better Results

- Use `site:` to target or avoid specific domains.
  ```text
  intitle:"index of /" mkv -site:youtube.com
  ```
- Use wildcards like `*` in URL matching.
  ```text
  inurl:*movies* intitle:"index of /" mp4
  ```

---

## ⚠️ Legal Disclaimer

Accessing or downloading copyrighted or unauthorized content without permission is **illegal**. Use this information for learning about **OSINT, misconfigurations, and indexing behavior** only.

---

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*

