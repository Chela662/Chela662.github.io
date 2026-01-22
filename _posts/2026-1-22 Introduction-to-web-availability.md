---
title: "Introduction to Web Vulnerabilities"
date: 2026-01-22
categories: [Web development]
tags: [SQL injection]
---

Web applications are widely used today, but they are often vulnerable if proper security measures are not implemented. Understanding common web vulnerabilities is crucial for building secure applications.

### SQL Injection

SQL Injection occurs when an attacker manipulates database queries by inserting malicious SQL through input fields.

**Example:**

```sql
SELECT * FROM users WHERE username = 'input' AND password = 'input';
