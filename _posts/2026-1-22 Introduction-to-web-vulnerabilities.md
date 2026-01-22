---
title: "Introduction to Web Vulnerabilities"
date: 2026-01-22
categories: [web-development]
tags: [sql-injection, security]
layout: post
---

Web applications are widely used today, but they are often vulnerable if proper security measures are not implemented. Understanding common web vulnerabilities is crucial for building secure applications.

## SQL Injection

SQL Injection occurs when an attacker manipulates database queries by inserting malicious SQL through input fields.

### Example

```sql
SELECT * FROM users
WHERE username = 'input'
AND password = 'input';
' OR '1'='1

---

### **Post 2 — Cross-Site Scripting (XSS)**

**File:** `_posts/2026-01-23-cross-site-scripting.md`

```markdown
---
title: "Introduction to Cross-Site Scripting (XSS)"
date: 2026-01-23
categories: [web-development]
tags: [xss, security]
layout: post
---

Cross-Site Scripting (XSS) is a common web vulnerability where attackers inject malicious scripts into web pages that other users view. XSS can steal sensitive data, hijack user sessions, or manipulate website content.

## Types of XSS

1. **Stored XSS** — Malicious scripts stored on the server and executed when users view the page.  
2. **Reflected XSS** — Scripts sent via URLs or forms and reflected back immediately.  
3. **DOM-Based XSS** — Scripts manipulate the DOM on the client side without involving the server.

## Example

If a comment form does not sanitize input:

```html
<script>alert('XSS attack');</script>

---

### **Post 3 — Cross-Site Request Forgery (CSRF)**

**File:** `_posts/2026-01-24-cross-site-request-forgery.md`

```markdown
---
title: "Introduction to Cross-Site Request Forgery (CSRF)"
date: 2026-01-24
categories: [web-development]
tags: [csrf, security]
layout: post
---

Cross-Site Request Forgery (CSRF) is a vulnerability that tricks a logged-in user into performing unwanted actions on a web application without their consent.

## Example

A malicious website can create a hidden form that submits a request to a bank transfer page:

```html
<form action="https://bank.com/transfer" method="POST">
  <input type="hidden" name="amount" value="1000">
  <input type="hidden" name="to" value="attacker-account">
</form>
<script>document.forms[0].submit();</script>

---

### ✅ Instructions to make it live

1. Create `_posts` folder in your project root.  
2. Copy these three files exactly as named.  
3. Run locally to test:

```bash
bundle exec jekyll serve
