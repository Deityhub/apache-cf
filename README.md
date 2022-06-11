# Apache Web Server - AWS Cloudformation

In this project, will deploy web servers for a highly available web app using CloudFormation.

## Template Usage
1. Make the scripts executable

    ```
    # Make create script runnable
    chmod +x ./create.sh

    # Make update script runnable
    chmod +x ./update.sh
    ```

2. Create cloudformation stack
   ```
   ./create.sh <stack name> final-project-starter.yml server-parameters.json
   ```
   > Change \<stack name\> to any value of your choice

3. Update stack
   ```
   ./update.sh <stack name> final-project-starter.yml server-parameters.json
   ```

