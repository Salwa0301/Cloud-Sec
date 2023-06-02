---
title: "Exploiting Security Vulnerabilities"
date: 2023-06-02T11:59:34+01:00
---
Create code that can automatically exploit its documented vulnerabilities.

##Introduction
There were many aspects to this challenge. First using the Gruyere website along with extra reading, I familiarised myself with common vunerabilities that hackers exploit such as XSS/ CSRF. It was interesting to learn how for example hackers can use authentication such as cookies or the sneaky codes they nest into scripts. 

## H2 Hugo
One of the intial tasks I had completed was installing Hugo. Using the gohugo website, I built Hugo from source whereby I had installed Git, Go and updated my PATH environment variable. With several attempts of updating the system variable, I was able to finally generate my hugo site.It was great exploring this tool as I was able to create a website with minimal complexity and due to its static nature, I didn't need to worry about server side processing or databases to generate web pages.

CI automation using GH actions
CI automation is a process that streamlines the process of integrating code changes made to a shared repository (so improves collaboration) and verifying its correctness. I achieved CI automation by using Git Hub actions whereby I created a job. This job was important in automatically updating my hugo site anytime I made any changes. I can now observe the power of CI automation- not only does it allow for multiple developers to work on a project colloboratively but also detects any issues and thus reduces the likelihood of bugs.




