
Run Synthetic Tests from Private Locations

Overview
Private locations allow you to monitor internal-facing applications or any private endpoints that aren’t accessible from the public internet.

Configure your private location by customizing the generated configuration file and this configuration file is in json format and we have stored this file in ssm parameter. To fetch the ssm parameter inside cluster we are using secrets-store-csi-driver and mounting it inside a pod to create a secret from it so DataDog agent can run with this configuration file. 

