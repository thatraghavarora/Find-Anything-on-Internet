# ☁️ Cloud & Configuration Leak Dorking  (Educational & Legal Use Only)
```
filetype:env intext:DB_PASSWORD
filetype:env intext:AWS_SECRET_ACCESS_KEY
filetype:env intext:AWS_ACCESS_KEY_ID
filetype:env intext:MAIL_PASSWORD
filetype:env intext:SECRET_KEY
filetype:env intext:DB_USERNAME
filetype:env intext:APP_KEY
filetype:env intext:PRIVATE_KEY
filetype:env intext:GCP_CREDENTIAL
filetype:env intext:S3_BUCKET
filetype:env intext:SMTP_PASSWORD

filetype:json intext:private_key
filetype:json intext:client_email
filetype:json intext:type: service_account
filetype:json intext:auth_uri
filetype:json intext:gcp
filetype:json intext:firebase
filetype:json intext:project_id
filetype:json intext:access_token
filetype:json intext:refresh_token
filetype:json intext:client_id

filetype:yaml intext:secret
filetype:yaml intext:password
filetype:yaml intext:api_key
filetype:yaml intext:access_token
filetype:yaml intext:aws_access_key_id
filetype:yaml intext:aws_secret_access_key
filetype:yaml intext:gcp_credentials

filetype:xml intext:apiKey
filetype:xml intext:clientSecret
filetype:xml intext:authToken
filetype:xml intext:s3

filetype:log intext:aws
filetype:log intext:ERROR
filetype:log intext:Exception
filetype:log intext:traceback
filetype:log intext:access_token
filetype:log intext:refresh_token
filetype:log intext:password

filetype:ini intext:password
filetype:ini intext:aws
filetype:ini intext:token

filetype:bashrc intext:export
filetype:bash_profile intext:AWS
filetype:zshrc intext:export

inurl:.env DB_PASSWORD
inurl:.env MAIL_HOST
inurl:.env DB_HOST
inurl:.env AWS_ACCESS_KEY_ID
inurl:.env AWS_SECRET_ACCESS_KEY

inurl:.git/config filetype:txt
inurl:.svn/entries filetype:txt
intitle:"index of" ".git"
intitle:"index of" ".svn"

inurl:"config.json"
inurl:"settings.json"
inurl:"config.js" intext:apiKey
inurl:"firebase.js" intext:apiKey
inurl:"appsettings.json"
inurl:"config.php" intext:password
inurl:"wp-config.php" intext:DB_PASSWORD

inurl:"/ftp" intitle:"index of"
inurl:"ftp://" intitle:"index of"
inurl:"s3.amazonaws.com"
inurl:"bucket" intitle:"index of"
intext:"bucket name" filetype:txt

inurl:"credentials.json"
inurl:"service-account.json"
inurl:"aws-credentials.csv"
inurl:"gcp-key.json"
inurl:"accessTokens.txt"
inurl:"auth_tokens.txt"

inurl:"secret.txt"
inurl:"token.txt"
inurl:"password.txt"
inurl:"auth.txt"
inurl:"db.txt"

intitle:"index of" "config"
intitle:"index of" "aws"
intitle:"index of" ".env"
intitle:"index of" "secrets"
intitle:"index of" "private"

filetype:conf inurl:"nginx"
filetype:conf inurl:"apache"
filetype:conf inurl:"cloudflare"
filetype:conf inurl:"vhost"

filetype:bak inurl:"config"
filetype:old inurl:"backup"
filetype:backup inurl:"settings"

filetype:swp inurl:config
filetype:tmp inurl:"access_key"

filetype:xls intext:"account id" intext:AWS
filetype:xls intext:"client id" intext:GCP
filetype:doc intext:"secret key"
filetype:pdf intext:"confidential" intext:"token"

inurl:"docker-compose.yml" intext:password
inurl:"Dockerfile" intext:ENV

inurl:"Jenkinsfile"
inurl:"jenkins" filetype:xml intext:"password"

inurl:"bitbucket-pipelines.yml"
inurl:"azure-pipelines.yml"
inurl:"travis.yml"
inurl:".circleci/config.yml"

filetype:txt intext:"Authorization: Bearer"
filetype:txt intext:"api_token"
filetype:txt intext:"access_token"

filetype:ps1 intext:"AWS_ACCESS_KEY_ID"
filetype:sh intext:"gcloud"
filetype:bat intext:"aws configure"

filetype:cfg intext:"s3"
filetype:cfg intext:"bucket"
filetype:cfg intext:"token"

filetype:rb intext:"Rails.application.secrets"
filetype:py intext:"google.cloud"
filetype:php intext:"define('DB_PASSWORD'"
filetype:java intext:"AWSStaticCredentialsProvider"

site:github.com inurl:"/blob/" intext:"AWS_SECRET_ACCESS_KEY"
site:bitbucket.org inurl:"/projects/" intext:"firebase"
site:gitlab.com inurl:"/blob/" intext:"access_token"

intext:"BEGIN RSA PRIVATE KEY"
intext:"BEGIN PRIVATE KEY"
intext:"Authorization: Basic"
intext:"s3_access_key"
intext:"gcloud auth login"

```
> ✍️ **Made by Raghav Arora**  
> 💬 *"Age is just a number.*  
> *You can do anything at any age."*
