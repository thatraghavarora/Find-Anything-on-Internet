# 📷 Unsecured Public Cameras Dorking Guide (For Legal & Educational Use Only)

> ⚠️ This guide is strictly for ethical use: academic learning, cybersecurity research, and OSINT exploration only. Do NOT access or tamper with private or unauthorized feeds.

---

## 🎯 Objective

Learn how to create **custom Google Dorks** to find publicly exposed, unsecured IP/Webcams across the internet.

---

## 🧠 What Are We Looking For?

We aim to identify cameras that are:

* Exposed without login (no authentication)
* Hosted on default ports or URLs
* Indexed by Google, Shodan, or public search engines

---

## 🔑 Target Keywords and Strings

```
inurl:view/view.shtml
inurl:top.htm
inurl:axis-cgi
intitle:"Live View / - AXIS"
inurl:/mjpg/video.mjpg
inurl:/cgi-bin/guestimage.html
intitle:"IP Camera ["
inurl:/video.cgi
intitle:"WebcamXP 5"
```

---

## 🧱 Build Your Own Dork

### 🔹 Step-by-Step Example:

#### 1. Find Webcam Vendors:

Look at the URLs and interface strings of popular public webcam software like:

* Axis
* Hikvision
* Foscam
* WebcamXP
* MJPEG-streamer

#### 2. Observe Common URLs and Ports:

These may include:

* `:8080`, `:81`, `:8000`, `:8888`
* `/video`, `/video.cgi`, `/axis-cgi`, `/view.shtml`, `/snapshot.cgi`

#### 3. Craft Dork with Operators:

```text
inurl:view/index.shtml intitle:"Live Webcam"
```

Or target camera brands directly:

```text
inurl:"axis-cgi/mjpg" intitle:"Axis"
```

Combine with `-site:` to exclude known demo pages or documentation.

#### 4. Use Specific Location or ISP Targeting:

```text
intitle:"Live Cam" inurl:8080 "New York"
```

```text
inurl:"/video.cgi" -site:axis.com -site:documentation.com
```

---

## 📌 Safety & Ethics Reminder

* Do **NOT** exploit, tamper with, or make changes to any camera systems.
* View-only access does not imply authorization.
* Respect privacy and laws in your region.

---
> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
