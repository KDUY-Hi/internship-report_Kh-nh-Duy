---
title: "Blogs Posted"
date: 2026-07-29
weight: 4
chapter: false
pre: " <b> 4. </b> "
---

## Overview

During the project, the team not only built a practical application but also summarized the learning process into technical blog posts. These posts helped organize the analysis, solution design, backend/frontend implementation, and use of AWS services in the project.

## Blog List

| Blog | Topic | Main Content | Learning Value | Link |
| --- | --- | --- | --- | --- |
| Blog 1 | Building Secure Applications from the Design Phase with AWS Security Agent | Explains why security should be considered during system design, introduces AWS Security Agent, Threat Modeling, and applies the ideas to the Student Internship Portal project. | Learned the "Design for Security" mindset, how to identify architectural risks early, and how to improve AWS deployments more securely. | [Facebook post](https://www.facebook.com/groups/660548818043427?multi_permalinks=2227782947986665) |
| Blog 2 | AI Code Review with AWS Security Agent | Explains how AWS Security Agent helps analyze source code and detect security risks in login APIs, CV upload, and internship-post management before deployment. | Learned that an application can work functionally but still be insecure, and gained a clearer understanding of secure coding and automated code review. | [Facebook post](https://www.facebook.com/groups/660548818043427/?multi_permalinks=2228768907888069) |
| Blog 3 | Deploying the Project on AWS | Summarizes how the backend was deployed on EC2, how RDS PostgreSQL was used for the database, how S3 stored CV files, and how CloudWatch supported log monitoring. | Understood the process of moving an application from local development to the cloud and the key points to consider during deployment. | To be updated |

## Blog 1 - Building Secure Applications from the Design Phase with AWS Security Agent

The first blog post belongs to the **AWS Security Agent** series. It focuses on the idea that security should not only start after an application has been completed. A secure design from the beginning can help development teams identify and remove many risks before they become vulnerabilities in source code or deployment environments.

The post emphasizes that many security issues do not come directly from programming mistakes, but from early architectural decisions. For example, a database may be placed in a network area that is reachable from the Internet, an API may lack a proper authentication mechanism, or AWS services may receive permissions beyond their actual needs. If these issues are discovered only after the system is complete, fixing them often requires more time and cost.

### AWS Security Agent

The blog introduces **AWS Security Agent** as an AI assistant that helps development teams evaluate the security of a system from the design phase. Instead of only scanning source code, Security Agent can analyze design documents, architecture diagrams, data flows, AWS deployment configurations, and relationships between services.

From this information, the tool can help identify potential security risks and suggest improvements before the team starts coding or deploying the system. This represents a shift in mindset from **Fix Security** to **Design for Security**.

### Threat Modeling

An important part of the post is **Threat Modeling**, which is the process of analyzing a system to identify potential threats. It helps answer questions such as what the system needs to be protected from, which components are most exposed, how an attacker might exploit the system, and what design changes are needed to reduce risk.

AWS Security Agent does not replace security experts, but it can help development teams detect architectural problems earlier before they become real vulnerabilities in the product.

### Connection to the Student Internship Portal Project

The blog applies these ideas to the **Cloud-based Student Internship Portal on AWS** project. The system uses services such as Amazon CloudFront, Amazon S3, Amazon EC2, Amazon RDS PostgreSQL, AWS IAM, and Amazon CloudWatch. From a security perspective, the team needs to consider whether RDS is placed in a private subnet, whether EC2 exposes SSH to the entire Internet, whether IAM Roles have excessive permissions, and whether data exchanged between components is encrypted.

One practical example is deploying Amazon RDS with public access enabled for convenience during development. Functionally, the system may still work normally, but from a security perspective, this introduces significant risk. AWS Security Agent can recommend placing RDS in a private subnet, allowing access only from EC2 through Security Groups, and removing direct access from the Internet.

### Key Takeaways

Through this blog post, I learned that a good architecture is not only one that works correctly, but also one that is secure, controllable, and able to reduce risks early. Evaluating security from the design phase helps reduce remediation cost, supports developers in understanding the impact of architectural decisions, and establishes a foundation for DevSecOps thinking in later development stages.

Blog post link: [Facebook post](https://www.facebook.com/groups/660548818043427?multi_permalinks=2227782947986665)

Reference: [AWS Security Agent](https://aws.amazon.com/vi/security-agent/)

## Blog 2 - AI Code Review with AWS Security Agent

The second blog post in the **AWS Security Agent** series focuses on the stage after the initial system design: reviewing source code before the application is deployed. The main idea is that an application working correctly from a functional perspective does not necessarily mean that it is secure against real-world attacks.

The post emphasizes that many security vulnerabilities appear during implementation. An API may satisfy business requirements but still contain authentication issues, insufficient input validation, weak authorization checks, or logs that expose sensitive information. These problems are often difficult to detect through normal functional testing.

### AI Code Review

AI Code Review is the process of using artificial intelligence to analyze source code, identify security risks, and suggest improvements. Unlike tools that only check syntax or code formatting, AI Code Review tries to understand the application context, including processing flows, API data, authentication logic, authorization mechanisms, and interactions with databases or external services.

With AWS Security Agent, review can be applied to Pull Requests or to the whole project. The Agent can read new code, identify risky areas, explain the cause, assess the potential impact, and recommend suitable fixes.

### Connection to the Student Internship Portal Project

The blog uses the **Cloud-based Student Internship Portal on AWS** project to illustrate common security issues in code.

For the **login API**, AWS Security Agent can check risks such as overly long JWT lifetimes, missing login-attempt limits, improper password handling, or error messages that reveal too much information. For example, if the system returns separate messages such as "Email does not exist" and "Incorrect password", attackers may use the difference to identify valid accounts. A safer approach is to use a generic message such as "Email or password is incorrect".

For the **CV upload API**, successful upload does not guarantee security. The system should validate file type, file size, file name, actual file content, and the way files are stored on S3. AWS Security Agent can suggest additional checks to reduce the risk of malicious or invalid file uploads.

For the **internship-post management API**, a common issue is checking only whether a user is logged in without checking whether the user owns the resource. This can lead to one company editing or deleting another company's internship posts. The Agent can identify missing authorization checks and suggest verifying ownership before performing the action.

### Value of AWS Security Agent

An important value of AWS Security Agent is that it does not only point out problematic code. It also explains why the issue is a security risk, what the impact could be if exploited, how an attacker might abuse it, and how to fix it. This makes code review a learning activity for secure coding, especially for development teams with limited security experience.

### Key Takeaways

Through this blog post, I learned that functional testing and security review are different perspectives. Features such as login, CV upload, and internship-post management may work correctly but still need careful review for authentication, authorization, validation, logging, and data access control. Integrating AI Code Review into the development workflow helps detect risks earlier, reduce remediation cost, and improve code quality before deployment.

Blog post link: [Facebook post](https://www.facebook.com/groups/660548818043427/?multi_permalinks=2228768907888069)

## Lessons Learned

Writing blog posts gave me an opportunity to review the whole project in a more structured way. Instead of only focusing on code, I had to explain the problem, the reason for choosing each technology, how the components connected with each other, and the results achieved after implementation.

This activity helped me improve technical communication, documentation writing, information selection, and the ability to explain a technology solution in a clearer way for readers.
