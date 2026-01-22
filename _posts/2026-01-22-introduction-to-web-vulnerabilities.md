---
layout: post
title: "Introduction to Web Vulnerabilities"
date: 2026-01-22
categories: [web-development]
tags: [sql-injection, security]
---

Web applications are widely used today, but they are often vulnerable if proper security measures are not implemented.

## SQL Injection

SQL Injection occurs when an attacker manipulates database queries by inserting malicious SQL through input fields.

### Example

```sql
SELECT * FROM users
WHERE username = 'input'
AND password = 'input';
