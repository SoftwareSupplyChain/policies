
# Supply Chain Policies

How are you securing your software supply chain today? If the answer feels unclear or overwhelming, you're not alone. Software supply chain security can be a massive, confusing topic, and many teams struggle to figure out where to begin.

This repository is here to change that. We've created a community-driven, easy-to-follow checklist of essential policies to secure your software supply chain.

You'll find clear, actionable policies that help you confidently protect your supply chain and ensure compliance with security best practices, all in one place. Let's make this easier together!


## 📋 What is a policy

A policy is a set of controls that define how an organization should operate to achieve a specific security or compliance objective. Policies are supported by:
- A title
- A scope
- A statement
- A rationale
- A set of actionable controls

### Policy example

**🔐 Ensure there is no clear secret (password, tokens, ...) in the repository**
- Scope: Git repository
- Statement: No cleartext secrets shall be stored or transmitted in any file of a repository.
- Rationale: Cleartext secrets pose a significant security risk as they can be easily compromised if a system is breached. Storing or secrets in plain text makes it possible for unauthorized individuals to access sensitive systems and data.
- Controls:
    - Scan all your repository files **in the whole git history (every commits)** to search for clear secrets


## 🖊️ How to contribute

*Work in progress*
