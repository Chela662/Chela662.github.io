---
title: "Introduction to Web Vulnerabilities"
date: 2026-01-22
categories: [Web development]
tags: [SQL injection]
layout: post
---

Web applications are widely used today, but many are vulnerable if proper security measures are not applied. Understanding web vulnerabilities is crucial for building secure applications and protecting users’ data.

## What are Web Vulnerabilities?

A **web vulnerability** is a weakness in a website or web application that can be exploited by attackers to perform unauthorized actions, access sensitive data, or disrupt services. Common examples include:

- SQL Injection  
- Cross-Site Scripting (XSS)  
- Cross-Site Request Forgery (CSRF)  
- Insecure authentication  
- Security misconfigurations  

In this post, we will focus on **SQL Injection**, one of the most critical vulnerabilities.

## SQL Injection

SQL Injection occurs when an attacker manipulates a website’s database query by inserting malicious SQL code into input fields. This can allow attackers to bypass authentication, read sensitive information, or modify/delete data.

### Example

Imagine a login system with this SQL query:

```sql
SELECT * FROM users
WHERE username = 'input'
AND password = 'input';
