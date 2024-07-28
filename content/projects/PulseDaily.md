---
title: PulseDaily
draft: false
tags:
  - Projects
  - Electron
  - API
  - React
  - AWS
  - Lambda
  - RDS
  - SQL
---

## [React Dashboard Video](https://youtu.be/QtoI7eBz6yE)

## [Electron Desktop App Video](https://youtu.be/lrO7QD9M6UA)

##### [Check out the website for our company here: https://pulsedaily.org/](https://pulsedaily.org/)
(Also built by me :D)

---
## 🫀 Inspiration
During the NH Innovation Challenge, we noticed that employee retention was a huge issue for many hospitals, with attrition rates ranging from 5% to 50%. PulseDaily provides a safe environment for healthcare worker to have an anonymous voice and an easy interface for management to take action.
##### [Read our planning doc](https://docs.google.com/document/d/1_ZGC9LbGSz3Pwx8CFWPhTFH2Z5hUbEQZReuaLfO3hLc/edit?usp=sharing)

## 🔍  What it does
After PulseDaily's desktop application has been installed on an employee's computer, it will pop up everyday with a new survey question. Employee responses are aggregated and stored in a MySQL database via AWS RDS. 

The administrator, manager, or higher-up can access and sign into PulseDaily's React dashboard to discover a user-friendly data visualization of employee responses over time. The dashboard also displays response rates, employee rating breakdowns, and more.

In the future we plan to add on AI recommendations to deliver actionable insights and pattern prediction to better understand employee needs. 

---
## 🔨  How I built it

PulseDaily consists of three main parts:
- **Backend** --> built with Python, SQL, AWS Lambda, RDS, EC2, API Gateway, QuickSight (first iteration)
- **Desktop app** (.msi) --> built with Electron (Electron forge)
- **Dashboard web app** --> built with React, HTML, CSS, JS

Every single one of those skills are new to me (I learnt them via PulseDaily), with the exception of HTML, CSS, Python, and SQL.
##### [Check out the react dashboard code here](https://github.com/arielycliu/pulsedailydemo/tree/master/ReactApp/frontend)
##### [Check out the electron desktop app code here](https://github.com/arielycliu/pulsedaily_desktopapp)


![[Pasted image 20240727233723.png]]

![[Pasted image 20240727233756.png]]
![[Pasted image 20240727233806.png]]
![[Pasted image 20240727233814.png]]