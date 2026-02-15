# Hey, I'm Uzair Ahmed

Full-stack engineer who builds production systems — not just prototypes. I work across the stack from React/Next.js frontends to Node.js and FastAPI backends, with a focus on systems that handle real business complexity: workflow engines, ML classification pipelines, voice AI agents, and IoT device management.

Most of my work involves figuring out how to make different systems talk to each other cleanly — whether that's connecting a CLIP-based document classifier to a FastAPI backend as a separate microservice, building a voice agent that scrapes flight data in real-time through a browser pool, or designing a complaint routing engine with multi-stage workflows and automated escalation.

## What I work with

**Languages:** JavaScript, TypeScript, Python, Java

**Frontend:** React, Next.js (App Router), Tailwind CSS

**Backend:** Node.js, Express, FastAPI, REST APIs

**Databases:** MongoDB, PostgreSQL (Neon), Prisma, SQLAlchemy, Mongoose

**ML/AI:** CLIP (ViT-L/14), scikit-learn, RetellAI, n8n workflow automation

**Infrastructure:** GitHub Actions CI/CD, Docker, Render, Vercel, Cloudinary, Supabase

## Notable projects

### [PSO Onboarding App](https://github.com/UzairAhmedDahraj/pso-onboarding-app) — Microservices + ML Document Classification
Business partner onboarding system with an ML-powered document classifier running as a separate microservice. The backend (FastAPI + PostgreSQL) communicates with the ML service (PyTorch + CLIP) asynchronously via httpx. Deployed across Render, Vercel, and Hugging Face Spaces with 4 GitHub Actions CI/CD workflows handling independent deployment pipelines.

### [ResolveSuite](https://github.com/UzairAhmedDahraj/ResolveSuite) — Complaint Management System
Multi-tenant complaint management platform with a custom workflow engine that handles stage-based routing, automated escalation, deadline tracking, and email notifications. Built with a proper service layer (WorkflowService, EmailService, NotificationService, OTPService) on the backend. Frontend organizes features by domain (Complaint/, Department/, Workflow/, Feedback/) with shared common components.

### [Flight Search Voice Agent](https://github.com/UzairAhmedDahraj/Custom-Flight-Search-Agent) — RetellAI + Puppeteer
Voice-based flight search agent that integrates with RetellAI's conversation API. Scrapes live flight data from booking sites using Puppeteer with a managed browser pool, response caching, and a prefetcher for faster results. Built with Express, designed for deployment in DevContainers.

### [Audio Story Book](https://github.com/UzairAhmedDahraj/audio_story_book) — IoT Device Management
Backend system for managing IoT audio story devices. Handles firmware OTA updates with semver-aware version comparison, story content management with file uploads, and device registration. Built with Next.js API routes, MongoDB, and a typed service layer (FirmwareService, StoryService, DeviceService, FileService).

## How I think about code

I care about separation of concerns more than clever abstractions. In most of my projects, you'll see a consistent pattern: routes handle HTTP, controllers coordinate logic, services encapsulate business rules, and models define data. I prefer explicit service layers over stuffing everything into controllers, because when the workflow engine needs to send an email after advancing a complaint stage, that logic shouldn't live next to your route handler.

I also tend to pull ML workloads into separate services rather than bundling heavy dependencies into the main backend — the PSO app's architecture is a good example of that tradeoff.

## Get in touch

I'm open to opportunities involving full-stack development, AI/ML integration, or systems architecture.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/uzair.ahmed.dahraj/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/UzairAhmedDahraj)
