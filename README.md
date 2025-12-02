# js-security-keywords

# 🔍 Top Key Points to Search in JavaScript Files  
### For Code Review, Security Audit & Sensitive Data Detection  
**By: Virendra Kumar  
Company:- Cyber Leelawat**  
🌐 https://cyberleelawat.vercel.app/

---

## 1. API Keys / Secrets

Look for exposed credentials, environment variables, or hardcoded secrets:

```
REACT_APP_
API_KEY
SECRET_KEY
ACCESS_TOKEN
AUTH_TOKEN
JWT
BEARER
client_secret
client_id
aws_access_key_id
aws_secret_access_key
firebaseConfig
google_api_key
stripe_public_key
```

---

## 2. Endpoints & URLs

Check for internal API routes, GraphQL endpoints, or sensitive URLs:

```
apiUrl
baseUrl
endpoint
.graphql
.json
/v1/
/auth/
appsync
cognito
```

---

## 3. Developer & Build Information

Useful for understanding the environment setup and debugging:

```
package.json
scripts
webpack
env
NODE_ENV
process.env
debug=true
loglevel
```

---

## 4. Authentication / Auth Flow

Common functions and variables used in login/auth systems:

```
login()
logout()
authHeader
Authorization
Bearer
JWT.decode
getToken()
setToken
```

---

## 5. Cloud Services Usage

Indicators of cloud platform usage or misconfigurations:

```
aws
gcp
firebase
s3.amazonaws.com
bucket
cloudfront
amplify
appsync
cognito
```

---

## 6. Payment Integrations

Payment gateway references or public/test keys:

```
stripe
paypal
razorpay
public_key
merchant_id
```

---

## 7. Security / Misconfigurations

Potential vulnerabilities and insecure practices:

```
cors
headers.set('Access-Control-Allow-Origin'
x-api-key
authToken
adminToken
```

## ⚠️ Security Note

If any of these patterns appear inside JavaScript files, it may indicate:

- Sensitive data exposure  
- Credential leakage  
- Hardcoded secrets  
- API or authentication misconfigurations  
- Cloud misconfigurations  

---

## ✨ Created by **Virendra Kumar**  
🌐 https://cyberleelawat.vercel.app/  
Web Security | Bug Bounty | Cyber Researcher
