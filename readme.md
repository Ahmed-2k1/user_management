
## Introduction:
The User Management Project involved enhancing the existing user management functionality by addressing key issues, adding features, and ensuring the robustness of the system through additional test cases and improvements in logging and error handling.

## Key Issues Resolved:

1. **Duplicate Login Endpoint Removed:**
Simplified the user route by removing a redundant login endpoint, ensuring only a single login route exists. This reduces redundancy, improves maintainability, and prevents potential inconsistencies in login logic.
Link to the issue:  https://github.com/Ahmed-2k1/user_management/tree/11-duplicate-login-endpoint

2. **Email Missing UUID:**
Resolved an issue where emails were sent before the user was added to the database by ensuring the email is sent after successful database insertion.
Link to the issue:  https://github.com/Ahmed-2k1/user_management/tree/2-email-missing-uuid

3. **GitHub and LinkedIn URLs Null in Create User Response:**
Ensured GitHub and LinkedIn URLs are correctly mapped to the response object in the create user functionality.
Link to the issue:  https://github.com/Ahmed-2k1/user_management/tree/7-github-and-linked-url-are-null-in-create-user

4. **User role is anonymous when user created as admin:**
Role is getting default to Anonymous even after verification it doesn’t change to admin. Fix: Added code for role to be admin if user is created as admin
Link to the issue: https://github.com/Ahmed-2k1/user_management/tree/9-user-role-is-anonymous-when-user-created-as-admin

5. **Email ID update:**
Cause: Success response is given on trying to update email with already existing email. Fix: Check was done by retrieving data based on mail and if it's already present then error is thrown.
Link to the issue: https://github.com/Ahmed-2k1/user_management/tree/5-email-id-update



## Added Features:
User Profile Management
Enhanced user profile management by allowing users to update fields such as name, bio, and location, and enabling managers or admins to upgrade users to professional status. This included API endpoints, profile page updates, notifications, and optional field validation.
Commit Link: https://github.com/kaw393939/user_management/commit/f96bbe65eaa1bb300032a816b25cb09d9ec8b646

## What I Learned:
Through this project, I gained practical experience in debugging and resolving critical issues, implementing robust logging and error-handling mechanisms, and enhancing application security through features like password validation. I also learned the importance of maintainable code through refactoring, detailed documentation, and testing. Adding 31 extra test cases helped me understand the value of comprehensive testing to ensure the reliability of new features and changes.
