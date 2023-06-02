---
title: "Exploiting Security Vulnerabilities"
date: 2023-06-02T11:59:34+01:00
---


## Introduction
There were many aspects to this challenge where the overarching task was '**to create code that can automatically exploit its documented vunerabilities**'. First, using the Gruyere website along with extra reading, I familiarised myself with common vunerabilities that hackers exploit such as XSS/ CSRF. It was interesting to learn how for example hackers can use authentication such as cookies or the sneaky codes they nest into scripts. 

##  Hugo
One of the intial tasks I had completed was installing Hugo. Using the gohugo website, I built Hugo from source whereby I had installed Git, Go and updated my PATH environment variable. With several attempts of updating the system variable, I was able to finally generate my hugo site. It was great exploring this tool as I was able to create a website with minimal complexity and due to its static nature, I didn't need to worry about server side processing or databases to generate web pages.

## CI automation using GH Actions
CI automation is a process that streamlines the process of integrating code changes made to a shared repository (so improves collaboration) and verifyies its correctness. I achieved CI automation by using Git Hub actions whereby I created a job. This job was important in automatically updating my hugo site anytime I made any changes. I can now observe the power of CI automation- not only does it allow for multiple developers to work on a project colloboratively but also detects any issues and thus reduces the likelihood of bugs.

## Playwright for Browser Automation Exploits
The bulk of my attention went to synthesising a python code that automates:
1. Opening of the Gruyere website
2. Clicking 'Agree and Start'
3. Clicking of the 'Sign up' button
4. Input of username and password followed by clicking the 'login' button
5. Clicking 'Choose File' which contains the payload variable/script exhibiting xss attack on opening 
6. Clicking 'Upload File' 
7. Successful uploading of the URL whereby the script 'you are hacked' would appear on the victim's screen
 
 Through a combination of inspecting elements, running pytests and defining variables, I was able to automate a process from the opening of a website to the clicking of a URL that was compromised. I initially found it difficult to observe the testing due to the sheer rapid nature and thus included a page wait time into the code. This python code can be analysed/accessed in a separate link.




