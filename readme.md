Links for Q/A issues and Test scripts:
There are 14 test cases written in total. Each branch has test cases to test the necessary changes. You can verify it in the commits of the branch. The commit would be named as testcase for testcases written.

Issue 1: Verify Email missing UUID.
Cause: Email was being sent before the user got added to the DB.
Fix: Mail was made to sent after the user was added to the DB.
[Issue link:](https://github.com/Abishek183/final_project_user_management/issues/1)
Link for fix and test case: [Link](https://github.com/Abishek183/final_project_user_management/tree/1-email-missing-uuid)


Issue 2: Email id update to existing email
Cause: Success response is given on trying to update email with already existing email.
Fix: Check was done by retrieving data based on mail and if its already present then error is thrown.
[Issue link:](https://github.com/Abishek183/final_project_user_management/issues/3)
Link for fix and test case: [Branch Link](https://github.com/Abishek183/final_project_user_management/tree/3-email-id-update)

Issue 3: GitHub and LinkedIn URL are null in create user.
Cause: GitHub URL and LinkedIn URL are null in the response of the create user.
Fix: Values are being correctly mapped to response object.
[Issue link:](https://github.com/Abishek183/final_project_user_management/issues/5)
Link for fix and test case: [Branch Link](https://github.com/Abishek183/final_project_user_management/tree/5-github-and-linked-url-are-null-in-create-user)

Issue 4: User role is Anonymous when user created as Admin.
Cause: Role is getting default to Anonymous even after verification it doesn’t change to admin.
Fix: Added code for role to be admin if user is created as admin.
[Issue link:](https://github.com/Abishek183/final_project_user_management/issues/8)
Link for fix and test case: [Branch Link](https://github.com/Abishek183/final_project_user_management/tree/8-user-role-is-anonymous-when-user-created-as-admin)

Issue 5: Deleting URL fields is giving error.
Cause: The fields don’t accept empty string to delete the value.
Fix: a validator was added to check if the incoming field is empty then the value is set to null.
[Issue Link:](https://github.com/Abishek183/final_project_user_management/issues/12) 
Link for fix and test case: [Branch Link](https://github.com/Abishek183/final_project_user_management/tree/12-deleting-url-fields-is-giving-error)


Feature:
I have chosen the feature 9 which is User Profile Management. In this we need to create two endpoints, one for updating self-profile fields(/users/updateMyProfile/) and the other for managers and admin to upgrade status of users to professional (/users/{user_id}/upgrade/). Once the professional field is updated, we should notify the user in email that their status has been updated.
Code changes and test script: [link](https://github.com/Abishek183/final_project_user_management/tree/feature)
