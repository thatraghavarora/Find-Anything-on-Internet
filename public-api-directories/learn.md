# 🔍 public-api-directories Dorking Guide (By Raghav Arora)

> ⚠️ For **educational and legal** research only. Do not misuse this information.

---

## 🎯 Objective

Learn to create your own **Google Dorks** to discover:
- Publicly exposed API directories
- Open Swagger / Postman / REST interfaces
- Misconfigured API endpoints
- API documentation meant for internal use
- Potential API leakages on GitHub or web servers

---

## 🧠 Step 1: Understand What You’re Looking For

### 🔹 Common Keywords
```
swagger
api-docs
rest-api
openapi
api/v1/
graphql
postman
.json
.yaml
```

### 🔹 Common API Doc Patterns
- `/swagger.json`
- `/swagger-ui.html`
- `/openapi.yaml`
- `/api-docs/`
- `/v1/docs`
- `/v2/docs`
- `?format=openapi`
- `intitle:Swagger`
- `inurl:api-docs`

---

## 🧩 Step 2: Build Custom Google Dorks

### 🔹 Swagger UI or OpenAPI Interfaces
```
intitle:"Swagger UI" inurl:swagger
inurl:"swagger.json" filetype:json
inurl:"openapi.yaml" filetype:yaml
inurl:"api-docs"
```

### 🔹 Public Postman Collections
```
site:postman.com "view collection"
inurl:postman "collection"
"exported with Postman" filetype:json
```

### 🔹 Open REST Endpoints
```
inurl:"/api/v1/" -github
inurl:"/api/v2/" intitle:"API"
inurl:"/rest/api/"
```

---

## 🧠 Step 3: Add Filters

### 🔹 Technology Filters
```
intext:"Express API" filetype:json
intext:"FastAPI" inurl:docs
intext:"GraphQL Playground" intitle:"API"
```

### 🔹 Domain Specific
```
site:company.com inurl:swagger
site:*.gov.in inurl:openapi
site:*.edu intitle:"API Docs"
```

---

## 🛠️ Step 4: Advanced Combinations

```
filetype:json inurl:swagger -site:github.com
filetype:yaml "openapi" intext:"paths"
intitle:"API Reference" inurl:docs
"public api" inurl:/docs filetype:html
```

---

## 🧪 Step 5: What to Do When You Find One

1. Open the Swagger/OpenAPI URL in browser.
2. Look at available endpoints (GET/POST/PUT/DELETE).
3. Verify if authentication is needed or not.
4. Never send malicious payloads — keep it ethical.
5. Document everything.

---

## 📌 Tips for Making Your Own Dork

- Start with a known pattern: `/swagger.json`, `/api/v1/`
- Add `filetype:json` or `filetype:yaml`
- Add keyword like `intext:"paths"` or `intext:"info"`
- Exclude noise with `-site:github.com` or `-site:swagger.io`
- Filter by domain with `site:example.com`

---

## 🏁 Summary Example Custom Dorks

```text
inurl:swagger filetype:json
inurl:api-docs intitle:"API"
filetype:yaml intext:"openapi" inurl:/docs
site:*.gov inurl:openapi
site:*.edu filetype:json "swagger"
```

---

> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
