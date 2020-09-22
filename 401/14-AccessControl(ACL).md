# Access Control (ACL)
![](https://redislabs.com/wp-content/uploads/2020/06/Adobe-ACL-image.jpg)
is an approach to restricting system access to authorized users.
> user working on a public network, while in a coffee shop.  The user’s credentials were compromised, resulting in the compromise of the company’s entire infrastructure.

## Role-based access control (RBAC) approach
assigning system access to users based on their role within an organization.
- With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.

## RBAC implementation 
1. Inventory your systems
2. Analyze your workforce and create roles
3. Assign people to roles
4. Never make one-off changes
5. Audit

## Review, Research, and Discussion

### When is Basic Authorization used vs. Bearer Authorization?
- Basic auth it is used when need just to login 
- Bearer It is the recommended Authentication methods whenever possible. It is ideal when scripting, when developing external app or when doing integration with external tools.

### What does the JSON Web Token package do?
securely transmitting information between parties as a JSON object.

### What considerations should we make when creating and storing a SECRET?
Store secrets safely and Use encryption to store secrets within .git repositories

- `Encryption `is the method by which information is converted into secret code that hides the information's true meaning
- `tokens` are used in token-based authentication to allow an application to access an API. The application receives an access token after a user successfully authenticates and authorizes access, then passes the access token as a credential when it calls the target API.
- `Bearer` Token is an opaque string, not intended to have any meaning to clients using it. Some servers will issue tokens that are a short string of hexadecimal characters, while others may use structured tokens such as JSON Web Tokens.