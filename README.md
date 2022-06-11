# Apache Web Server - AWS Cloudformation

This template deploys a VPC, with a pair of public and private subnets spread 
across two Availabilty Zones. It deploys an Internet Gateway, with a default 
route on the public subnets. It deploys a pair of NAT Gateways (one in each AZ), 
and default routes for them in the private subnets. And finally the web server will be deployed
in each of the private subnets and each of the availability zones to ensure availability.

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

