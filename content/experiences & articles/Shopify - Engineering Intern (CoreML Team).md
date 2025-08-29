---
title: 2. Shopify Winter 2025
draft: false
tags:
  - work
  - internship
  - Experiences
---
> **Role**: Engineering Intern
> 
> **Team**: CoreML


### Phash
As part of adding image similarity search to Shopify, I was tasked with implementing a hashing algorithm for the images. I ran experiments using CometML using hundreds of Shopify images to figure out the best algorithm and parameters to use. This was extra tricky because of our unique requirements. For example:
1. Cropped copies of an image should be considered the same image as the original
2. Products photoshopped to be a different colour should not be considered a match
I worked with a couple different algorithms like phash, dhash, average hash, and crop-resistant hash - but eventually settled on phash.

### Sidekick Media Generation
Sidekick is Shopify's AI assistant, it can help you do things like locate settings and generate blog post ideas. I worked on adding image generation to Sidekick as part of an overarching goal of AI website generation. We used a LoRA to tune the LLM to generate images that match the Shopify brand.

### ⚙️Tech Stack
- [ ] Ruby
- [ ] Python
- [ ] GCP
- [ ] LLMs
- [ ] GraphQL