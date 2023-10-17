# Class 33 Reading Notes

## What is Role Based Access Control (RBAC)?

1. What is Role Based Access Control (RBAC)?

- RBAC refers to the level of access individuals have. It restricts access based on a person's role within an organization.

2. Share some an example of RBAC including all possible CRUD operations and correlating roles.

- Some examples include management role scope, group and assignemnt.
  - management role scope limits what objects the role gropu is allowed to manage.
  - management role group tool can add and remove members
  - manaement role is based on role groups.
  - role assignment links a role to a certain group.

- For example, an admin can have Create, Read, Update and Delete permissions while a regular user or employee may only have read and create permissions.

3. What are the Benefits of RBAC?

- RBAC can reduce the amount of paperwork or password changes when an employee is hired or changes roles. It offers a streamlined approach to operational efficiency. It also improves compliance and gives executives and/or IT departments the ability to manage how data is accessed and used.

## React-Cookie Library vs. React-Cookies Component

1. Describe some react-cookie features.

- react-cookie allows users to set a cookie value with a name, value, and an object param that holds cookie options, it also allows users to remove a cookie and update cookies. It makes it easy to access cookies in components.useCookies allows you to access cookies and CookiesProvider makes cookies available to child components.

2. Describe some react-cookies features.

- react-cookies allows users to set and remove cookies,it also allows you to load the user cookies so you can do server-rendering and match new cookies.

3. Which library would you prefer would you prefer? Why?

- With the knowledge I currently have I would prefer to use react-cookie because it seems that there is more information about it, it has more features and makes cookies more managable.
