---
title: "Introduction to Web Vulnerabilities"
date: 2026-01-22
categories: [web-development]
tags: [SQL injection, security]
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

---

### **Post 2 — XSS**

**File:** `_posts/2026-01-23-cross-site-scripting.md`

```markdown
---
title: "Introduction to Cross-Site Scripting (XSS)"
date: 2026-01-23
categories: [web-development]
tags: [XSS, security]
layout: post
---

Cross-Site Scripting (XSS) is a common web vulnerability where attackers inject malicious scripts into web pages that other users view. XSS can steal sensitive data, hijack user sessions, or manipulate website content.

## Types of XSS

1. **Stored XSS**  
   Malicious scripts are stored on the server (e.g., in a database) and executed whenever users view the affected page.

2. **Reflected XSS**  
   Scripts are sent via URLs or form inputs and immediately reflected back by the server.  

3. **DOM-Based XSS**  
   Scripts manipulate the Document Object Model (DOM) on the client side without involving the server.

## Example

If a comment form does not sanitize input:

```html
<script>alert('XSS attack');</script>

---

###  Key Changes for Chirpy Compatibility

1. `layout: post` added → ensures Chirpy renders it correctly.  
2. `categories` are **lowercase with hyphens** → needed for category pages.  
3. `tags` are lowercase → needed for tag pages.  
4. Properly closed code blocks.  
5. Markdown headings are consistent.  

---

###  Steps to Make Them Show

1. Copy these two files into your `_posts` folder.  
2. Run locally (optional but recommended):

```bash
bundle exec jekyll serve
