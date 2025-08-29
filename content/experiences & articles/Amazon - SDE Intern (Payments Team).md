---
title: 1. Amazon Summer 2025
draft: false
tags:
  - work
  - internship
  - Experiences
---
> **Role**: SDE Intern
> 
> **Team**: Payments (Amazon STORES)

### RPS Orchestration
I worked on the recurring payments subscriptions team, our main client is Amazon Prime and we handle the storage and creation of recurring payment contracts.
Previously, upstream clients were responsible for orchestrating customer authentication with via Amazon internal endpoints. Instead of having the clients make a ton of api calls to different endpoints and have to poll the authentication resource, I created a new orchestration layer to handle all of it. This also allows for the mandate generation process to be asynchronous instead of waiting on authentication, which reduces latency in the checkout process.

### ⚙️Tech Stack
- [ ] AWS
	- [ ] Lambdas
	- [ ] DynamoDB
	- [ ] SNS
	- [ ] SQS
	- [ ] CloudWatch
	- [ ] CDK
- [ ] ORCA (Amazon internal equivalent of step functions)
- [ ] Java
- [ ] Typescript