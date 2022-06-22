# Code 401 - Class 08 - Access Control (ACL)

## [5 steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

### What is Role Based Access Control (RBAC) and why do we care?

- RBAC = allowing different levels of access to users based on their role at a company
- If implemented correctly, it can become a systematic and easily-repeatable way to manage access to information, ultimately making that info more secure

### Describe a Role/Permission heirarchy that you might implement using RBAC

- Basic user role (basic access)
- Customer Service rep (read/write access to customer database)
- Customer database admin (full control of customer database)

### What approach might you take to implement RBAC?

- The article suggests:
>
> 1. Inventory your systems (email systems, customer database, etc.)
> 2. Analyze your workforce and create roles
> 3. Assign people to roles (can cause the system to quickly unravel)
> 4. Never make one-off changes
> 5. Audit to ensure effectiveness

## [wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)

### If Authentication is “you are who you say you are,” what is Authorization?

- Authorization = access allowed to certain resources

### Name three primary rules defined for RBAC

- According to wikipedia:
>
> 1. Role assignment
> 2. Role authorization
> 3. Permission authorization

### Describe RBAC to a non-technical friend

- RBAC is an approach to access management that creates a heirarchy or structure of access that is based on someone's role at a company. For instance, a financial analyst might need access to the financial systems, while a customer service rep may not - so the CSR would not have access to those systems. But the CSR might be given access to a customer database, while the analyst would not because they have no need for it.

## [RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)

### What Are access rights Associated with? The User? or The Role? Explain

- They are associated with the role, NOT the user.

### Access Rights, or Authorization, is activated after a user successfully does what?

- Authenticates themselves

### Explain how RBAC might benefit a business

- Policy does not need to change based on who is brought on, or who leaves the company
- Automated access to specific resources

[Back to Home](../README.md)
