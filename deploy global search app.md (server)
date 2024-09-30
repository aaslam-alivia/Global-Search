Deployment Instructions
Follow the steps below to build and deploy the necessary components using Jenkins.

Access Jenkins
Visit the following URL:
DevOps Independent Pipeline

Steps to Build and Deploy
1. Build AI Commons
Locate DevOps_Ind_03_Build_AI_Commons.
Right-click on it and select Build with Parameters.
Enter the {branch} and click Build.
Wait for all steps to complete successfully (all should turn green).
2. Build Alivia Messenger
Locate DevOps_Ind_02_Build_AliviaMessenger.
Right-click on it and select Build with Parameters.
Enter the {branch} and click Build.
Wait for all steps to complete successfully (all should turn green).
3. Deploy Case Manager Release
Locate DevOps_Ind_06_Deploy_CaseManager_Rlse.
Right-click on it and select Build with Parameters.
Enter the {branch} and the target {server} for deployment.
Wait for all steps to complete successfully, especially ensure that the Execute Ansible Script Check passes.
4. Deploy AI Tenant Secrets Map
Locate DevOps_Ind_44_Deploy_AI_Tenant_Secrets_Map.
Right-click on it and select Build with Parameters.
Enter the {branch} and the target {server} for deployment.
Wait for all steps to complete successfully, especially ensure that the Execute Ansible Script Check passes.
5. Deploy AI Global Search
Locate DevOps_Ind_43_Deploy_AI_Global_Search.
Right-click on it and select Build with Parameters.
Enter the {branch} and the target {server} for deployment.
Wait for all steps to complete successfully, especially ensure that the Execute Ansible Script Check passes.
Important Notes
Run these tasks in serial order to ensure proper dependency handling.
Once all builds and deployments are complete, you can start additional tasks.
Troubleshooting
If you encounter any issues during the process:

Rebuild AI Commons.
Rebuild Alivia Messenger.
Feel free to reach out if you need further assistance!
