# SSCP-1 | Plain text secret

**🔐 Ensure there is no plain text secret (password, tokens, ...) in the repository files**
- Scope: Git repository files
- Statement: No cleartext secrets shall be stored or transmitted in any file of a repository.
- Rationale: Cleartext secrets pose a significant security risk as they can be easily compromised if a system is breached. Storing secrets in plain text makes it possible for unauthorized individuals to access sensitive systems and data.
- Controls:
    - Scan all your repository files **throughout the entire git history (every commit)** to search for cleartext secrets
      - Example: inside a git repository containing a Go project, there is a plain text `Personal access token` in the `request.go` file
        ```golang
        client := graphql.NewClient(graphQLURL)                      
        req := graphql.NewRequest(request)
        req.Header.Add("Authorization", "Bearer glpat-UoLK3Pgax8Kio7Ukx")  
        ```