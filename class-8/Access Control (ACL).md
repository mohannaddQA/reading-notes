# Bearer Authorization

## 1- Role-based access control

### What is Role Based Access Control (RBAC) and why do we care?

RBAC is a security model that grants access based on roles assigned to users. It improves security, simplifies administration, and supports scalability. RBAC ensures users have appropriate access permissions, aids compliance, and enhances productivity.

### 2- Describe a Role/Permission heirarchy that you might implement using RBAC.

In an RBAC implementation, a typical role/permission hierarchy may include the following levels:

Superadmin Role: This role has the highest level of privileges and is responsible for managing the entire RBAC system. Superadmins can create and manage roles, assign permissions, and handle user assignments.

Admin Roles: These roles have administrative rights over specific functional areas or departments. They can manage users within their assigned domain, assign roles to users, and grant/revoke permissions accordingly.

User Roles: These roles represent different job functions or responsibilities within the organization. Users are assigned to specific roles based on their job requirements. Each user role is associated with a predefined set of permissions necessary to perform their tasks effectively.

Individual Permissions: These are the lowest level of access control. Individual permissions are specific actions or operations that can be performed on system resources. They are associated with user roles and determine the granular level of access a user has within the system.

By implementing this hierarchy, RBAC ensures a structured approach to access control, where superadmins have overall control, admins manage specific areas, and users are assigned roles with predefined permissions based on their responsibilities.

### 3-What approach might you take to implement RBAC?

Identify roles: Identify the different roles within your organization based on job functions and responsibilities. Determine the specific permissions each role should have.

Assign permissions to roles: Associate appropriate permissions with each role. Define the actions and operations that users in each role should be able to perform.

Group users into roles: Assign users to the roles that align with their job functions and responsibilities. Ensure that each user is assigned to the most appropriate role(s) based on their access needs.

Implement access controls: Implement access controls in your system based on the assigned roles and their associated permissions. This may involve configuring user management systems, setting up access control lists (ACLs), or using RBAC frameworks or libraries.

### 4-If Authentication is “you are who you say you are,” what is Authorization?

Authorization is the process of determining what a user is allowed to do or access after successful authentication. It verifies whether an authenticated user has the necessary permissions to perform specific actions or access certain resources within a system or application. In simpler terms, authorization answers the question, "What are you allowed to do?" based on the user's authenticated identity.

### 5- Name three primary rules defined for RBAC.

Role-Assignment Rule: Users are assigned to roles based on their job functions or responsibilities.

Role-Permission Rule: Roles are associated with specific permissions that define the actions and operations users can perform.

Permission-Inheritance Rule: Roles inherit permissions from higher-level roles in the role hierarchy, allowing for a hierarchical and scalable approach to access control.

### 6- Describe RBAC to a non-technical friend.

RBAC, or Role-Based Access Control, is a way to manage and control who can do what within a system or organization. Think of it like a building with different rooms and keys. In RBAC, each person is given a specific role, like "employee" or "manager," and each role has a set of permissions, like what rooms they can enter and what actions they can take. Instead of giving individual keys to each person, RBAC simplifies things by assigning keys to roles. So when someone joins the organization or changes roles, you just give them the right key (role) and they automatically get access to the appropriate rooms and actions they need for their job. It helps keep things secure, organized, and makes it easier to manage who can access what.

### 7- What Are access rights Associated with? The User? or The Role? Explain.

In RBAC, access rights are primarily associated with roles rather than individual users. Roles are predefined sets of permissions that define what actions or operations can be performed within a system. Users are then assigned to specific roles based on their job functions or responsibilities.

By associating access rights with roles, RBAC provides a more streamlined and scalable approach to access control. Instead of managing permissions individually for each user, administrators can simply assign users to roles, and the associated access rights are automatically granted. This simplifies administration, reduces complexity, and makes it easier to manage access control in large organizations or systems with many users.

Additionally, associating access rights with roles allows for easier role-based changes and updates. If a user's responsibilities change, their role can be updated, and the corresponding access rights will be adjusted accordingly. This flexibility ensures that users have the appropriate level of access permissions based on their roles, making access management more efficient and effective.

### 8- Access Rights, or Authorization, is activated after a user successfully does what?

Access rights, or authorization, are activated after a user successfully authenticates or proves their identity. Authentication is the process of verifying that a user is who they claim to be, typically through credentials such as usernames and passwords, biometrics, or other authentication methods.

Once a user has been authenticated, the system or application can then proceed to authorize the user by granting them the appropriate access rights based on their authenticated identity. Authorization determines what actions the user is allowed to perform and what resources they can access within the system.

In summary, access rights or authorization are activated after a user successfully authenticates their identity.

### 9- Explain how RBAC might benefit a business.

RBAC benefits businesses by improving security, simplifying administration, ensuring compliance, increasing productivity, enabling scalability, and promoting effective collaboration among teams.
