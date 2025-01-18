# Jerrel Gordon

## AWS Cloud Resume Challenge

Hello! I'm **Jerrel Gordon**, a Software Engineer with a background in **Control Systems** within the **manufacturing industry**. I studied **Computer Science** at the **Florida Institute of Technology**, graduating **magna cum laude**. During my time there, I served as president of **Upsilon Pi Epsilon**, the Computer Science honor society. My concentration was in **Cybersecurity**, and I focused on research involving **DNS (DOH, DOT, DNSSEC)**, comparing security and efficiency using **NFV** and **SDN** concepts, while leveraging **OpenStack** for implementation. This research ignited my passion for **Cloud Computing**, leading me to dive deeper into AWS services and cloud architecture.

So here is my version of the **Cloud Resume Challenge**! 🎉
**https://cloudresumechallenge.dev/docs/the-challenge/aws/**
---

## The Project

This project is a **state-driven single-page web app** built with the **Svelte** framework, integrating several **AWS services** such as **S3**, **CloudFront**, **Route 53**, **ACM**, **IAM**, **Lambda**, **API Gateway**, and **DynamoDB**. The goal is to create a dynamic, serverless web app that showcases my **cloud resume**, all while leveraging modern web technologies and AWS services.

---

## How I Got Here

I didn’t always find web development exciting. Early on, I was more focused on other areas of tech. But then, in a random Reddit thread, I stumbled upon **Svelte**, a lightweight and modern framework. Intrigued by its simplicity and performance, I decided to give it a try.

At the same time, I was diving deeper into **cloud computing**, studying for the **AWS Solutions Architect** and **AWS Associate Developer** certifications. This project was the perfect opportunity to merge both my web development skills and cloud knowledge into one fun, practical challenge!

---

## Project Breakdown

### Frontend: Svelte Framework

**Svelte** was the ideal choice for this project because it:
- **Compiles to efficient JavaScript**: The build output is small and fast.
- **Uses reactive state management**: Makes it easy to create dynamic, state-driven components.
- **Offers a simple developer experience**: The syntax is clean, and setup is straightforward, allowing me to focus on building the app rather than fighting the framework.

The frontend displays my cloud resume in a clean, user-friendly web app, with data pulled from AWS services like **DynamoDB**.

### Backend: AWS Services

To power the app’s backend, I leveraged various AWS services:
- **S3**: Hosts the build artifacts of my Svelte app.
- **CloudFront**: Serves the content via a CDN for fast global access.
- **Route 53**: Manages DNS for the custom domain and directs traffic to S3 and CloudFront.
- **ACM**: Provides an SSL certificate for secure HTTPS connections.
- **IAM**: Used to create a github user for programmatic access.
- **DynamoDB**: Keeps track of the number of visits my webapp has gotten.
- **Lambda & API Gateway**: Handles serverless functions for updating the visitor count.

These services work together to make the app fully functional, scalable, and secure.

---

## CI/CD Pipeline with GitHub Actions

To automate deployments, I set up a **CI/CD pipeline** using **GitHub Actions**. Here's how it works:
- **GitHub Actions** is triggered every time I push to the `main` branch.
- It installs the project dependencies, runs `npm run build` to generate static files, and syncs the build output to the **S3 bucket**.
- It then nvalidates the **CloudFront cache** to ensure the latest version of the app is served.

This pipeline ensures that the app is always up to date, and I don’t have to manually deploy changes every time.

### Secrets and Security

To keep my AWS credentials safe, I store sensitive data like **AWS_ACCESS_KEY_ID**, **AWS_SECRET_ACCESS_KEY**, **CLOUDFRONT_DISTRIBUTION_ID** and the **S3_BUCKET_NAME** in **GitHub Secrets**. This prevents accidental exposure of credentials in the codebase.

---

## Final Thoughts

This project has been a great way to combine my growing skills in **web development** and **cloud computing**. By building and deploying a serverless web app, I’ve gained hands-on experience with key AWS services and learned how to automate deployments with GitHub Actions. I’m excited to continue exploring cloud technologies and web development as I grow my skills.

Thanks for checking out my **Cloud Resume Challenge** project! 🌐🚀

---