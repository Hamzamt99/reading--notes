# Access Control:
## 5 steps to RBAC:

### What is Role Based Access Control (RBAC) and why do we care?
*Role-Based Access Control (RBAC) is a security model that assigns permissions to users based on their roles.
We care about RBAC because it simplifies access management, improves security by enforcing least privilege, and ensures compliance with access control policies.*

### Describe a Role/Permission heirarchy that you might implement using RBAC:
*In a RBAC implementation, a typical role/permission hierarchy could include a "Superadmin" role with full access rights,
followed by an "Admin" role with administrative privileges but restricted to certain actions, and a "User" role with limited access rights and basic functionalities.*

### What approach might you take to implement RBAC?
*To implement RBAC, you can follow these steps:*
1. Identify and define roles based on user responsibilities and access requirements.
2. Determine the permissions associated with each role, specifying what actions and resources they can access.
3. Assign users to appropriate roles based on their job functions and responsibilities, ensuring that access is granted based on role membership rather than individual permissions.

## wiki - RBAC:

### If Authentication is “you are who you say you are,” what is Authorization?
*Authorization is "what you are allowed to do" or the process of granting or denying access to resources based on the authenticated user's permissions and privileges.
It ensures that authenticated users are granted appropriate access rights and privileges based on their roles or defined permissions, while preventing unauthorized actions and protecting sensitive information.*

### Three primary rules defined for RBAC are:
1. Role assignment: Users are assigned roles based on their job functions or responsibilities.
2. Role authorization: Roles are granted permissions and access rights to perform specific actions and access resources.
3. User-role relationship: Users are associated with roles, and their access is determined by the permissions assigned to those roles, ensuring that users inherit the access rights of their assigned roles.

### RBAC is like having different keys for different doors. Imagine a building where each person has a specific key that opens only the doors they need. Roles are like key sets, where each set has access to certain doors. So, instead of managing individual keys for each person, RBAC simplifies access control by giving people a key set (role) that opens the right doors they need for their job, making it efficient and secure:
*RBAC is like having different keys for different doors. Imagine a building where each person has a specific key that opens only the doors they need.
Roles are like key sets, where each set has access to certain doors. So, instead of managing individual keys for each person, RBAC simplifies access control by giving people a key set (role) that opens the right doors they need for their job, making it efficient and secure.*
