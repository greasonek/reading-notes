# Class 08 Reading Notes

## 5 Steps to RBAC

1. What is Role Based Access Control (RBAC) and why do we care?

- Restricts network access based on a person's role within an organization. Refers to the level of access employees have to the network. <a href="https://www.digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more">Source</a>. RBAC can prevent data breach/hacking related breaches that occur because of compromised credentials. 

2. Describe a Role/Permission heirarchy that you might implement using RBAC.

- In a customer database, you would have a basic user role with access to email and website, then a role for customer service rep with access to read/write to the customer database, then a customer database admin with full control of the costumer database. <a href="https://www.csoonline.com/article/555873/5-steps-to-simple-role-based-access-control.html">Source</a>

3. What approach might you take to implement RBAC?

## wiki - RBAC

1. If Authentication is “you are who you say you are,” what is Authorization?

- Authorization allows the authenticated user to perform roles for which they are authorized or assigned to.

2. Name three primary rules defined for RBAC.

- role assignment: a subject can exercise a permission if they have been assigned a role
- role authorization: a subject's active role must be authorized for the subject.
- permission authorization: a subject can exercise permission if it is authorized for the subject's active role.

3. Describe RBAC to a non-technical friend.

- For example, within a company's Google suite, some users are authorized as admin roles and can perform certain exercises such as assigning roles, denying access, creating new users, authorizing certain exercises for other users, etc. Whereas other user's without those authorized exercises can perform tasks they have been authorized to perform like sending emails, adding meetings to the Google calendar, changing their personalized email signature, etc but they cannot add new users or control the authorization of other users like a user in an admin role can.

## RBAC Tutorial

1. What Are access rights Associated with? The User? or The Role? Explain.

- rights are associated with the role not the user. What role do I have in my system and what resources do they need access to? People in this role can have access to this right. Users must be activated to role and based on the role, they will be given certain rights.

2. Access Rights, or Authorization, is activated after a user successfully does what?

- authenticate themselves to the system and have roles activated for them.

3. Explain how RBAC might benefit a business.

- policy does not need to be changed when any certain person leaves the business organization because rights are assigned to roles, not users.
- new employees can activate desired roles

## Things I want to know more about

- RBAC implementation