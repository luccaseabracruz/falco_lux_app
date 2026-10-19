# Falco Lux App - Security Guidelines

Use the **10 OWASP Security by Design principles** as lightweight guidelines throughout the project.

I am developing this project primarily as a solo developer, so do not turn these principles into a formal compliance exercise or introduce unnecessary complexity.

The goal is to make sensible security decisions from the beginning.

When relevant, consider:

1. Minimize attack surface
    
2. Establish secure defaults
    
3. Apply least privilege
    
4. Use defense in depth
    
5. Fail securely
    
6. Don't trust services
    
7. Separate responsibilities where practical
    
8. Avoid security through obscurity
    
9. Keep security simple
    
10. Fix security issues correctly
    

### Practical approach

Apply these principles proportionally to the project's size and risks.

Prioritize fundamentals such as:

- proper authentication;
    
- server-side authorization;
    
- RBAC;
    
- input validation;
    
- secure password handling;
    
- secure session/token handling;
    
- HTTPS in production;
    
- secrets kept outside source code;
    
- safe error handling;
    
- dependency updates;
    
- database access controls;
    
- avoiding unnecessary exposed services;
    
- appropriate logging;
    
- backups;
    
- basic security testing.
    

Do not introduce a complex security mechanism merely because it can be associated with one of the principles.

When making a security-related decision, briefly ask:

> **What are we protecting, what could go wrong, and what is the simplest reasonable way to reduce that risk?**

If a security issue is found, prefer understanding and fixing its root cause rather than applying a superficial workaround.

The objective is not to make the project perfectly secure. The objective is to **systematically avoid preventable security problems and develop good Security by Design habits**.
# References
- [Principles of security](https://devguide.owasp.org/en/02-foundations/03-security-principles/)